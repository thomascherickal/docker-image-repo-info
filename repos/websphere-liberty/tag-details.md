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
$ docker pull websphere-liberty@sha256:30f5d32d5b952493cd9b4d82043a3f8d430f50fdb4046388bb3e673c3f48598e
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
$ docker pull websphere-liberty@sha256:eaa097ef38324aac0f147d3f0b6813d915533b9b9968f3a48cbbed128b8d676c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.7 MB (396695982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3ba97273459980c1b9a8d45e57f0e45c2150d83d817a20eaebd8638115284dd`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:20:15 GMT
ADD file:014236839eaee978894ae0bd6aecc246177a0a2c11af73f86d9cfafe5478ce18 in / 
# Fri, 07 Jan 2022 02:20:19 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:29 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:22:19 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:23:02 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 01:26:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:26:46 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:26:48 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:27:31 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:37:48 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:37:49 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:45:16 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Tue, 01 Feb 2022 02:45:18 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Tue, 01 Feb 2022 02:45:20 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Tue, 01 Feb 2022 02:45:22 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:45:24 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Tue, 01 Feb 2022 02:45:25 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:45:28 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:45:50 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:45:56 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:45:58 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl21.0.0.12920-1900
# Tue, 01 Feb 2022 02:46:00 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:46:05 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:46:05 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:46:06 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:46:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:46:26 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:46:30 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:46:32 GMT
USER 1001
# Tue, 01 Feb 2022 02:46:34 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:46:37 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:46:39 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 01 Feb 2022 02:47:02 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:47:05 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 01 Feb 2022 02:51:17 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 01 Feb 2022 02:51:23 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 01 Feb 2022 02:52:16 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:e6e6dea5a8cc4bdc9e5e51e2bfa948159b69d5fbc2dca99bc41776fb04dab967`  
		Last Modified: Fri, 07 Jan 2022 02:22:43 GMT  
		Size: 33.3 MB (33286892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2db03674d664c4c13747eecf6ee9d3578adc9eb95e5a3993661ba5f37f676f8`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 17.2 MB (17206916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0441717da968406ddb594da0c1ad05e5f42434a3584422d7fab7e64763e30b4`  
		Last Modified: Tue, 01 Feb 2022 01:39:44 GMT  
		Size: 48.4 MB (48356102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6fe9db05a97733f7b24220942aef850723e6992236fcba495134a2fc03a312b`  
		Last Modified: Tue, 01 Feb 2022 01:39:36 GMT  
		Size: 3.3 MB (3331743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd951b2f63ad5c87a257c00ace1b87917a17bc55f2d7f51cf49e4f03e723aa1e`  
		Last Modified: Tue, 01 Feb 2022 03:00:16 GMT  
		Size: 14.3 MB (14286603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2467ca4cde039e05b93a30920246f8c81f15fed4abc15d6bc8445b4e65f8d0`  
		Last Modified: Tue, 01 Feb 2022 03:00:12 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e827664c35967cbc0924137b4b51288f2080d8773dbd9371d0f0f579b0903e`  
		Last Modified: Tue, 01 Feb 2022 03:00:12 GMT  
		Size: 9.7 KB (9668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca060c94cc295078bd7c8dd0290c0675ece69e8ac9dc69a0a4de2b5774f4d02`  
		Last Modified: Tue, 01 Feb 2022 03:00:12 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77553ab561424ad8114dfcd67bf39142266456ff0d7e784d5d325d22eed2feb5`  
		Last Modified: Tue, 01 Feb 2022 03:00:12 GMT  
		Size: 10.7 KB (10658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f145a66885ecddb48e51e2edb9f025b46027536c746bc236af5527961b4e7d`  
		Last Modified: Tue, 01 Feb 2022 03:00:12 GMT  
		Size: 2.5 MB (2475054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a18f69769cd5022f69a78fef5fbf0f62a3f8100500f148fdd3f0ec0e4c8df1a`  
		Last Modified: Tue, 01 Feb 2022 03:00:53 GMT  
		Size: 264.6 MB (264635327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ffe2e46f2ad6c70e99887641402f75413278a0451193f4b9d137f2e4dca101`  
		Last Modified: Tue, 01 Feb 2022 03:00:24 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b557cb4bddde7a1d4271c349c52a444a464ad6b0496cd6f75910c93dc87c959`  
		Last Modified: Tue, 01 Feb 2022 03:00:27 GMT  
		Size: 13.1 MB (13095108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:a347c85a122a09b9ed935ee1d4cd2bfbe35db0aabaa4e11a5860bb4106d71eda
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **389.6 MB (389578170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ad23677262196438f13f587ed293ba88b4cf0e708cc081c5325286d40f7f570`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 01:42:20 GMT
ADD file:b6119f4fcd6a113749f515278b315ffd96aecce7006f086acb060f981e5c59db in / 
# Fri, 07 Jan 2022 01:42:22 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:15:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 02:24:31 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:00:54 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 02:01:59 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 02:02:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:02:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 02:02:34 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:40:32 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:40:32 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:46:33 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Tue, 01 Feb 2022 02:46:33 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Tue, 01 Feb 2022 02:46:33 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Tue, 01 Feb 2022 02:46:33 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:46:33 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Tue, 01 Feb 2022 02:46:33 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:46:33 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:46:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:46:45 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:46:45 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl21.0.0.12920-1900
# Tue, 01 Feb 2022 02:46:45 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:46:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:46:46 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:46:46 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:46:47 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:46:52 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:46:52 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:46:52 GMT
USER 1001
# Tue, 01 Feb 2022 02:46:52 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:46:52 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:46:52 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 01 Feb 2022 02:47:06 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:47:06 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 01 Feb 2022 02:51:09 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 01 Feb 2022 02:51:16 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 01 Feb 2022 02:51:39 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:6d200361446626b53394c2a1a520a74a1221795562eac9b318c58e0abe147e23`  
		Last Modified: Fri, 07 Jan 2022 01:44:09 GMT  
		Size: 27.1 MB (27120999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2ea75c80fa68be6367734322b7c053932a41106663b880c832691c5c615f18`  
		Last Modified: Fri, 07 Jan 2022 02:32:46 GMT  
		Size: 15.7 MB (15739670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023197abac635771a2ec673c654381b9781d402f783200893ecc1cf31e3cbe62`  
		Last Modified: Tue, 01 Feb 2022 02:06:41 GMT  
		Size: 46.7 MB (46692338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943879201f267efb1789221ed57faefb9be861ea6702644113808ea5e86c79e4`  
		Last Modified: Tue, 01 Feb 2022 02:06:35 GMT  
		Size: 4.3 MB (4280295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ff29453f71380d2041f09c365f74be86b53e15d287c0fe7b9e7b7e2563abeb`  
		Last Modified: Tue, 01 Feb 2022 02:57:57 GMT  
		Size: 14.3 MB (14286325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ae1a4a83f1c75828585b6aea6d85065e2775f1c9c9b074116eadae8f29e240`  
		Last Modified: Tue, 01 Feb 2022 02:57:55 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0ba242f4dd0f8cce9d8605e50c3bd8f09f9a72586c113a60d7da49b212f4d8`  
		Last Modified: Tue, 01 Feb 2022 02:57:55 GMT  
		Size: 9.7 KB (9667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13cedf0d9418e3d2885b102954096e3c41c989c0ddad2972b7b01b444e30e510`  
		Last Modified: Tue, 01 Feb 2022 02:57:55 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0bb45bcf0e82ef2b0b1b86b4244e5ca1c9bed1248fe661f8086780286aa766`  
		Last Modified: Tue, 01 Feb 2022 02:57:55 GMT  
		Size: 10.6 KB (10635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218458e329b015285b27f7681ba15bc89a8fefb4090276d722ff3bacee95d688`  
		Last Modified: Tue, 01 Feb 2022 02:57:55 GMT  
		Size: 2.5 MB (2494410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554d837d11ffdec5e51bb42d0ff7b718e88e1772c7fbdf0c7d521c2a61b581de`  
		Last Modified: Tue, 01 Feb 2022 02:58:14 GMT  
		Size: 264.6 MB (264635065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea58517b4f6094fead31c02e695a3bf9758edae9b8d77078c2c48774e38e6d3b`  
		Last Modified: Tue, 01 Feb 2022 02:58:03 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2ac14432a1f4001b36d7464fc87c4d753ffa83a9a9d03f9e5689377e8998ff`  
		Last Modified: Tue, 01 Feb 2022 02:58:05 GMT  
		Size: 14.3 MB (14306865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.12-full-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:a3b8dd73f469146569a23c51ef3b7ad51be6c3b2db1c3d279544b37491e9f953
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
$ docker pull websphere-liberty@sha256:88d282937a8e1e636c123dd963b053fa086dc705758d204611817924df70b44f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **459.5 MB (459497437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c58183cb1c5fc280e52776fb8dda4e98cee7c4c8b13fe1ba52f088640d23dc8`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:19:52 GMT
ADD file:e29b7078eb9c78ec6f3931c4beea820e4b7fe5d0d02e02e220c083dcd603aad1 in / 
# Fri, 07 Jan 2022 02:19:55 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:28:44 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 03:29:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:17 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 03:30:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 03:30:11 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:14:00 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 07:14:02 GMT
ARG OPENJ9_SCC=true
# Fri, 07 Jan 2022 07:14:04 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Fri, 07 Jan 2022 07:14:05 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Fri, 07 Jan 2022 07:14:06 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Fri, 07 Jan 2022 07:14:08 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 07 Jan 2022 07:14:09 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Fri, 07 Jan 2022 07:14:10 GMT
ARG LIBERTY_URL
# Fri, 07 Jan 2022 07:14:12 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 07 Jan 2022 07:14:42 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 07:14:44 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Jan 2022 07:14:45 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl21.0.0.12920-1900
# Fri, 07 Jan 2022 07:14:46 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 07 Jan 2022 07:14:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 07 Jan 2022 07:14:56 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Fri, 07 Jan 2022 07:14:57 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 07 Jan 2022 07:15:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 07 Jan 2022 07:15:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 07 Jan 2022 07:15:22 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:15:24 GMT
USER 1001
# Fri, 07 Jan 2022 07:15:25 GMT
EXPOSE 9080 9443
# Fri, 07 Jan 2022 07:15:27 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 07 Jan 2022 07:15:28 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 07 Jan 2022 07:17:21 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 07:17:23 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 07 Jan 2022 07:22:26 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Fri, 07 Jan 2022 07:22:30 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 07 Jan 2022 07:23:26 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:f130035f6453da800db2a1c34f617d35285297b1e549cc5fe138db9ecb704f0b`  
		Last Modified: Fri, 07 Jan 2022 02:22:21 GMT  
		Size: 30.4 MB (30432347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89db02523773279c64e3768c4c557e84eb48533e8cd88fa8b305a4631fe1620f`  
		Last Modified: Fri, 07 Jan 2022 03:32:43 GMT  
		Size: 3.1 MB (3081902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8372d0c07db9ee4af75625eda00922334eb122c9730ed278ccf2668f02d09f82`  
		Last Modified: Fri, 07 Jan 2022 03:32:57 GMT  
		Size: 128.3 MB (128256173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3965b4317707127fee579fc3c78ea6257283c272b585bc31158d3901b4d1106e`  
		Last Modified: Fri, 07 Jan 2022 07:42:16 GMT  
		Size: 14.2 MB (14187495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fcabb9bc09f8dd92d5360fe84be98f2a1845cd593d9e71230db51c1b068449c`  
		Last Modified: Fri, 07 Jan 2022 07:42:11 GMT  
		Size: 697.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb350c3175bb6dd773fa8f97fec1c865ae4d5414812adf6cc2fcbb4065f4e52`  
		Last Modified: Fri, 07 Jan 2022 07:42:12 GMT  
		Size: 9.7 KB (9673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f096c91c30d59406ee0d9818b5958fe1bc83993daa9b0ad25221784dc94c437`  
		Last Modified: Fri, 07 Jan 2022 07:42:11 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c61c7363701b22ec57852b33130940163868e3c1581676c6f1e934d65fbbcd1`  
		Last Modified: Fri, 07 Jan 2022 07:42:11 GMT  
		Size: 10.7 KB (10655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c041f02818601344297d9538a27b695fe8d8819caa421b4eef28ed573a9cda90`  
		Last Modified: Fri, 07 Jan 2022 07:42:12 GMT  
		Size: 5.2 MB (5237132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3edf1df1f86a16ca81b0c2f29f6b3066094ab3ed435456316637818449599f8`  
		Last Modified: Fri, 07 Jan 2022 07:43:00 GMT  
		Size: 264.6 MB (264635010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d872f4baead4137a9cdc5a98adb3a49d43365aaa4363f7eb1957e37051fca4`  
		Last Modified: Fri, 07 Jan 2022 07:42:37 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50871aa31766644515d4039b3fd3c9b530ce8a4edfd72f67f813c2c052141c87`  
		Last Modified: Fri, 07 Jan 2022 07:42:40 GMT  
		Size: 13.6 MB (13645137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-full-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:d20aaa096c6f9609d3dd631345dc47b825239378b3b90056e8b4d136e3225e79
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **454.3 MB (454312581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d601ea4ccf2962c5ec3569bbcbfa5882878eda2dca13253a98fad2e7c7e056b`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 01:42:09 GMT
ADD file:caefb9be68fabe0b9b7dba683dabb869e5165a5a13534742d73a489a3712d9a9 in / 
# Fri, 07 Jan 2022 01:42:12 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:20:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 02:20:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:20:32 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 02:21:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 02:21:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 03:56:22 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 03:56:22 GMT
ARG OPENJ9_SCC=true
# Fri, 07 Jan 2022 03:56:22 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Fri, 07 Jan 2022 03:56:22 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Fri, 07 Jan 2022 03:56:23 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Fri, 07 Jan 2022 03:56:23 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 07 Jan 2022 03:56:23 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Fri, 07 Jan 2022 03:56:23 GMT
ARG LIBERTY_URL
# Fri, 07 Jan 2022 03:56:23 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 07 Jan 2022 03:56:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:56:35 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Jan 2022 03:56:35 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl21.0.0.12920-1900
# Fri, 07 Jan 2022 03:56:35 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 07 Jan 2022 03:56:36 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 07 Jan 2022 03:56:36 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Fri, 07 Jan 2022 03:56:36 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 07 Jan 2022 03:56:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 07 Jan 2022 03:56:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 07 Jan 2022 03:56:45 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Fri, 07 Jan 2022 03:56:45 GMT
USER 1001
# Fri, 07 Jan 2022 03:56:45 GMT
EXPOSE 9080 9443
# Fri, 07 Jan 2022 03:56:45 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 07 Jan 2022 03:56:45 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 07 Jan 2022 03:57:21 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 03:57:21 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 07 Jan 2022 04:01:42 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Fri, 07 Jan 2022 04:01:47 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 07 Jan 2022 04:02:13 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:7587f9252eef493a02840102ba78c74de317d3d47f6d568af5602ff6c1c54a20`  
		Last Modified: Fri, 07 Jan 2022 01:43:57 GMT  
		Size: 25.4 MB (25362136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d5d9207d0f328849a5bf2aec9290cf52dbfa8a48e3d39b130fd1471f46a16e`  
		Last Modified: Fri, 07 Jan 2022 02:23:17 GMT  
		Size: 2.7 MB (2676903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5948905ea3b7602d130be3b792486e9fa35aaf89ee11c6a87e63c7eabe5fdcf1`  
		Last Modified: Fri, 07 Jan 2022 02:23:25 GMT  
		Size: 125.7 MB (125737337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae092e18b98459590ea6caa33c2570c636487414ebcfdcebb4a46513631f7766`  
		Last Modified: Fri, 07 Jan 2022 04:17:26 GMT  
		Size: 14.2 MB (14187204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7bf3f3c0e6a13db68330bec3fb091f9eecba6afc134f1fc533846c98b743d5`  
		Last Modified: Fri, 07 Jan 2022 04:17:24 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b055004c04ef48f7b59b89674f36df7b49cdcffad86a6490fd2074a9d5f4b0`  
		Last Modified: Fri, 07 Jan 2022 04:17:24 GMT  
		Size: 9.7 KB (9672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1981c00f942abf2861c677139dd12a84d91550c8df20e1e59b8609df45397c69`  
		Last Modified: Fri, 07 Jan 2022 04:17:24 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ec547e5c6e7a71e2c357a00e308a5a34cff6babe1e18a39506d4d97c49e017`  
		Last Modified: Fri, 07 Jan 2022 04:17:24 GMT  
		Size: 10.6 KB (10649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ee0345d22ccb5c43a6eeaf1c067fe96b12f25eb8c2736e55b3d66720801dcc`  
		Last Modified: Fri, 07 Jan 2022 04:17:25 GMT  
		Size: 5.7 MB (5729255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da44655593882561c17397eb7d406697252dfa696217af012ca1e508ea8de9d`  
		Last Modified: Fri, 07 Jan 2022 04:17:50 GMT  
		Size: 264.6 MB (264635484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af85e983f89d0e8825926a219d497633b0f5fef9dfc8d1be9039118df877829`  
		Last Modified: Fri, 07 Jan 2022 04:17:38 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ff3bd90008fa43827de2252cef7b051a39fbb3e91e88159960eb5a62944c73`  
		Last Modified: Fri, 07 Jan 2022 04:17:40 GMT  
		Size: 16.0 MB (15962027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.12-kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:600668fd307c8724f7d87dce8cdeafa1c5b78f388d476feae41745d9eec27ff6
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
$ docker pull websphere-liberty@sha256:4b2a87e3f30d8acf7908721982c96daf7038d56c9a8682e8248c9fc882b1d218
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118964601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8e13c21dfa76824d68da11e1eff16f9458dc73a128736fcf7b686effec3262a`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:20:15 GMT
ADD file:014236839eaee978894ae0bd6aecc246177a0a2c11af73f86d9cfafe5478ce18 in / 
# Fri, 07 Jan 2022 02:20:19 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:29 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:22:19 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:23:02 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 01:26:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:26:46 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:26:48 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:27:31 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:37:48 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:37:49 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:45:16 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Tue, 01 Feb 2022 02:45:18 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Tue, 01 Feb 2022 02:45:20 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Tue, 01 Feb 2022 02:45:22 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:45:24 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Tue, 01 Feb 2022 02:45:25 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:45:28 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:45:50 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:45:56 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:45:58 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl21.0.0.12920-1900
# Tue, 01 Feb 2022 02:46:00 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:46:05 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:46:05 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:46:06 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:46:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:46:26 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:46:30 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:46:32 GMT
USER 1001
# Tue, 01 Feb 2022 02:46:34 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:46:37 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:46:39 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e6e6dea5a8cc4bdc9e5e51e2bfa948159b69d5fbc2dca99bc41776fb04dab967`  
		Last Modified: Fri, 07 Jan 2022 02:22:43 GMT  
		Size: 33.3 MB (33286892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2db03674d664c4c13747eecf6ee9d3578adc9eb95e5a3993661ba5f37f676f8`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 17.2 MB (17206916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0441717da968406ddb594da0c1ad05e5f42434a3584422d7fab7e64763e30b4`  
		Last Modified: Tue, 01 Feb 2022 01:39:44 GMT  
		Size: 48.4 MB (48356102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6fe9db05a97733f7b24220942aef850723e6992236fcba495134a2fc03a312b`  
		Last Modified: Tue, 01 Feb 2022 01:39:36 GMT  
		Size: 3.3 MB (3331743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd951b2f63ad5c87a257c00ace1b87917a17bc55f2d7f51cf49e4f03e723aa1e`  
		Last Modified: Tue, 01 Feb 2022 03:00:16 GMT  
		Size: 14.3 MB (14286603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2467ca4cde039e05b93a30920246f8c81f15fed4abc15d6bc8445b4e65f8d0`  
		Last Modified: Tue, 01 Feb 2022 03:00:12 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e827664c35967cbc0924137b4b51288f2080d8773dbd9371d0f0f579b0903e`  
		Last Modified: Tue, 01 Feb 2022 03:00:12 GMT  
		Size: 9.7 KB (9668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca060c94cc295078bd7c8dd0290c0675ece69e8ac9dc69a0a4de2b5774f4d02`  
		Last Modified: Tue, 01 Feb 2022 03:00:12 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77553ab561424ad8114dfcd67bf39142266456ff0d7e784d5d325d22eed2feb5`  
		Last Modified: Tue, 01 Feb 2022 03:00:12 GMT  
		Size: 10.7 KB (10658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f145a66885ecddb48e51e2edb9f025b46027536c746bc236af5527961b4e7d`  
		Last Modified: Tue, 01 Feb 2022 03:00:12 GMT  
		Size: 2.5 MB (2475054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:829fff2b25ac922119c6b84b57a968a89ac50a0005fd86d5408b4ade2e86b21d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110635298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b813ef4ed3e7c0cbd881a5985eb4241d561b30eb1d31f5aafd04762a2bfedf4`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 01:42:20 GMT
ADD file:b6119f4fcd6a113749f515278b315ffd96aecce7006f086acb060f981e5c59db in / 
# Fri, 07 Jan 2022 01:42:22 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:15:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 02:24:31 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:00:54 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 02:01:59 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 02:02:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:02:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 02:02:34 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:40:32 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:40:32 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:46:33 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Tue, 01 Feb 2022 02:46:33 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Tue, 01 Feb 2022 02:46:33 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Tue, 01 Feb 2022 02:46:33 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:46:33 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Tue, 01 Feb 2022 02:46:33 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:46:33 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:46:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:46:45 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:46:45 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl21.0.0.12920-1900
# Tue, 01 Feb 2022 02:46:45 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:46:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:46:46 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:46:46 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:46:47 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:46:52 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:46:52 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:46:52 GMT
USER 1001
# Tue, 01 Feb 2022 02:46:52 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:46:52 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:46:52 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6d200361446626b53394c2a1a520a74a1221795562eac9b318c58e0abe147e23`  
		Last Modified: Fri, 07 Jan 2022 01:44:09 GMT  
		Size: 27.1 MB (27120999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2ea75c80fa68be6367734322b7c053932a41106663b880c832691c5c615f18`  
		Last Modified: Fri, 07 Jan 2022 02:32:46 GMT  
		Size: 15.7 MB (15739670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023197abac635771a2ec673c654381b9781d402f783200893ecc1cf31e3cbe62`  
		Last Modified: Tue, 01 Feb 2022 02:06:41 GMT  
		Size: 46.7 MB (46692338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943879201f267efb1789221ed57faefb9be861ea6702644113808ea5e86c79e4`  
		Last Modified: Tue, 01 Feb 2022 02:06:35 GMT  
		Size: 4.3 MB (4280295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ff29453f71380d2041f09c365f74be86b53e15d287c0fe7b9e7b7e2563abeb`  
		Last Modified: Tue, 01 Feb 2022 02:57:57 GMT  
		Size: 14.3 MB (14286325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ae1a4a83f1c75828585b6aea6d85065e2775f1c9c9b074116eadae8f29e240`  
		Last Modified: Tue, 01 Feb 2022 02:57:55 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0ba242f4dd0f8cce9d8605e50c3bd8f09f9a72586c113a60d7da49b212f4d8`  
		Last Modified: Tue, 01 Feb 2022 02:57:55 GMT  
		Size: 9.7 KB (9667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13cedf0d9418e3d2885b102954096e3c41c989c0ddad2972b7b01b444e30e510`  
		Last Modified: Tue, 01 Feb 2022 02:57:55 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0bb45bcf0e82ef2b0b1b86b4244e5ca1c9bed1248fe661f8086780286aa766`  
		Last Modified: Tue, 01 Feb 2022 02:57:55 GMT  
		Size: 10.6 KB (10635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218458e329b015285b27f7681ba15bc89a8fefb4090276d722ff3bacee95d688`  
		Last Modified: Tue, 01 Feb 2022 02:57:55 GMT  
		Size: 2.5 MB (2494410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.12-kernel-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:703bc6ed7ff4c35987104c8c15b839e3ca5102d0dd961a4f38d0364fe14f444a
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
$ docker pull websphere-liberty@sha256:b3ee81bc59f8ad72734d076a1e711c4a98cc61c6ac3858eff9afcde13db7b8ef
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.2 MB (181216346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9422d212ecdb01bdf7497224332defd1ac0f33d65d5461eb7d4e4f34dcddfb1`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:19:52 GMT
ADD file:e29b7078eb9c78ec6f3931c4beea820e4b7fe5d0d02e02e220c083dcd603aad1 in / 
# Fri, 07 Jan 2022 02:19:55 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:28:44 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 03:29:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:17 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 03:30:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 03:30:11 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:14:00 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 07:14:02 GMT
ARG OPENJ9_SCC=true
# Fri, 07 Jan 2022 07:14:04 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Fri, 07 Jan 2022 07:14:05 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Fri, 07 Jan 2022 07:14:06 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Fri, 07 Jan 2022 07:14:08 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 07 Jan 2022 07:14:09 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Fri, 07 Jan 2022 07:14:10 GMT
ARG LIBERTY_URL
# Fri, 07 Jan 2022 07:14:12 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 07 Jan 2022 07:14:42 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 07:14:44 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Jan 2022 07:14:45 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl21.0.0.12920-1900
# Fri, 07 Jan 2022 07:14:46 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 07 Jan 2022 07:14:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 07 Jan 2022 07:14:56 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Fri, 07 Jan 2022 07:14:57 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 07 Jan 2022 07:15:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 07 Jan 2022 07:15:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 07 Jan 2022 07:15:22 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:15:24 GMT
USER 1001
# Fri, 07 Jan 2022 07:15:25 GMT
EXPOSE 9080 9443
# Fri, 07 Jan 2022 07:15:27 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 07 Jan 2022 07:15:28 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:f130035f6453da800db2a1c34f617d35285297b1e549cc5fe138db9ecb704f0b`  
		Last Modified: Fri, 07 Jan 2022 02:22:21 GMT  
		Size: 30.4 MB (30432347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89db02523773279c64e3768c4c557e84eb48533e8cd88fa8b305a4631fe1620f`  
		Last Modified: Fri, 07 Jan 2022 03:32:43 GMT  
		Size: 3.1 MB (3081902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8372d0c07db9ee4af75625eda00922334eb122c9730ed278ccf2668f02d09f82`  
		Last Modified: Fri, 07 Jan 2022 03:32:57 GMT  
		Size: 128.3 MB (128256173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3965b4317707127fee579fc3c78ea6257283c272b585bc31158d3901b4d1106e`  
		Last Modified: Fri, 07 Jan 2022 07:42:16 GMT  
		Size: 14.2 MB (14187495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fcabb9bc09f8dd92d5360fe84be98f2a1845cd593d9e71230db51c1b068449c`  
		Last Modified: Fri, 07 Jan 2022 07:42:11 GMT  
		Size: 697.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb350c3175bb6dd773fa8f97fec1c865ae4d5414812adf6cc2fcbb4065f4e52`  
		Last Modified: Fri, 07 Jan 2022 07:42:12 GMT  
		Size: 9.7 KB (9673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f096c91c30d59406ee0d9818b5958fe1bc83993daa9b0ad25221784dc94c437`  
		Last Modified: Fri, 07 Jan 2022 07:42:11 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c61c7363701b22ec57852b33130940163868e3c1581676c6f1e934d65fbbcd1`  
		Last Modified: Fri, 07 Jan 2022 07:42:11 GMT  
		Size: 10.7 KB (10655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c041f02818601344297d9538a27b695fe8d8819caa421b4eef28ed573a9cda90`  
		Last Modified: Fri, 07 Jan 2022 07:42:12 GMT  
		Size: 5.2 MB (5237132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-kernel-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:e032ea1e3d24b6bd1b4ff23035ecc8eac744a198071b629c14f291e1f765f763
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.7 MB (173714125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e48508ecb2ff9fd382a0b5a64786154990805779c3e299e885c13035ebe874ea`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 01:42:09 GMT
ADD file:caefb9be68fabe0b9b7dba683dabb869e5165a5a13534742d73a489a3712d9a9 in / 
# Fri, 07 Jan 2022 01:42:12 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:20:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 02:20:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:20:32 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 02:21:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 02:21:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 03:56:22 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 03:56:22 GMT
ARG OPENJ9_SCC=true
# Fri, 07 Jan 2022 03:56:22 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Fri, 07 Jan 2022 03:56:22 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Fri, 07 Jan 2022 03:56:23 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Fri, 07 Jan 2022 03:56:23 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl21.0.0.12920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 07 Jan 2022 03:56:23 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Fri, 07 Jan 2022 03:56:23 GMT
ARG LIBERTY_URL
# Fri, 07 Jan 2022 03:56:23 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 07 Jan 2022 03:56:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:56:35 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Jan 2022 03:56:35 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl21.0.0.12920-1900
# Fri, 07 Jan 2022 03:56:35 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 07 Jan 2022 03:56:36 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 07 Jan 2022 03:56:36 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Fri, 07 Jan 2022 03:56:36 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 07 Jan 2022 03:56:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 07 Jan 2022 03:56:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 07 Jan 2022 03:56:45 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Fri, 07 Jan 2022 03:56:45 GMT
USER 1001
# Fri, 07 Jan 2022 03:56:45 GMT
EXPOSE 9080 9443
# Fri, 07 Jan 2022 03:56:45 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 07 Jan 2022 03:56:45 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:7587f9252eef493a02840102ba78c74de317d3d47f6d568af5602ff6c1c54a20`  
		Last Modified: Fri, 07 Jan 2022 01:43:57 GMT  
		Size: 25.4 MB (25362136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d5d9207d0f328849a5bf2aec9290cf52dbfa8a48e3d39b130fd1471f46a16e`  
		Last Modified: Fri, 07 Jan 2022 02:23:17 GMT  
		Size: 2.7 MB (2676903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5948905ea3b7602d130be3b792486e9fa35aaf89ee11c6a87e63c7eabe5fdcf1`  
		Last Modified: Fri, 07 Jan 2022 02:23:25 GMT  
		Size: 125.7 MB (125737337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae092e18b98459590ea6caa33c2570c636487414ebcfdcebb4a46513631f7766`  
		Last Modified: Fri, 07 Jan 2022 04:17:26 GMT  
		Size: 14.2 MB (14187204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7bf3f3c0e6a13db68330bec3fb091f9eecba6afc134f1fc533846c98b743d5`  
		Last Modified: Fri, 07 Jan 2022 04:17:24 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b055004c04ef48f7b59b89674f36df7b49cdcffad86a6490fd2074a9d5f4b0`  
		Last Modified: Fri, 07 Jan 2022 04:17:24 GMT  
		Size: 9.7 KB (9672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1981c00f942abf2861c677139dd12a84d91550c8df20e1e59b8609df45397c69`  
		Last Modified: Fri, 07 Jan 2022 04:17:24 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ec547e5c6e7a71e2c357a00e308a5a34cff6babe1e18a39506d4d97c49e017`  
		Last Modified: Fri, 07 Jan 2022 04:17:24 GMT  
		Size: 10.6 KB (10649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ee0345d22ccb5c43a6eeaf1c067fe96b12f25eb8c2736e55b3d66720801dcc`  
		Last Modified: Fri, 07 Jan 2022 04:17:25 GMT  
		Size: 5.7 MB (5729255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.9-full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:cecaffe72e58ac67aab2db15365718a56ce0ed34bf1acb2ae5ce3dbd37e762ed
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
$ docker pull websphere-liberty@sha256:250c23ef97fe0fc79ab6b023a8794fdef5632874236494742d5e305b35afe5a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.5 MB (340535369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d087437630fe9dc7adc608a99b43741abd0869713c8d7a5d3f0adc529495adfb`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:20:15 GMT
ADD file:014236839eaee978894ae0bd6aecc246177a0a2c11af73f86d9cfafe5478ce18 in / 
# Fri, 07 Jan 2022 02:20:19 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:29 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:22:19 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:23:02 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 01:26:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:26:46 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:26:48 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:27:31 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:37:48 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:37:49 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:52:30 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Tue, 01 Feb 2022 02:52:33 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Tue, 01 Feb 2022 02:52:35 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Tue, 01 Feb 2022 02:52:37 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:52:39 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Tue, 01 Feb 2022 02:52:40 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:52:42 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:53:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:53:14 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:53:17 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Tue, 01 Feb 2022 02:53:20 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:53:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:53:27 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:53:29 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:53:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:53:49 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:53:51 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:53:53 GMT
USER 1001
# Tue, 01 Feb 2022 02:53:54 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:53:56 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:53:58 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 01 Feb 2022 02:54:13 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:54:14 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 01 Feb 2022 02:57:30 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 01 Feb 2022 02:57:37 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 01 Feb 2022 02:58:31 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:e6e6dea5a8cc4bdc9e5e51e2bfa948159b69d5fbc2dca99bc41776fb04dab967`  
		Last Modified: Fri, 07 Jan 2022 02:22:43 GMT  
		Size: 33.3 MB (33286892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2db03674d664c4c13747eecf6ee9d3578adc9eb95e5a3993661ba5f37f676f8`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 17.2 MB (17206916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0441717da968406ddb594da0c1ad05e5f42434a3584422d7fab7e64763e30b4`  
		Last Modified: Tue, 01 Feb 2022 01:39:44 GMT  
		Size: 48.4 MB (48356102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6fe9db05a97733f7b24220942aef850723e6992236fcba495134a2fc03a312b`  
		Last Modified: Tue, 01 Feb 2022 01:39:36 GMT  
		Size: 3.3 MB (3331743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27512861ea07d7a823d38571c11263552e8fe68ef2eb9195dea54f303814e9bc`  
		Last Modified: Tue, 01 Feb 2022 03:01:07 GMT  
		Size: 14.2 MB (14154688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed9d2778d729d40d1dc00d2caef2831f65d9fd10d9cc5b244446730d0ab09f8`  
		Last Modified: Tue, 01 Feb 2022 03:01:03 GMT  
		Size: 697.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd89ef09798fca7b80b2ac6ec2fb8ca2f39967958d50b7903d6af47587e88a8`  
		Last Modified: Tue, 01 Feb 2022 03:01:03 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0860d810bf3b2748c86f695c1752f6c56598cad69b89ea942a2b45a6904bc55f`  
		Last Modified: Tue, 01 Feb 2022 03:01:03 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b3152f07aaab75fb38930d0baf0000d5ce1f5b6d16c29c39ffad43e6175e0e`  
		Last Modified: Tue, 01 Feb 2022 03:01:03 GMT  
		Size: 10.7 KB (10654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85d9cd22b9a9f829de9e1139868c4ff0ffc2a6cacb15d17cfc7ffdf16eaa717`  
		Last Modified: Tue, 01 Feb 2022 03:01:03 GMT  
		Size: 2.5 MB (2478289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ea8f589a6b66c49c52b31d79eff890859810a528dd6ba02a339cef05ff141b`  
		Last Modified: Tue, 01 Feb 2022 03:01:35 GMT  
		Size: 209.2 MB (209236788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4401b05b4c82e14a07d4abf5a5fa78bc140d78c00f4c02b11fac04b5cd0d449c`  
		Last Modified: Tue, 01 Feb 2022 03:01:16 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515ea747462f7c4683f711c3ffeafef1a9ca763c5e4b246258f1e09e62cd0245`  
		Last Modified: Tue, 01 Feb 2022 03:01:19 GMT  
		Size: 12.5 MB (12461717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.9-full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:0d418c029f4eb09c926c910b0156f357b11bbd76c30ee3cac4634f82460967d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.0 MB (334013011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:016aa65c281d7a77610b0f5c48e6688af9a3154fbbbb41389ed4eae717e3d73b`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 01:42:20 GMT
ADD file:b6119f4fcd6a113749f515278b315ffd96aecce7006f086acb060f981e5c59db in / 
# Fri, 07 Jan 2022 01:42:22 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:15:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 02:24:31 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:00:54 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 02:01:59 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 02:02:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:02:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 02:02:34 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:40:32 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:40:32 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:52:04 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Tue, 01 Feb 2022 02:52:04 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Tue, 01 Feb 2022 02:52:04 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Tue, 01 Feb 2022 02:52:04 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:52:04 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Tue, 01 Feb 2022 02:52:04 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:52:04 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:52:15 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:52:15 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:52:16 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Tue, 01 Feb 2022 02:52:16 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:52:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:52:17 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:52:17 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:52:17 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:52:22 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:52:23 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:52:23 GMT
USER 1001
# Tue, 01 Feb 2022 02:52:23 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:52:23 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:52:24 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 01 Feb 2022 02:52:36 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:52:36 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 01 Feb 2022 02:55:56 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 01 Feb 2022 02:56:00 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 01 Feb 2022 02:56:23 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:6d200361446626b53394c2a1a520a74a1221795562eac9b318c58e0abe147e23`  
		Last Modified: Fri, 07 Jan 2022 01:44:09 GMT  
		Size: 27.1 MB (27120999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2ea75c80fa68be6367734322b7c053932a41106663b880c832691c5c615f18`  
		Last Modified: Fri, 07 Jan 2022 02:32:46 GMT  
		Size: 15.7 MB (15739670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023197abac635771a2ec673c654381b9781d402f783200893ecc1cf31e3cbe62`  
		Last Modified: Tue, 01 Feb 2022 02:06:41 GMT  
		Size: 46.7 MB (46692338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943879201f267efb1789221ed57faefb9be861ea6702644113808ea5e86c79e4`  
		Last Modified: Tue, 01 Feb 2022 02:06:35 GMT  
		Size: 4.3 MB (4280295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74165ab99ac4e51c2285e6c76e672bd94982fee8b888f47fa284fbabc5e4ac5`  
		Last Modified: Tue, 01 Feb 2022 02:58:23 GMT  
		Size: 14.2 MB (14154361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75138334d060974070f04ce4d4fdb234c8fb2bf5b4dcd46d1b4f285c02caf8d`  
		Last Modified: Tue, 01 Feb 2022 02:58:21 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a33de44a7ba7f7061048c611511d52165d2dbbca07cfc0e6e483d4795cecd9`  
		Last Modified: Tue, 01 Feb 2022 02:58:21 GMT  
		Size: 9.7 KB (9671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c97e7cc1960856e15e5f675f68ab9e94c502022d0d90c3e5dfe2f10ca45c70f`  
		Last Modified: Tue, 01 Feb 2022 02:58:21 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761dbac0e43bea2095f68f7b87acd9008bfa394ee60c68711314e1014451572e`  
		Last Modified: Tue, 01 Feb 2022 02:58:21 GMT  
		Size: 10.7 KB (10653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b387ca1d420aba563a46bcae2ce4448fab30212c3426a6d77204cc3de9e516`  
		Last Modified: Tue, 01 Feb 2022 02:58:21 GMT  
		Size: 2.5 MB (2505823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a380512cd2f9f8cadf2bde34beddaeb0a66ee1fdfa785426d8ec3afe5d3cf8`  
		Last Modified: Tue, 01 Feb 2022 02:58:38 GMT  
		Size: 209.2 MB (209237197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d950a9eef198857bd8da644326c964016c491949abc07b237823f060e784a885`  
		Last Modified: Tue, 01 Feb 2022 02:58:29 GMT  
		Size: 941.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbcdb34cf9f655402f94ceefa29d1843569d21bfb9a92bc9a78a72cf6379b7e4`  
		Last Modified: Tue, 01 Feb 2022 02:58:31 GMT  
		Size: 14.3 MB (14260101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.9-full-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:a530ff2913650dffd9d9c76fc0369d7cd13607aa58ad34f938e7d9a63f593ea0
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
$ docker pull websphere-liberty@sha256:6c821c4d9946936d0cedfab472d412a80732fe2fe492cb414c02dd57e35385a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.0 MB (404010318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc9238a2e509475114c5f7e94d6e275aab025f4e3b243e8018750c6fb21f2723`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:19:52 GMT
ADD file:e29b7078eb9c78ec6f3931c4beea820e4b7fe5d0d02e02e220c083dcd603aad1 in / 
# Fri, 07 Jan 2022 02:19:55 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:28:44 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 03:29:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:17 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 03:30:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 03:30:11 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:14:00 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 07:14:02 GMT
ARG OPENJ9_SCC=true
# Fri, 07 Jan 2022 07:29:16 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Fri, 07 Jan 2022 07:29:18 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Fri, 07 Jan 2022 07:29:19 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Fri, 07 Jan 2022 07:29:21 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 07 Jan 2022 07:29:22 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Fri, 07 Jan 2022 07:29:23 GMT
ARG LIBERTY_URL
# Fri, 07 Jan 2022 07:29:25 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 07 Jan 2022 07:29:50 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 07:29:52 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Jan 2022 07:29:57 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Fri, 07 Jan 2022 07:29:59 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 07 Jan 2022 07:30:06 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 07 Jan 2022 07:30:08 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Fri, 07 Jan 2022 07:30:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 07 Jan 2022 07:30:15 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 07 Jan 2022 07:30:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 07 Jan 2022 07:30:34 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:30:37 GMT
USER 1001
# Fri, 07 Jan 2022 07:30:38 GMT
EXPOSE 9080 9443
# Fri, 07 Jan 2022 07:30:41 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 07 Jan 2022 07:30:43 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 07 Jan 2022 07:32:22 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 07:32:23 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 07 Jan 2022 07:35:46 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Fri, 07 Jan 2022 07:35:56 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 07 Jan 2022 07:36:51 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:f130035f6453da800db2a1c34f617d35285297b1e549cc5fe138db9ecb704f0b`  
		Last Modified: Fri, 07 Jan 2022 02:22:21 GMT  
		Size: 30.4 MB (30432347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89db02523773279c64e3768c4c557e84eb48533e8cd88fa8b305a4631fe1620f`  
		Last Modified: Fri, 07 Jan 2022 03:32:43 GMT  
		Size: 3.1 MB (3081902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8372d0c07db9ee4af75625eda00922334eb122c9730ed278ccf2668f02d09f82`  
		Last Modified: Fri, 07 Jan 2022 03:32:57 GMT  
		Size: 128.3 MB (128256173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61a14b96da178ddf73423a23596f9c7b27d5086e505ba08273ed387a206bd69`  
		Last Modified: Fri, 07 Jan 2022 07:44:04 GMT  
		Size: 14.1 MB (14056076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a713b83c15fac82c88e50022a6a72e738ec96b4c033038a0f5ac475d287b107`  
		Last Modified: Fri, 07 Jan 2022 07:44:00 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ccedb4c7b0e2134ae863fda35e2e18e7c5bcc427262b49f3f5c433482aefe5`  
		Last Modified: Fri, 07 Jan 2022 07:44:00 GMT  
		Size: 9.7 KB (9672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe72711c0af548e44f1ea9ae5b91355fc1b970b3337afff4283e2e3fc00b105e`  
		Last Modified: Fri, 07 Jan 2022 07:44:00 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2f7614810e4d9b9bcf3b4c65a3faa4619e64151bb38e816b58356839c415a1`  
		Last Modified: Fri, 07 Jan 2022 07:44:00 GMT  
		Size: 10.7 KB (10658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd055f925c19743f7a818085e6fbfe17d4486808538f1b377fe444916f339e51`  
		Last Modified: Fri, 07 Jan 2022 07:44:01 GMT  
		Size: 5.3 MB (5252005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a0f674baaf1b98b2935a5d733c2b324a822342e97aba2682fae4597f77166c`  
		Last Modified: Fri, 07 Jan 2022 07:44:45 GMT  
		Size: 209.2 MB (209236573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879a21aa166cabb0d18c5fd7f83d4f56deb3ed2fce82270e3ebeb957c2832b19`  
		Last Modified: Fri, 07 Jan 2022 07:44:25 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc81757a0d3c144c866c2198478074db6631938f2f9de98aadb0f8e755088c65`  
		Last Modified: Fri, 07 Jan 2022 07:44:28 GMT  
		Size: 13.7 MB (13672998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.9-full-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:4d6a71af71c00ca6c9b3a8a7d9fa67bac15180f3ee5f10c12b3b3a60e17ee2f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.7 MB (398659110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b290bb32601ab76ea419d771cea0657aadcd705636279e6d16b49ebc1498013e`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 01:42:09 GMT
ADD file:caefb9be68fabe0b9b7dba683dabb869e5165a5a13534742d73a489a3712d9a9 in / 
# Fri, 07 Jan 2022 01:42:12 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:20:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 02:20:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:20:32 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 02:21:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 02:21:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 03:56:22 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 03:56:22 GMT
ARG OPENJ9_SCC=true
# Fri, 07 Jan 2022 04:07:43 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Fri, 07 Jan 2022 04:07:43 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Fri, 07 Jan 2022 04:07:43 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Fri, 07 Jan 2022 04:07:43 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 07 Jan 2022 04:07:43 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Fri, 07 Jan 2022 04:07:44 GMT
ARG LIBERTY_URL
# Fri, 07 Jan 2022 04:07:44 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 07 Jan 2022 04:07:55 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:07:55 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Jan 2022 04:07:55 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Fri, 07 Jan 2022 04:07:56 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 07 Jan 2022 04:07:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 07 Jan 2022 04:07:57 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Fri, 07 Jan 2022 04:07:57 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 07 Jan 2022 04:07:57 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 07 Jan 2022 04:08:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 07 Jan 2022 04:08:05 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Fri, 07 Jan 2022 04:08:05 GMT
USER 1001
# Fri, 07 Jan 2022 04:08:05 GMT
EXPOSE 9080 9443
# Fri, 07 Jan 2022 04:08:05 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 07 Jan 2022 04:08:05 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 07 Jan 2022 04:08:38 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 04:08:38 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 07 Jan 2022 04:12:05 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Fri, 07 Jan 2022 04:12:09 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 07 Jan 2022 04:12:34 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:7587f9252eef493a02840102ba78c74de317d3d47f6d568af5602ff6c1c54a20`  
		Last Modified: Fri, 07 Jan 2022 01:43:57 GMT  
		Size: 25.4 MB (25362136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d5d9207d0f328849a5bf2aec9290cf52dbfa8a48e3d39b130fd1471f46a16e`  
		Last Modified: Fri, 07 Jan 2022 02:23:17 GMT  
		Size: 2.7 MB (2676903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5948905ea3b7602d130be3b792486e9fa35aaf89ee11c6a87e63c7eabe5fdcf1`  
		Last Modified: Fri, 07 Jan 2022 02:23:25 GMT  
		Size: 125.7 MB (125737337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7267f5b5b89b76bc8c416d555e78011782fd85ad9a3fa2583b37d1b05aa6a0`  
		Last Modified: Fri, 07 Jan 2022 04:18:29 GMT  
		Size: 14.1 MB (14055692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc555cee5444c7e947070324a54b9ca25c75e443fbec66a62b35f727e40e30`  
		Last Modified: Fri, 07 Jan 2022 04:18:27 GMT  
		Size: 690.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5a8cca353c09c64957412bdf9d39bcc70a88d19de8763bf23cb63af0934e59`  
		Last Modified: Fri, 07 Jan 2022 04:18:27 GMT  
		Size: 9.7 KB (9675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebf853da83cca1c3a2656f8ab425ed0a75055e3819c7f93589c0376ee917036`  
		Last Modified: Fri, 07 Jan 2022 04:18:27 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822e8278506e653c77210970e14c7bacdb64f173c6c6da1279cee3fc8ae8d1d8`  
		Last Modified: Fri, 07 Jan 2022 04:18:27 GMT  
		Size: 10.6 KB (10644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcf6ac67b863a33e39e1aff68c25bb6577b51c851f7259b57d50877b3c7d10f`  
		Last Modified: Fri, 07 Jan 2022 04:18:27 GMT  
		Size: 5.7 MB (5739351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856468c73e5dbf6278cb5e06fe9b130d37cb5f5bc21b0a0329761528a9792bf3`  
		Last Modified: Fri, 07 Jan 2022 04:18:49 GMT  
		Size: 209.2 MB (209237758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae19cd764f5ce36017b6ca7ed7c6583e3ed5453bd3ffdbb40fffe6a438a29d52`  
		Last Modified: Fri, 07 Jan 2022 04:18:40 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a938f6045b9aa4eed70926e0002eadac87278aba80ed8065821e31392423f2e`  
		Last Modified: Fri, 07 Jan 2022 04:18:42 GMT  
		Size: 15.8 MB (15827707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.9-kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:15e51102aed103c74787cfd5c8d7d0fadba72f0b475284edd46ff3e708b14fa7
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
$ docker pull websphere-liberty@sha256:0fec8e430d0df6d2b4bdb7dc2a23d3a500ca0b04c54647d33a5266b2200fbdf8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118835921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:375ff3902485d35475e1035450a0aa7cc888246b9d89ce6a13d4b094eefae5c4`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:20:15 GMT
ADD file:014236839eaee978894ae0bd6aecc246177a0a2c11af73f86d9cfafe5478ce18 in / 
# Fri, 07 Jan 2022 02:20:19 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:29 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:22:19 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:23:02 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 01:26:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:26:46 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:26:48 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:27:31 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:37:48 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:37:49 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:52:30 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Tue, 01 Feb 2022 02:52:33 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Tue, 01 Feb 2022 02:52:35 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Tue, 01 Feb 2022 02:52:37 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:52:39 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Tue, 01 Feb 2022 02:52:40 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:52:42 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:53:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:53:14 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:53:17 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Tue, 01 Feb 2022 02:53:20 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:53:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:53:27 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:53:29 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:53:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:53:49 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:53:51 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:53:53 GMT
USER 1001
# Tue, 01 Feb 2022 02:53:54 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:53:56 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:53:58 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e6e6dea5a8cc4bdc9e5e51e2bfa948159b69d5fbc2dca99bc41776fb04dab967`  
		Last Modified: Fri, 07 Jan 2022 02:22:43 GMT  
		Size: 33.3 MB (33286892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2db03674d664c4c13747eecf6ee9d3578adc9eb95e5a3993661ba5f37f676f8`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 17.2 MB (17206916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0441717da968406ddb594da0c1ad05e5f42434a3584422d7fab7e64763e30b4`  
		Last Modified: Tue, 01 Feb 2022 01:39:44 GMT  
		Size: 48.4 MB (48356102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6fe9db05a97733f7b24220942aef850723e6992236fcba495134a2fc03a312b`  
		Last Modified: Tue, 01 Feb 2022 01:39:36 GMT  
		Size: 3.3 MB (3331743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27512861ea07d7a823d38571c11263552e8fe68ef2eb9195dea54f303814e9bc`  
		Last Modified: Tue, 01 Feb 2022 03:01:07 GMT  
		Size: 14.2 MB (14154688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed9d2778d729d40d1dc00d2caef2831f65d9fd10d9cc5b244446730d0ab09f8`  
		Last Modified: Tue, 01 Feb 2022 03:01:03 GMT  
		Size: 697.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd89ef09798fca7b80b2ac6ec2fb8ca2f39967958d50b7903d6af47587e88a8`  
		Last Modified: Tue, 01 Feb 2022 03:01:03 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0860d810bf3b2748c86f695c1752f6c56598cad69b89ea942a2b45a6904bc55f`  
		Last Modified: Tue, 01 Feb 2022 03:01:03 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b3152f07aaab75fb38930d0baf0000d5ce1f5b6d16c29c39ffad43e6175e0e`  
		Last Modified: Tue, 01 Feb 2022 03:01:03 GMT  
		Size: 10.7 KB (10654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85d9cd22b9a9f829de9e1139868c4ff0ffc2a6cacb15d17cfc7ffdf16eaa717`  
		Last Modified: Tue, 01 Feb 2022 03:01:03 GMT  
		Size: 2.5 MB (2478289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.9-kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:d2f773d61f597af572c3352baf86841035b13ee4040bb3140704b62664ef044b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110514772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0be74411015f1fc89868dff9d570b9332921e0bdc8373ee408ed835063fe7d96`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 01:42:20 GMT
ADD file:b6119f4fcd6a113749f515278b315ffd96aecce7006f086acb060f981e5c59db in / 
# Fri, 07 Jan 2022 01:42:22 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:15:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 02:24:31 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:00:54 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 02:01:59 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 02:02:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:02:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 02:02:34 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:40:32 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:40:32 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:52:04 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Tue, 01 Feb 2022 02:52:04 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Tue, 01 Feb 2022 02:52:04 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Tue, 01 Feb 2022 02:52:04 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:52:04 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Tue, 01 Feb 2022 02:52:04 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:52:04 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:52:15 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:52:15 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:52:16 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Tue, 01 Feb 2022 02:52:16 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:52:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:52:17 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:52:17 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:52:17 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:52:22 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:52:23 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:52:23 GMT
USER 1001
# Tue, 01 Feb 2022 02:52:23 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:52:23 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:52:24 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6d200361446626b53394c2a1a520a74a1221795562eac9b318c58e0abe147e23`  
		Last Modified: Fri, 07 Jan 2022 01:44:09 GMT  
		Size: 27.1 MB (27120999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2ea75c80fa68be6367734322b7c053932a41106663b880c832691c5c615f18`  
		Last Modified: Fri, 07 Jan 2022 02:32:46 GMT  
		Size: 15.7 MB (15739670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023197abac635771a2ec673c654381b9781d402f783200893ecc1cf31e3cbe62`  
		Last Modified: Tue, 01 Feb 2022 02:06:41 GMT  
		Size: 46.7 MB (46692338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943879201f267efb1789221ed57faefb9be861ea6702644113808ea5e86c79e4`  
		Last Modified: Tue, 01 Feb 2022 02:06:35 GMT  
		Size: 4.3 MB (4280295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74165ab99ac4e51c2285e6c76e672bd94982fee8b888f47fa284fbabc5e4ac5`  
		Last Modified: Tue, 01 Feb 2022 02:58:23 GMT  
		Size: 14.2 MB (14154361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75138334d060974070f04ce4d4fdb234c8fb2bf5b4dcd46d1b4f285c02caf8d`  
		Last Modified: Tue, 01 Feb 2022 02:58:21 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a33de44a7ba7f7061048c611511d52165d2dbbca07cfc0e6e483d4795cecd9`  
		Last Modified: Tue, 01 Feb 2022 02:58:21 GMT  
		Size: 9.7 KB (9671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c97e7cc1960856e15e5f675f68ab9e94c502022d0d90c3e5dfe2f10ca45c70f`  
		Last Modified: Tue, 01 Feb 2022 02:58:21 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761dbac0e43bea2095f68f7b87acd9008bfa394ee60c68711314e1014451572e`  
		Last Modified: Tue, 01 Feb 2022 02:58:21 GMT  
		Size: 10.7 KB (10653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b387ca1d420aba563a46bcae2ce4448fab30212c3426a6d77204cc3de9e516`  
		Last Modified: Tue, 01 Feb 2022 02:58:21 GMT  
		Size: 2.5 MB (2505823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.9-kernel-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:b227922b29f048a3e29402188e385231a6fe78349333488c299f6666ac14b7ab
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
$ docker pull websphere-liberty@sha256:ea3c8f2dda6238595f0258f407d66a2ae04c790a9c61db19177477c061582069
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.1 MB (181099801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:764f661991cdabc1031572b28414ec4b2956c46512f3c46fd31040aa8ae467e5`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:19:52 GMT
ADD file:e29b7078eb9c78ec6f3931c4beea820e4b7fe5d0d02e02e220c083dcd603aad1 in / 
# Fri, 07 Jan 2022 02:19:55 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:28:44 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 03:29:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:17 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 03:30:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 03:30:11 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:14:00 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 07:14:02 GMT
ARG OPENJ9_SCC=true
# Fri, 07 Jan 2022 07:29:16 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Fri, 07 Jan 2022 07:29:18 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Fri, 07 Jan 2022 07:29:19 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Fri, 07 Jan 2022 07:29:21 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 07 Jan 2022 07:29:22 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Fri, 07 Jan 2022 07:29:23 GMT
ARG LIBERTY_URL
# Fri, 07 Jan 2022 07:29:25 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 07 Jan 2022 07:29:50 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 07:29:52 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Jan 2022 07:29:57 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Fri, 07 Jan 2022 07:29:59 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 07 Jan 2022 07:30:06 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 07 Jan 2022 07:30:08 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Fri, 07 Jan 2022 07:30:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 07 Jan 2022 07:30:15 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 07 Jan 2022 07:30:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 07 Jan 2022 07:30:34 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:30:37 GMT
USER 1001
# Fri, 07 Jan 2022 07:30:38 GMT
EXPOSE 9080 9443
# Fri, 07 Jan 2022 07:30:41 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 07 Jan 2022 07:30:43 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:f130035f6453da800db2a1c34f617d35285297b1e549cc5fe138db9ecb704f0b`  
		Last Modified: Fri, 07 Jan 2022 02:22:21 GMT  
		Size: 30.4 MB (30432347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89db02523773279c64e3768c4c557e84eb48533e8cd88fa8b305a4631fe1620f`  
		Last Modified: Fri, 07 Jan 2022 03:32:43 GMT  
		Size: 3.1 MB (3081902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8372d0c07db9ee4af75625eda00922334eb122c9730ed278ccf2668f02d09f82`  
		Last Modified: Fri, 07 Jan 2022 03:32:57 GMT  
		Size: 128.3 MB (128256173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61a14b96da178ddf73423a23596f9c7b27d5086e505ba08273ed387a206bd69`  
		Last Modified: Fri, 07 Jan 2022 07:44:04 GMT  
		Size: 14.1 MB (14056076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a713b83c15fac82c88e50022a6a72e738ec96b4c033038a0f5ac475d287b107`  
		Last Modified: Fri, 07 Jan 2022 07:44:00 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ccedb4c7b0e2134ae863fda35e2e18e7c5bcc427262b49f3f5c433482aefe5`  
		Last Modified: Fri, 07 Jan 2022 07:44:00 GMT  
		Size: 9.7 KB (9672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe72711c0af548e44f1ea9ae5b91355fc1b970b3337afff4283e2e3fc00b105e`  
		Last Modified: Fri, 07 Jan 2022 07:44:00 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2f7614810e4d9b9bcf3b4c65a3faa4619e64151bb38e816b58356839c415a1`  
		Last Modified: Fri, 07 Jan 2022 07:44:00 GMT  
		Size: 10.7 KB (10658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd055f925c19743f7a818085e6fbfe17d4486808538f1b377fe444916f339e51`  
		Last Modified: Fri, 07 Jan 2022 07:44:01 GMT  
		Size: 5.3 MB (5252005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.9-kernel-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:4b92339930d8e278307e809bddb7f14f13986de31c4f3c41ba018169c576db78
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.6 MB (173592699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f3dbc557b6aad26beb57b7a80eaeeddf1efcf13bde4bb0409b899d0bf29f25e`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 01:42:09 GMT
ADD file:caefb9be68fabe0b9b7dba683dabb869e5165a5a13534742d73a489a3712d9a9 in / 
# Fri, 07 Jan 2022 01:42:12 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:20:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 02:20:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:20:32 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 02:21:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 02:21:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 03:56:22 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 03:56:22 GMT
ARG OPENJ9_SCC=true
# Fri, 07 Jan 2022 04:07:43 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Fri, 07 Jan 2022 04:07:43 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Fri, 07 Jan 2022 04:07:43 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Fri, 07 Jan 2022 04:07:43 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 07 Jan 2022 04:07:43 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Fri, 07 Jan 2022 04:07:44 GMT
ARG LIBERTY_URL
# Fri, 07 Jan 2022 04:07:44 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 07 Jan 2022 04:07:55 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:07:55 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Jan 2022 04:07:55 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Fri, 07 Jan 2022 04:07:56 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 07 Jan 2022 04:07:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 07 Jan 2022 04:07:57 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Fri, 07 Jan 2022 04:07:57 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 07 Jan 2022 04:07:57 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 07 Jan 2022 04:08:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 07 Jan 2022 04:08:05 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Fri, 07 Jan 2022 04:08:05 GMT
USER 1001
# Fri, 07 Jan 2022 04:08:05 GMT
EXPOSE 9080 9443
# Fri, 07 Jan 2022 04:08:05 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 07 Jan 2022 04:08:05 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:7587f9252eef493a02840102ba78c74de317d3d47f6d568af5602ff6c1c54a20`  
		Last Modified: Fri, 07 Jan 2022 01:43:57 GMT  
		Size: 25.4 MB (25362136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d5d9207d0f328849a5bf2aec9290cf52dbfa8a48e3d39b130fd1471f46a16e`  
		Last Modified: Fri, 07 Jan 2022 02:23:17 GMT  
		Size: 2.7 MB (2676903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5948905ea3b7602d130be3b792486e9fa35aaf89ee11c6a87e63c7eabe5fdcf1`  
		Last Modified: Fri, 07 Jan 2022 02:23:25 GMT  
		Size: 125.7 MB (125737337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7267f5b5b89b76bc8c416d555e78011782fd85ad9a3fa2583b37d1b05aa6a0`  
		Last Modified: Fri, 07 Jan 2022 04:18:29 GMT  
		Size: 14.1 MB (14055692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bc555cee5444c7e947070324a54b9ca25c75e443fbec66a62b35f727e40e30`  
		Last Modified: Fri, 07 Jan 2022 04:18:27 GMT  
		Size: 690.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5a8cca353c09c64957412bdf9d39bcc70a88d19de8763bf23cb63af0934e59`  
		Last Modified: Fri, 07 Jan 2022 04:18:27 GMT  
		Size: 9.7 KB (9675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebf853da83cca1c3a2656f8ab425ed0a75055e3819c7f93589c0376ee917036`  
		Last Modified: Fri, 07 Jan 2022 04:18:27 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822e8278506e653c77210970e14c7bacdb64f173c6c6da1279cee3fc8ae8d1d8`  
		Last Modified: Fri, 07 Jan 2022 04:18:27 GMT  
		Size: 10.6 KB (10644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcf6ac67b863a33e39e1aff68c25bb6577b51c851f7259b57d50877b3c7d10f`  
		Last Modified: Fri, 07 Jan 2022 04:18:27 GMT  
		Size: 5.7 MB (5739351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.1-full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:ef85825bbeeaa6a49e86a9b1fb25b16f4bebad6217f88c1dd4c7583638b5df08
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
$ docker pull websphere-liberty@sha256:b563ee89e504ed04bdcd078c9cc94a2c6d35476a8d30627dcfda9f3597cc1e47
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.6 MB (402573394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad1822da907beab36d9d11bc122f9a6e68cddd3d7ab9b7f371d8330a1c8fe397`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:20:15 GMT
ADD file:014236839eaee978894ae0bd6aecc246177a0a2c11af73f86d9cfafe5478ce18 in / 
# Fri, 07 Jan 2022 02:20:19 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:29 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:22:19 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:23:02 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 01:26:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:26:46 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:26:48 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:27:31 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:37:48 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:37:49 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:37:51 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 01 Feb 2022 02:37:52 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 01 Feb 2022 02:37:53 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 01 Feb 2022 02:37:55 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:37:56 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 01 Feb 2022 02:37:57 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:37:59 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:38:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:38:23 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:38:25 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:38:26 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:38:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:38:35 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:38:36 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:38:42 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:38:57 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:39:00 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:39:02 GMT
USER 1001
# Tue, 01 Feb 2022 02:39:03 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:39:06 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:39:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 01 Feb 2022 02:39:30 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:39:32 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 01 Feb 2022 02:43:51 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 01 Feb 2022 02:43:58 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 01 Feb 2022 02:44:50 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:e6e6dea5a8cc4bdc9e5e51e2bfa948159b69d5fbc2dca99bc41776fb04dab967`  
		Last Modified: Fri, 07 Jan 2022 02:22:43 GMT  
		Size: 33.3 MB (33286892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2db03674d664c4c13747eecf6ee9d3578adc9eb95e5a3993661ba5f37f676f8`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 17.2 MB (17206916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0441717da968406ddb594da0c1ad05e5f42434a3584422d7fab7e64763e30b4`  
		Last Modified: Tue, 01 Feb 2022 01:39:44 GMT  
		Size: 48.4 MB (48356102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6fe9db05a97733f7b24220942aef850723e6992236fcba495134a2fc03a312b`  
		Last Modified: Tue, 01 Feb 2022 01:39:36 GMT  
		Size: 3.3 MB (3331743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8c1ccdcc6fa005e08601a78df2c2c2dc66a26b3c98b205990fe93f874f2fc3`  
		Last Modified: Tue, 01 Feb 2022 02:59:19 GMT  
		Size: 14.2 MB (14229311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb27ceffbbfca5c4cf1ff0ecb2ed2ac2bb8d361bc5b9eb5710fba58612f9300`  
		Last Modified: Tue, 01 Feb 2022 02:59:15 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a7fce256b6bac271d8eca5daa9f2616c9155eabf30e665b72fe94b86ed64a3`  
		Last Modified: Tue, 01 Feb 2022 02:59:15 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e939b47f221027a6e4276f9bef4fa26cceae123bd74cf67b9f451853311c24d`  
		Last Modified: Tue, 01 Feb 2022 02:59:15 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3781ae8f25c5b975b098869c29df88b893751f727df92046e7aabf7adb8aaf8`  
		Last Modified: Tue, 01 Feb 2022 02:59:15 GMT  
		Size: 10.6 KB (10648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e1d7d246ecf25dabc1f88d90837560cb57593034e5a8f30c0dad2da5269571`  
		Last Modified: Tue, 01 Feb 2022 02:59:15 GMT  
		Size: 2.5 MB (2499995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9dd50c2e4a58c83932af6bc25499c3088a26cfc31b1b734c0ceed9274111f8`  
		Last Modified: Tue, 01 Feb 2022 02:59:53 GMT  
		Size: 271.1 MB (271128541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08cd116d8f40b91e21bb2223a14378f34b314d5d8d6026953ec119caf8fd9ae`  
		Last Modified: Tue, 01 Feb 2022 02:59:29 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb466770d8bd48209650f39278d6b5c3139a892e3041d034ff9824e041bf7845`  
		Last Modified: Tue, 01 Feb 2022 02:59:31 GMT  
		Size: 12.5 MB (12511672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.1-full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:14281953dd131e77d24e1e941ad6326c4ebc80c7f9dc79b8bc77bc7e9873870b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (396048660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cb5652f86ef090cd47eb4d458ad678e843981867c9a1f504a248358c3321994`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 01:42:20 GMT
ADD file:b6119f4fcd6a113749f515278b315ffd96aecce7006f086acb060f981e5c59db in / 
# Fri, 07 Jan 2022 01:42:22 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:15:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 02:24:31 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:00:54 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 02:01:59 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 02:02:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:02:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 02:02:34 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:40:32 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:40:32 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:40:33 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 01 Feb 2022 02:40:33 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 01 Feb 2022 02:40:33 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 01 Feb 2022 02:40:33 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:40:33 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 01 Feb 2022 02:40:33 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:40:33 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:40:45 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:40:45 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:40:46 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:40:46 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:40:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:40:47 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:40:47 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:40:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:40:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:40:54 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:40:54 GMT
USER 1001
# Tue, 01 Feb 2022 02:40:54 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:40:54 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:40:55 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 01 Feb 2022 02:41:10 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:41:10 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 01 Feb 2022 02:45:19 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 01 Feb 2022 02:45:24 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 01 Feb 2022 02:45:47 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:6d200361446626b53394c2a1a520a74a1221795562eac9b318c58e0abe147e23`  
		Last Modified: Fri, 07 Jan 2022 01:44:09 GMT  
		Size: 27.1 MB (27120999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2ea75c80fa68be6367734322b7c053932a41106663b880c832691c5c615f18`  
		Last Modified: Fri, 07 Jan 2022 02:32:46 GMT  
		Size: 15.7 MB (15739670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023197abac635771a2ec673c654381b9781d402f783200893ecc1cf31e3cbe62`  
		Last Modified: Tue, 01 Feb 2022 02:06:41 GMT  
		Size: 46.7 MB (46692338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943879201f267efb1789221ed57faefb9be861ea6702644113808ea5e86c79e4`  
		Last Modified: Tue, 01 Feb 2022 02:06:35 GMT  
		Size: 4.3 MB (4280295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971a9441a33f11684c3e9667cde258d46891756e1fb54127a4a64a59a6c07d87`  
		Last Modified: Tue, 01 Feb 2022 02:57:25 GMT  
		Size: 14.2 MB (14229001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01f7fc2e619b6062e5718b78398219595c5bb73f2e5dad10710ce4dc697e72d`  
		Last Modified: Tue, 01 Feb 2022 02:57:23 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08dfbc2aac22f01dc5b43f6ed1aab08579b7d84aeda82a0b56b4156666222fa1`  
		Last Modified: Tue, 01 Feb 2022 02:57:23 GMT  
		Size: 9.7 KB (9666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616d7e23c40c4bdacf94f3182587164f346b50dde78435436684068dfeddefab`  
		Last Modified: Tue, 01 Feb 2022 02:57:23 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfee6b39aa9ced83e885371f3d6d0d5ad3140af3f92cfd26b5d8ad6b5fc63d8e`  
		Last Modified: Tue, 01 Feb 2022 02:57:23 GMT  
		Size: 10.6 KB (10647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b95ce28aacacbfdb6b24b93a0ce60173005e08dfe97d8952254cec679c18b1`  
		Last Modified: Tue, 01 Feb 2022 02:57:23 GMT  
		Size: 2.5 MB (2484024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4164e18d9ba857469e5a11151a2a98dfff74c656f8f42d99b9dcc4ea1474cdf6`  
		Last Modified: Tue, 01 Feb 2022 02:57:43 GMT  
		Size: 271.1 MB (271128864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc6b804eee80f0c6cfcd131cfd439aa33a6e03f3bb97c80ab36986a87fdbcb5`  
		Last Modified: Tue, 01 Feb 2022 02:57:32 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414003ebc18c1ae1422a0037e6bfb6d0ec0bee1376b7656fd882b9318013f283`  
		Last Modified: Tue, 01 Feb 2022 02:57:33 GMT  
		Size: 14.4 MB (14351247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.1-full-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:36c70d093f1a55754f170fce75ce4c1e2a626bbc43ae0bf1282a1578eb3066dd
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
$ docker pull websphere-liberty@sha256:e53082942ca99dbb3d0de59c77ea7de01aa084bdd7cf565d13ddab6fc4564af5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.0 MB (465979005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6622d26f3292c95a7626ba6ec9e83d0e89ee87dd77ce686bf3e6dfee9ff80a38`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:19:52 GMT
ADD file:e29b7078eb9c78ec6f3931c4beea820e4b7fe5d0d02e02e220c083dcd603aad1 in / 
# Fri, 07 Jan 2022 02:19:55 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:28:44 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 03:29:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:17 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 03:30:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 03:30:11 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:14:00 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 07:14:02 GMT
ARG OPENJ9_SCC=true
# Tue, 25 Jan 2022 23:37:02 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 25 Jan 2022 23:37:05 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 25 Jan 2022 23:37:06 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 25 Jan 2022 23:37:07 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 25 Jan 2022 23:37:10 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 25 Jan 2022 23:37:12 GMT
ARG LIBERTY_URL
# Tue, 25 Jan 2022 23:37:15 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 25 Jan 2022 23:37:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Jan 2022 23:37:55 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Jan 2022 23:37:56 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 25 Jan 2022 23:37:59 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 25 Jan 2022 23:38:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 25 Jan 2022 23:38:13 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 25 Jan 2022 23:38:15 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 25 Jan 2022 23:38:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 25 Jan 2022 23:38:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 25 Jan 2022 23:38:42 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 25 Jan 2022 23:38:45 GMT
USER 1001
# Tue, 25 Jan 2022 23:38:47 GMT
EXPOSE 9080 9443
# Tue, 25 Jan 2022 23:38:49 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 25 Jan 2022 23:38:51 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 25 Jan 2022 23:41:09 GMT
ARG VERBOSE=false
# Tue, 25 Jan 2022 23:41:11 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 25 Jan 2022 23:46:15 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 25 Jan 2022 23:46:19 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 25 Jan 2022 23:47:23 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:f130035f6453da800db2a1c34f617d35285297b1e549cc5fe138db9ecb704f0b`  
		Last Modified: Fri, 07 Jan 2022 02:22:21 GMT  
		Size: 30.4 MB (30432347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89db02523773279c64e3768c4c557e84eb48533e8cd88fa8b305a4631fe1620f`  
		Last Modified: Fri, 07 Jan 2022 03:32:43 GMT  
		Size: 3.1 MB (3081902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8372d0c07db9ee4af75625eda00922334eb122c9730ed278ccf2668f02d09f82`  
		Last Modified: Fri, 07 Jan 2022 03:32:57 GMT  
		Size: 128.3 MB (128256173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475bb3417bf6ff364123967a770248133ab925eb6395df236943481d7a65b732`  
		Last Modified: Tue, 25 Jan 2022 23:55:20 GMT  
		Size: 14.1 MB (14130769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11826c8657c1d52b0fb45e40297c6010a446b3d2ba1a761182812cdc9df6c864`  
		Last Modified: Tue, 25 Jan 2022 23:55:15 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841ef7af7eccf58dfe3bb7bcbc88dd1bf51463c49fc9e80612695a54f7327fa8`  
		Last Modified: Tue, 25 Jan 2022 23:55:15 GMT  
		Size: 9.7 KB (9672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c5019794d1dc8fe1a55f649e87c5902cbfff7f9327b0d0c9456486aa7d5862`  
		Last Modified: Tue, 25 Jan 2022 23:55:15 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae2e35a92f7b74dd19272d8ab64cf83beba92f2bdfc9531c4d5256d585046df`  
		Last Modified: Tue, 25 Jan 2022 23:55:15 GMT  
		Size: 10.7 KB (10666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c692a5a5f5829c5a72db011cf970f6b45297eb12ddecc2805bb21bf6393ffc`  
		Last Modified: Tue, 25 Jan 2022 23:55:16 GMT  
		Size: 5.2 MB (5214016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097824fed894a925d00c793b105d7d3817497995a7883d18d7f5bbff8ee9e7da`  
		Last Modified: Tue, 25 Jan 2022 23:56:05 GMT  
		Size: 271.1 MB (271128413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03ce43b8ff2c28e974a4f611d301bc15062ebb731cf88f55678f7087228b981`  
		Last Modified: Tue, 25 Jan 2022 23:55:41 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345db745ca862919ca086830317f462c563769b2a00ebd9e4e37b079bd77bf3e`  
		Last Modified: Tue, 25 Jan 2022 23:55:44 GMT  
		Size: 13.7 MB (13713124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.1-full-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:dbdee6a2eb85182ece5453817554bb7559c2e3b5a22ec37a6d9b8740b99c7f44
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.8 MB (460821847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ef688692daaca426c929ff18a43ba696aaa411da6dd168b323547b569cdb5c9`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 01:42:09 GMT
ADD file:caefb9be68fabe0b9b7dba683dabb869e5165a5a13534742d73a489a3712d9a9 in / 
# Fri, 07 Jan 2022 01:42:12 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:20:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 02:20:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:20:32 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 02:21:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 02:21:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 03:56:22 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 03:56:22 GMT
ARG OPENJ9_SCC=true
# Tue, 25 Jan 2022 22:50:21 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 25 Jan 2022 22:50:21 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 25 Jan 2022 22:50:21 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 25 Jan 2022 22:50:21 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 25 Jan 2022 22:50:21 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 25 Jan 2022 22:50:21 GMT
ARG LIBERTY_URL
# Tue, 25 Jan 2022 22:50:22 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 25 Jan 2022 22:50:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Jan 2022 22:50:35 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Jan 2022 22:50:35 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 25 Jan 2022 22:50:35 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 25 Jan 2022 22:50:36 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 25 Jan 2022 22:50:36 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 25 Jan 2022 22:50:37 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 25 Jan 2022 22:50:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 25 Jan 2022 22:50:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 25 Jan 2022 22:50:44 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 25 Jan 2022 22:50:45 GMT
USER 1001
# Tue, 25 Jan 2022 22:50:45 GMT
EXPOSE 9080 9443
# Tue, 25 Jan 2022 22:50:45 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 25 Jan 2022 22:50:45 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 25 Jan 2022 22:51:17 GMT
ARG VERBOSE=false
# Tue, 25 Jan 2022 22:51:17 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 25 Jan 2022 22:55:34 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 25 Jan 2022 22:55:39 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 25 Jan 2022 22:56:04 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:7587f9252eef493a02840102ba78c74de317d3d47f6d568af5602ff6c1c54a20`  
		Last Modified: Fri, 07 Jan 2022 01:43:57 GMT  
		Size: 25.4 MB (25362136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d5d9207d0f328849a5bf2aec9290cf52dbfa8a48e3d39b130fd1471f46a16e`  
		Last Modified: Fri, 07 Jan 2022 02:23:17 GMT  
		Size: 2.7 MB (2676903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5948905ea3b7602d130be3b792486e9fa35aaf89ee11c6a87e63c7eabe5fdcf1`  
		Last Modified: Fri, 07 Jan 2022 02:23:25 GMT  
		Size: 125.7 MB (125737337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd61fa2a3e34c1f251eeb825db741748cb869eb5c1196679869febe1ec64d7c`  
		Last Modified: Tue, 25 Jan 2022 23:02:54 GMT  
		Size: 14.1 MB (14130397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9284e6c9904993c3203811a67b2c635e1bad3011aee96fa15aa19754efe58dd7`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8807d075a904f772644acadc1a8adc85b7a427c4e2d338446969052905495a4a`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 9.7 KB (9674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab336ecd772534b0c471553d84d95f9863daf44e36d0d8679e27414d28ee770`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3f429e652be594c3ce6efe1f666921da03c5b4f45b3e52bc8ea8c695c7789b`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 10.7 KB (10660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc741e14a82cbff06e34f42ad6d6ead805dc108549d5432ac9423b06d0ad79d3`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 5.8 MB (5806866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a8a2b6e7b7e8d63d735861ecb0e8d6445d44b35f3c7bb0ea956ea4988363e4`  
		Last Modified: Tue, 25 Jan 2022 23:03:23 GMT  
		Size: 271.1 MB (271129421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c98224775bc1cd7055fdd38e429c48cf4a21073935e580f61bc9cea0520a82e`  
		Last Modified: Tue, 25 Jan 2022 23:03:11 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397d53729199787d7c84c576d051e881766470292036adb63f3bd931e8f4d057`  
		Last Modified: Tue, 25 Jan 2022 23:03:13 GMT  
		Size: 16.0 MB (15956529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.1-kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:712693c5f904a553c3d3e646ee408c89374bcd3dc1b012bb0d431fa2976ca9c6
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
$ docker pull websphere-liberty@sha256:76d4fa7140ecc383baaeee2376b6d9d1bd8d14a314885ff702879053be0839d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118932236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf9b11312264cdecd9ef7c59e16ff71a2478f456236dd3fca284065a91b4fb61`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:20:15 GMT
ADD file:014236839eaee978894ae0bd6aecc246177a0a2c11af73f86d9cfafe5478ce18 in / 
# Fri, 07 Jan 2022 02:20:19 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:29 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:22:19 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:23:02 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 01:26:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:26:46 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:26:48 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:27:31 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:37:48 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:37:49 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:37:51 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 01 Feb 2022 02:37:52 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 01 Feb 2022 02:37:53 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 01 Feb 2022 02:37:55 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:37:56 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 01 Feb 2022 02:37:57 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:37:59 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:38:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:38:23 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:38:25 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:38:26 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:38:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:38:35 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:38:36 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:38:42 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:38:57 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:39:00 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:39:02 GMT
USER 1001
# Tue, 01 Feb 2022 02:39:03 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:39:06 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:39:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e6e6dea5a8cc4bdc9e5e51e2bfa948159b69d5fbc2dca99bc41776fb04dab967`  
		Last Modified: Fri, 07 Jan 2022 02:22:43 GMT  
		Size: 33.3 MB (33286892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2db03674d664c4c13747eecf6ee9d3578adc9eb95e5a3993661ba5f37f676f8`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 17.2 MB (17206916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0441717da968406ddb594da0c1ad05e5f42434a3584422d7fab7e64763e30b4`  
		Last Modified: Tue, 01 Feb 2022 01:39:44 GMT  
		Size: 48.4 MB (48356102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6fe9db05a97733f7b24220942aef850723e6992236fcba495134a2fc03a312b`  
		Last Modified: Tue, 01 Feb 2022 01:39:36 GMT  
		Size: 3.3 MB (3331743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8c1ccdcc6fa005e08601a78df2c2c2dc66a26b3c98b205990fe93f874f2fc3`  
		Last Modified: Tue, 01 Feb 2022 02:59:19 GMT  
		Size: 14.2 MB (14229311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb27ceffbbfca5c4cf1ff0ecb2ed2ac2bb8d361bc5b9eb5710fba58612f9300`  
		Last Modified: Tue, 01 Feb 2022 02:59:15 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a7fce256b6bac271d8eca5daa9f2616c9155eabf30e665b72fe94b86ed64a3`  
		Last Modified: Tue, 01 Feb 2022 02:59:15 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e939b47f221027a6e4276f9bef4fa26cceae123bd74cf67b9f451853311c24d`  
		Last Modified: Tue, 01 Feb 2022 02:59:15 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3781ae8f25c5b975b098869c29df88b893751f727df92046e7aabf7adb8aaf8`  
		Last Modified: Tue, 01 Feb 2022 02:59:15 GMT  
		Size: 10.6 KB (10648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e1d7d246ecf25dabc1f88d90837560cb57593034e5a8f30c0dad2da5269571`  
		Last Modified: Tue, 01 Feb 2022 02:59:15 GMT  
		Size: 2.5 MB (2499995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.1-kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:1394882f507fd6d6d085f4acdc1b60bc05e70af3cf635a9b83eae7200b974985
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110567601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a830781e6753b7a55533190d0c2333211aa5532b8651cdf39c6495c28397fb7f`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 01:42:20 GMT
ADD file:b6119f4fcd6a113749f515278b315ffd96aecce7006f086acb060f981e5c59db in / 
# Fri, 07 Jan 2022 01:42:22 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:15:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 02:24:31 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:00:54 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 02:01:59 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 02:02:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:02:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 02:02:34 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:40:32 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:40:32 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:40:33 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 01 Feb 2022 02:40:33 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 01 Feb 2022 02:40:33 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 01 Feb 2022 02:40:33 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:40:33 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 01 Feb 2022 02:40:33 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:40:33 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:40:45 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:40:45 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:40:46 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:40:46 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:40:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:40:47 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:40:47 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:40:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:40:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:40:54 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:40:54 GMT
USER 1001
# Tue, 01 Feb 2022 02:40:54 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:40:54 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:40:55 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6d200361446626b53394c2a1a520a74a1221795562eac9b318c58e0abe147e23`  
		Last Modified: Fri, 07 Jan 2022 01:44:09 GMT  
		Size: 27.1 MB (27120999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2ea75c80fa68be6367734322b7c053932a41106663b880c832691c5c615f18`  
		Last Modified: Fri, 07 Jan 2022 02:32:46 GMT  
		Size: 15.7 MB (15739670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023197abac635771a2ec673c654381b9781d402f783200893ecc1cf31e3cbe62`  
		Last Modified: Tue, 01 Feb 2022 02:06:41 GMT  
		Size: 46.7 MB (46692338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943879201f267efb1789221ed57faefb9be861ea6702644113808ea5e86c79e4`  
		Last Modified: Tue, 01 Feb 2022 02:06:35 GMT  
		Size: 4.3 MB (4280295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971a9441a33f11684c3e9667cde258d46891756e1fb54127a4a64a59a6c07d87`  
		Last Modified: Tue, 01 Feb 2022 02:57:25 GMT  
		Size: 14.2 MB (14229001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01f7fc2e619b6062e5718b78398219595c5bb73f2e5dad10710ce4dc697e72d`  
		Last Modified: Tue, 01 Feb 2022 02:57:23 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08dfbc2aac22f01dc5b43f6ed1aab08579b7d84aeda82a0b56b4156666222fa1`  
		Last Modified: Tue, 01 Feb 2022 02:57:23 GMT  
		Size: 9.7 KB (9666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616d7e23c40c4bdacf94f3182587164f346b50dde78435436684068dfeddefab`  
		Last Modified: Tue, 01 Feb 2022 02:57:23 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfee6b39aa9ced83e885371f3d6d0d5ad3140af3f92cfd26b5d8ad6b5fc63d8e`  
		Last Modified: Tue, 01 Feb 2022 02:57:23 GMT  
		Size: 10.6 KB (10647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b95ce28aacacbfdb6b24b93a0ce60173005e08dfe97d8952254cec679c18b1`  
		Last Modified: Tue, 01 Feb 2022 02:57:23 GMT  
		Size: 2.5 MB (2484024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.1-kernel-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:309ff047c4d4364acb0c4e50835dbf9be7a3b5c2cf352746c6ad205dad0d4479
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
$ docker pull websphere-liberty@sha256:4235263b35e77c51739edcd0b8f9b986da8c7f42c03c07cbc1146fb6d17893ff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.1 MB (181136519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c041af6a505d417d2030389265c2a0082fd01be1f91c315f30ba9d584bf25729`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:19:52 GMT
ADD file:e29b7078eb9c78ec6f3931c4beea820e4b7fe5d0d02e02e220c083dcd603aad1 in / 
# Fri, 07 Jan 2022 02:19:55 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:28:44 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 03:29:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:17 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 03:30:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 03:30:11 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:14:00 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 07:14:02 GMT
ARG OPENJ9_SCC=true
# Tue, 25 Jan 2022 23:37:02 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 25 Jan 2022 23:37:05 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 25 Jan 2022 23:37:06 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 25 Jan 2022 23:37:07 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 25 Jan 2022 23:37:10 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 25 Jan 2022 23:37:12 GMT
ARG LIBERTY_URL
# Tue, 25 Jan 2022 23:37:15 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 25 Jan 2022 23:37:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Jan 2022 23:37:55 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Jan 2022 23:37:56 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 25 Jan 2022 23:37:59 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 25 Jan 2022 23:38:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 25 Jan 2022 23:38:13 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 25 Jan 2022 23:38:15 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 25 Jan 2022 23:38:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 25 Jan 2022 23:38:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 25 Jan 2022 23:38:42 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 25 Jan 2022 23:38:45 GMT
USER 1001
# Tue, 25 Jan 2022 23:38:47 GMT
EXPOSE 9080 9443
# Tue, 25 Jan 2022 23:38:49 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 25 Jan 2022 23:38:51 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:f130035f6453da800db2a1c34f617d35285297b1e549cc5fe138db9ecb704f0b`  
		Last Modified: Fri, 07 Jan 2022 02:22:21 GMT  
		Size: 30.4 MB (30432347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89db02523773279c64e3768c4c557e84eb48533e8cd88fa8b305a4631fe1620f`  
		Last Modified: Fri, 07 Jan 2022 03:32:43 GMT  
		Size: 3.1 MB (3081902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8372d0c07db9ee4af75625eda00922334eb122c9730ed278ccf2668f02d09f82`  
		Last Modified: Fri, 07 Jan 2022 03:32:57 GMT  
		Size: 128.3 MB (128256173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475bb3417bf6ff364123967a770248133ab925eb6395df236943481d7a65b732`  
		Last Modified: Tue, 25 Jan 2022 23:55:20 GMT  
		Size: 14.1 MB (14130769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11826c8657c1d52b0fb45e40297c6010a446b3d2ba1a761182812cdc9df6c864`  
		Last Modified: Tue, 25 Jan 2022 23:55:15 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841ef7af7eccf58dfe3bb7bcbc88dd1bf51463c49fc9e80612695a54f7327fa8`  
		Last Modified: Tue, 25 Jan 2022 23:55:15 GMT  
		Size: 9.7 KB (9672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c5019794d1dc8fe1a55f649e87c5902cbfff7f9327b0d0c9456486aa7d5862`  
		Last Modified: Tue, 25 Jan 2022 23:55:15 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae2e35a92f7b74dd19272d8ab64cf83beba92f2bdfc9531c4d5256d585046df`  
		Last Modified: Tue, 25 Jan 2022 23:55:15 GMT  
		Size: 10.7 KB (10666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c692a5a5f5829c5a72db011cf970f6b45297eb12ddecc2805bb21bf6393ffc`  
		Last Modified: Tue, 25 Jan 2022 23:55:16 GMT  
		Size: 5.2 MB (5214016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.1-kernel-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:3d0724eb6ee1c51255d1db7243899b34f4f772d338e2f344a1cf56e6ad507c6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.7 MB (173734950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fe19001009cbad55c0c283de18313526ba8736d2aef95bdb956c506d1ce9dd9`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 01:42:09 GMT
ADD file:caefb9be68fabe0b9b7dba683dabb869e5165a5a13534742d73a489a3712d9a9 in / 
# Fri, 07 Jan 2022 01:42:12 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:20:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 02:20:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:20:32 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 02:21:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 02:21:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 03:56:22 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 03:56:22 GMT
ARG OPENJ9_SCC=true
# Tue, 25 Jan 2022 22:50:21 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 25 Jan 2022 22:50:21 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 25 Jan 2022 22:50:21 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 25 Jan 2022 22:50:21 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 25 Jan 2022 22:50:21 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 25 Jan 2022 22:50:21 GMT
ARG LIBERTY_URL
# Tue, 25 Jan 2022 22:50:22 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 25 Jan 2022 22:50:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Jan 2022 22:50:35 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Jan 2022 22:50:35 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 25 Jan 2022 22:50:35 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 25 Jan 2022 22:50:36 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 25 Jan 2022 22:50:36 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 25 Jan 2022 22:50:37 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 25 Jan 2022 22:50:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 25 Jan 2022 22:50:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 25 Jan 2022 22:50:44 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 25 Jan 2022 22:50:45 GMT
USER 1001
# Tue, 25 Jan 2022 22:50:45 GMT
EXPOSE 9080 9443
# Tue, 25 Jan 2022 22:50:45 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 25 Jan 2022 22:50:45 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:7587f9252eef493a02840102ba78c74de317d3d47f6d568af5602ff6c1c54a20`  
		Last Modified: Fri, 07 Jan 2022 01:43:57 GMT  
		Size: 25.4 MB (25362136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d5d9207d0f328849a5bf2aec9290cf52dbfa8a48e3d39b130fd1471f46a16e`  
		Last Modified: Fri, 07 Jan 2022 02:23:17 GMT  
		Size: 2.7 MB (2676903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5948905ea3b7602d130be3b792486e9fa35aaf89ee11c6a87e63c7eabe5fdcf1`  
		Last Modified: Fri, 07 Jan 2022 02:23:25 GMT  
		Size: 125.7 MB (125737337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd61fa2a3e34c1f251eeb825db741748cb869eb5c1196679869febe1ec64d7c`  
		Last Modified: Tue, 25 Jan 2022 23:02:54 GMT  
		Size: 14.1 MB (14130397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9284e6c9904993c3203811a67b2c635e1bad3011aee96fa15aa19754efe58dd7`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8807d075a904f772644acadc1a8adc85b7a427c4e2d338446969052905495a4a`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 9.7 KB (9674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab336ecd772534b0c471553d84d95f9863daf44e36d0d8679e27414d28ee770`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3f429e652be594c3ce6efe1f666921da03c5b4f45b3e52bc8ea8c695c7789b`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 10.7 KB (10660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc741e14a82cbff06e34f42ad6d6ead805dc108549d5432ac9423b06d0ad79d3`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 5.8 MB (5806866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:full`

```console
$ docker pull websphere-liberty@sha256:36c70d093f1a55754f170fce75ce4c1e2a626bbc43ae0bf1282a1578eb3066dd
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
$ docker pull websphere-liberty@sha256:e53082942ca99dbb3d0de59c77ea7de01aa084bdd7cf565d13ddab6fc4564af5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.0 MB (465979005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6622d26f3292c95a7626ba6ec9e83d0e89ee87dd77ce686bf3e6dfee9ff80a38`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:19:52 GMT
ADD file:e29b7078eb9c78ec6f3931c4beea820e4b7fe5d0d02e02e220c083dcd603aad1 in / 
# Fri, 07 Jan 2022 02:19:55 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:28:44 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 03:29:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:17 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 03:30:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 03:30:11 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:14:00 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 07:14:02 GMT
ARG OPENJ9_SCC=true
# Tue, 25 Jan 2022 23:37:02 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 25 Jan 2022 23:37:05 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 25 Jan 2022 23:37:06 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 25 Jan 2022 23:37:07 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 25 Jan 2022 23:37:10 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 25 Jan 2022 23:37:12 GMT
ARG LIBERTY_URL
# Tue, 25 Jan 2022 23:37:15 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 25 Jan 2022 23:37:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Jan 2022 23:37:55 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Jan 2022 23:37:56 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 25 Jan 2022 23:37:59 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 25 Jan 2022 23:38:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 25 Jan 2022 23:38:13 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 25 Jan 2022 23:38:15 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 25 Jan 2022 23:38:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 25 Jan 2022 23:38:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 25 Jan 2022 23:38:42 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 25 Jan 2022 23:38:45 GMT
USER 1001
# Tue, 25 Jan 2022 23:38:47 GMT
EXPOSE 9080 9443
# Tue, 25 Jan 2022 23:38:49 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 25 Jan 2022 23:38:51 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 25 Jan 2022 23:41:09 GMT
ARG VERBOSE=false
# Tue, 25 Jan 2022 23:41:11 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 25 Jan 2022 23:46:15 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 25 Jan 2022 23:46:19 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 25 Jan 2022 23:47:23 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:f130035f6453da800db2a1c34f617d35285297b1e549cc5fe138db9ecb704f0b`  
		Last Modified: Fri, 07 Jan 2022 02:22:21 GMT  
		Size: 30.4 MB (30432347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89db02523773279c64e3768c4c557e84eb48533e8cd88fa8b305a4631fe1620f`  
		Last Modified: Fri, 07 Jan 2022 03:32:43 GMT  
		Size: 3.1 MB (3081902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8372d0c07db9ee4af75625eda00922334eb122c9730ed278ccf2668f02d09f82`  
		Last Modified: Fri, 07 Jan 2022 03:32:57 GMT  
		Size: 128.3 MB (128256173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475bb3417bf6ff364123967a770248133ab925eb6395df236943481d7a65b732`  
		Last Modified: Tue, 25 Jan 2022 23:55:20 GMT  
		Size: 14.1 MB (14130769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11826c8657c1d52b0fb45e40297c6010a446b3d2ba1a761182812cdc9df6c864`  
		Last Modified: Tue, 25 Jan 2022 23:55:15 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841ef7af7eccf58dfe3bb7bcbc88dd1bf51463c49fc9e80612695a54f7327fa8`  
		Last Modified: Tue, 25 Jan 2022 23:55:15 GMT  
		Size: 9.7 KB (9672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c5019794d1dc8fe1a55f649e87c5902cbfff7f9327b0d0c9456486aa7d5862`  
		Last Modified: Tue, 25 Jan 2022 23:55:15 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae2e35a92f7b74dd19272d8ab64cf83beba92f2bdfc9531c4d5256d585046df`  
		Last Modified: Tue, 25 Jan 2022 23:55:15 GMT  
		Size: 10.7 KB (10666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c692a5a5f5829c5a72db011cf970f6b45297eb12ddecc2805bb21bf6393ffc`  
		Last Modified: Tue, 25 Jan 2022 23:55:16 GMT  
		Size: 5.2 MB (5214016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097824fed894a925d00c793b105d7d3817497995a7883d18d7f5bbff8ee9e7da`  
		Last Modified: Tue, 25 Jan 2022 23:56:05 GMT  
		Size: 271.1 MB (271128413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03ce43b8ff2c28e974a4f611d301bc15062ebb731cf88f55678f7087228b981`  
		Last Modified: Tue, 25 Jan 2022 23:55:41 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345db745ca862919ca086830317f462c563769b2a00ebd9e4e37b079bd77bf3e`  
		Last Modified: Tue, 25 Jan 2022 23:55:44 GMT  
		Size: 13.7 MB (13713124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:dbdee6a2eb85182ece5453817554bb7559c2e3b5a22ec37a6d9b8740b99c7f44
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.8 MB (460821847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ef688692daaca426c929ff18a43ba696aaa411da6dd168b323547b569cdb5c9`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 01:42:09 GMT
ADD file:caefb9be68fabe0b9b7dba683dabb869e5165a5a13534742d73a489a3712d9a9 in / 
# Fri, 07 Jan 2022 01:42:12 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:20:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 02:20:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:20:32 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 02:21:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 02:21:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 03:56:22 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 03:56:22 GMT
ARG OPENJ9_SCC=true
# Tue, 25 Jan 2022 22:50:21 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 25 Jan 2022 22:50:21 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 25 Jan 2022 22:50:21 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 25 Jan 2022 22:50:21 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 25 Jan 2022 22:50:21 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 25 Jan 2022 22:50:21 GMT
ARG LIBERTY_URL
# Tue, 25 Jan 2022 22:50:22 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 25 Jan 2022 22:50:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Jan 2022 22:50:35 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Jan 2022 22:50:35 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 25 Jan 2022 22:50:35 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 25 Jan 2022 22:50:36 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 25 Jan 2022 22:50:36 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 25 Jan 2022 22:50:37 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 25 Jan 2022 22:50:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 25 Jan 2022 22:50:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 25 Jan 2022 22:50:44 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 25 Jan 2022 22:50:45 GMT
USER 1001
# Tue, 25 Jan 2022 22:50:45 GMT
EXPOSE 9080 9443
# Tue, 25 Jan 2022 22:50:45 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 25 Jan 2022 22:50:45 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 25 Jan 2022 22:51:17 GMT
ARG VERBOSE=false
# Tue, 25 Jan 2022 22:51:17 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 25 Jan 2022 22:55:34 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 25 Jan 2022 22:55:39 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 25 Jan 2022 22:56:04 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:7587f9252eef493a02840102ba78c74de317d3d47f6d568af5602ff6c1c54a20`  
		Last Modified: Fri, 07 Jan 2022 01:43:57 GMT  
		Size: 25.4 MB (25362136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d5d9207d0f328849a5bf2aec9290cf52dbfa8a48e3d39b130fd1471f46a16e`  
		Last Modified: Fri, 07 Jan 2022 02:23:17 GMT  
		Size: 2.7 MB (2676903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5948905ea3b7602d130be3b792486e9fa35aaf89ee11c6a87e63c7eabe5fdcf1`  
		Last Modified: Fri, 07 Jan 2022 02:23:25 GMT  
		Size: 125.7 MB (125737337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd61fa2a3e34c1f251eeb825db741748cb869eb5c1196679869febe1ec64d7c`  
		Last Modified: Tue, 25 Jan 2022 23:02:54 GMT  
		Size: 14.1 MB (14130397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9284e6c9904993c3203811a67b2c635e1bad3011aee96fa15aa19754efe58dd7`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8807d075a904f772644acadc1a8adc85b7a427c4e2d338446969052905495a4a`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 9.7 KB (9674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab336ecd772534b0c471553d84d95f9863daf44e36d0d8679e27414d28ee770`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3f429e652be594c3ce6efe1f666921da03c5b4f45b3e52bc8ea8c695c7789b`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 10.7 KB (10660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc741e14a82cbff06e34f42ad6d6ead805dc108549d5432ac9423b06d0ad79d3`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 5.8 MB (5806866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a8a2b6e7b7e8d63d735861ecb0e8d6445d44b35f3c7bb0ea956ea4988363e4`  
		Last Modified: Tue, 25 Jan 2022 23:03:23 GMT  
		Size: 271.1 MB (271129421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c98224775bc1cd7055fdd38e429c48cf4a21073935e580f61bc9cea0520a82e`  
		Last Modified: Tue, 25 Jan 2022 23:03:11 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397d53729199787d7c84c576d051e881766470292036adb63f3bd931e8f4d057`  
		Last Modified: Tue, 25 Jan 2022 23:03:13 GMT  
		Size: 16.0 MB (15956529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:ef85825bbeeaa6a49e86a9b1fb25b16f4bebad6217f88c1dd4c7583638b5df08
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
$ docker pull websphere-liberty@sha256:b563ee89e504ed04bdcd078c9cc94a2c6d35476a8d30627dcfda9f3597cc1e47
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.6 MB (402573394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad1822da907beab36d9d11bc122f9a6e68cddd3d7ab9b7f371d8330a1c8fe397`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:20:15 GMT
ADD file:014236839eaee978894ae0bd6aecc246177a0a2c11af73f86d9cfafe5478ce18 in / 
# Fri, 07 Jan 2022 02:20:19 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:29 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:22:19 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:23:02 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 01:26:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:26:46 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:26:48 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:27:31 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:37:48 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:37:49 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:37:51 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 01 Feb 2022 02:37:52 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 01 Feb 2022 02:37:53 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 01 Feb 2022 02:37:55 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:37:56 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 01 Feb 2022 02:37:57 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:37:59 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:38:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:38:23 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:38:25 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:38:26 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:38:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:38:35 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:38:36 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:38:42 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:38:57 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:39:00 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:39:02 GMT
USER 1001
# Tue, 01 Feb 2022 02:39:03 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:39:06 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:39:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 01 Feb 2022 02:39:30 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:39:32 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 01 Feb 2022 02:43:51 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 01 Feb 2022 02:43:58 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 01 Feb 2022 02:44:50 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:e6e6dea5a8cc4bdc9e5e51e2bfa948159b69d5fbc2dca99bc41776fb04dab967`  
		Last Modified: Fri, 07 Jan 2022 02:22:43 GMT  
		Size: 33.3 MB (33286892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2db03674d664c4c13747eecf6ee9d3578adc9eb95e5a3993661ba5f37f676f8`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 17.2 MB (17206916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0441717da968406ddb594da0c1ad05e5f42434a3584422d7fab7e64763e30b4`  
		Last Modified: Tue, 01 Feb 2022 01:39:44 GMT  
		Size: 48.4 MB (48356102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6fe9db05a97733f7b24220942aef850723e6992236fcba495134a2fc03a312b`  
		Last Modified: Tue, 01 Feb 2022 01:39:36 GMT  
		Size: 3.3 MB (3331743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8c1ccdcc6fa005e08601a78df2c2c2dc66a26b3c98b205990fe93f874f2fc3`  
		Last Modified: Tue, 01 Feb 2022 02:59:19 GMT  
		Size: 14.2 MB (14229311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb27ceffbbfca5c4cf1ff0ecb2ed2ac2bb8d361bc5b9eb5710fba58612f9300`  
		Last Modified: Tue, 01 Feb 2022 02:59:15 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a7fce256b6bac271d8eca5daa9f2616c9155eabf30e665b72fe94b86ed64a3`  
		Last Modified: Tue, 01 Feb 2022 02:59:15 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e939b47f221027a6e4276f9bef4fa26cceae123bd74cf67b9f451853311c24d`  
		Last Modified: Tue, 01 Feb 2022 02:59:15 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3781ae8f25c5b975b098869c29df88b893751f727df92046e7aabf7adb8aaf8`  
		Last Modified: Tue, 01 Feb 2022 02:59:15 GMT  
		Size: 10.6 KB (10648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e1d7d246ecf25dabc1f88d90837560cb57593034e5a8f30c0dad2da5269571`  
		Last Modified: Tue, 01 Feb 2022 02:59:15 GMT  
		Size: 2.5 MB (2499995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9dd50c2e4a58c83932af6bc25499c3088a26cfc31b1b734c0ceed9274111f8`  
		Last Modified: Tue, 01 Feb 2022 02:59:53 GMT  
		Size: 271.1 MB (271128541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08cd116d8f40b91e21bb2223a14378f34b314d5d8d6026953ec119caf8fd9ae`  
		Last Modified: Tue, 01 Feb 2022 02:59:29 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb466770d8bd48209650f39278d6b5c3139a892e3041d034ff9824e041bf7845`  
		Last Modified: Tue, 01 Feb 2022 02:59:31 GMT  
		Size: 12.5 MB (12511672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:14281953dd131e77d24e1e941ad6326c4ebc80c7f9dc79b8bc77bc7e9873870b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (396048660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cb5652f86ef090cd47eb4d458ad678e843981867c9a1f504a248358c3321994`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 01:42:20 GMT
ADD file:b6119f4fcd6a113749f515278b315ffd96aecce7006f086acb060f981e5c59db in / 
# Fri, 07 Jan 2022 01:42:22 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:15:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 02:24:31 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:00:54 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 02:01:59 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 02:02:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:02:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 02:02:34 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:40:32 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:40:32 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:40:33 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 01 Feb 2022 02:40:33 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 01 Feb 2022 02:40:33 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 01 Feb 2022 02:40:33 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:40:33 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 01 Feb 2022 02:40:33 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:40:33 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:40:45 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:40:45 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:40:46 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:40:46 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:40:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:40:47 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:40:47 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:40:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:40:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:40:54 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:40:54 GMT
USER 1001
# Tue, 01 Feb 2022 02:40:54 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:40:54 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:40:55 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 01 Feb 2022 02:41:10 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:41:10 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 01 Feb 2022 02:45:19 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 01 Feb 2022 02:45:24 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 01 Feb 2022 02:45:47 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:6d200361446626b53394c2a1a520a74a1221795562eac9b318c58e0abe147e23`  
		Last Modified: Fri, 07 Jan 2022 01:44:09 GMT  
		Size: 27.1 MB (27120999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2ea75c80fa68be6367734322b7c053932a41106663b880c832691c5c615f18`  
		Last Modified: Fri, 07 Jan 2022 02:32:46 GMT  
		Size: 15.7 MB (15739670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023197abac635771a2ec673c654381b9781d402f783200893ecc1cf31e3cbe62`  
		Last Modified: Tue, 01 Feb 2022 02:06:41 GMT  
		Size: 46.7 MB (46692338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943879201f267efb1789221ed57faefb9be861ea6702644113808ea5e86c79e4`  
		Last Modified: Tue, 01 Feb 2022 02:06:35 GMT  
		Size: 4.3 MB (4280295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971a9441a33f11684c3e9667cde258d46891756e1fb54127a4a64a59a6c07d87`  
		Last Modified: Tue, 01 Feb 2022 02:57:25 GMT  
		Size: 14.2 MB (14229001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01f7fc2e619b6062e5718b78398219595c5bb73f2e5dad10710ce4dc697e72d`  
		Last Modified: Tue, 01 Feb 2022 02:57:23 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08dfbc2aac22f01dc5b43f6ed1aab08579b7d84aeda82a0b56b4156666222fa1`  
		Last Modified: Tue, 01 Feb 2022 02:57:23 GMT  
		Size: 9.7 KB (9666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616d7e23c40c4bdacf94f3182587164f346b50dde78435436684068dfeddefab`  
		Last Modified: Tue, 01 Feb 2022 02:57:23 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfee6b39aa9ced83e885371f3d6d0d5ad3140af3f92cfd26b5d8ad6b5fc63d8e`  
		Last Modified: Tue, 01 Feb 2022 02:57:23 GMT  
		Size: 10.6 KB (10647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b95ce28aacacbfdb6b24b93a0ce60173005e08dfe97d8952254cec679c18b1`  
		Last Modified: Tue, 01 Feb 2022 02:57:23 GMT  
		Size: 2.5 MB (2484024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4164e18d9ba857469e5a11151a2a98dfff74c656f8f42d99b9dcc4ea1474cdf6`  
		Last Modified: Tue, 01 Feb 2022 02:57:43 GMT  
		Size: 271.1 MB (271128864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc6b804eee80f0c6cfcd131cfd439aa33a6e03f3bb97c80ab36986a87fdbcb5`  
		Last Modified: Tue, 01 Feb 2022 02:57:32 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414003ebc18c1ae1422a0037e6bfb6d0ec0bee1376b7656fd882b9318013f283`  
		Last Modified: Tue, 01 Feb 2022 02:57:33 GMT  
		Size: 14.4 MB (14351247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:kernel`

```console
$ docker pull websphere-liberty@sha256:309ff047c4d4364acb0c4e50835dbf9be7a3b5c2cf352746c6ad205dad0d4479
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
$ docker pull websphere-liberty@sha256:4235263b35e77c51739edcd0b8f9b986da8c7f42c03c07cbc1146fb6d17893ff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.1 MB (181136519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c041af6a505d417d2030389265c2a0082fd01be1f91c315f30ba9d584bf25729`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:19:52 GMT
ADD file:e29b7078eb9c78ec6f3931c4beea820e4b7fe5d0d02e02e220c083dcd603aad1 in / 
# Fri, 07 Jan 2022 02:19:55 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:28:44 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 03:29:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:17 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 03:30:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 03:30:11 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:14:00 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 07:14:02 GMT
ARG OPENJ9_SCC=true
# Tue, 25 Jan 2022 23:37:02 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 25 Jan 2022 23:37:05 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 25 Jan 2022 23:37:06 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 25 Jan 2022 23:37:07 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 25 Jan 2022 23:37:10 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 25 Jan 2022 23:37:12 GMT
ARG LIBERTY_URL
# Tue, 25 Jan 2022 23:37:15 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 25 Jan 2022 23:37:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Jan 2022 23:37:55 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Jan 2022 23:37:56 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 25 Jan 2022 23:37:59 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 25 Jan 2022 23:38:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 25 Jan 2022 23:38:13 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 25 Jan 2022 23:38:15 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 25 Jan 2022 23:38:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 25 Jan 2022 23:38:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 25 Jan 2022 23:38:42 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 25 Jan 2022 23:38:45 GMT
USER 1001
# Tue, 25 Jan 2022 23:38:47 GMT
EXPOSE 9080 9443
# Tue, 25 Jan 2022 23:38:49 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 25 Jan 2022 23:38:51 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:f130035f6453da800db2a1c34f617d35285297b1e549cc5fe138db9ecb704f0b`  
		Last Modified: Fri, 07 Jan 2022 02:22:21 GMT  
		Size: 30.4 MB (30432347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89db02523773279c64e3768c4c557e84eb48533e8cd88fa8b305a4631fe1620f`  
		Last Modified: Fri, 07 Jan 2022 03:32:43 GMT  
		Size: 3.1 MB (3081902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8372d0c07db9ee4af75625eda00922334eb122c9730ed278ccf2668f02d09f82`  
		Last Modified: Fri, 07 Jan 2022 03:32:57 GMT  
		Size: 128.3 MB (128256173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475bb3417bf6ff364123967a770248133ab925eb6395df236943481d7a65b732`  
		Last Modified: Tue, 25 Jan 2022 23:55:20 GMT  
		Size: 14.1 MB (14130769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11826c8657c1d52b0fb45e40297c6010a446b3d2ba1a761182812cdc9df6c864`  
		Last Modified: Tue, 25 Jan 2022 23:55:15 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841ef7af7eccf58dfe3bb7bcbc88dd1bf51463c49fc9e80612695a54f7327fa8`  
		Last Modified: Tue, 25 Jan 2022 23:55:15 GMT  
		Size: 9.7 KB (9672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c5019794d1dc8fe1a55f649e87c5902cbfff7f9327b0d0c9456486aa7d5862`  
		Last Modified: Tue, 25 Jan 2022 23:55:15 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae2e35a92f7b74dd19272d8ab64cf83beba92f2bdfc9531c4d5256d585046df`  
		Last Modified: Tue, 25 Jan 2022 23:55:15 GMT  
		Size: 10.7 KB (10666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c692a5a5f5829c5a72db011cf970f6b45297eb12ddecc2805bb21bf6393ffc`  
		Last Modified: Tue, 25 Jan 2022 23:55:16 GMT  
		Size: 5.2 MB (5214016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:3d0724eb6ee1c51255d1db7243899b34f4f772d338e2f344a1cf56e6ad507c6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.7 MB (173734950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fe19001009cbad55c0c283de18313526ba8736d2aef95bdb956c506d1ce9dd9`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 01:42:09 GMT
ADD file:caefb9be68fabe0b9b7dba683dabb869e5165a5a13534742d73a489a3712d9a9 in / 
# Fri, 07 Jan 2022 01:42:12 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:20:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 02:20:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:20:32 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 02:21:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 02:21:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 03:56:22 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 03:56:22 GMT
ARG OPENJ9_SCC=true
# Tue, 25 Jan 2022 22:50:21 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 25 Jan 2022 22:50:21 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 25 Jan 2022 22:50:21 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 25 Jan 2022 22:50:21 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 25 Jan 2022 22:50:21 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 25 Jan 2022 22:50:21 GMT
ARG LIBERTY_URL
# Tue, 25 Jan 2022 22:50:22 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 25 Jan 2022 22:50:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Jan 2022 22:50:35 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Jan 2022 22:50:35 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 25 Jan 2022 22:50:35 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 25 Jan 2022 22:50:36 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 25 Jan 2022 22:50:36 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 25 Jan 2022 22:50:37 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 25 Jan 2022 22:50:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 25 Jan 2022 22:50:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 25 Jan 2022 22:50:44 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 25 Jan 2022 22:50:45 GMT
USER 1001
# Tue, 25 Jan 2022 22:50:45 GMT
EXPOSE 9080 9443
# Tue, 25 Jan 2022 22:50:45 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 25 Jan 2022 22:50:45 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:7587f9252eef493a02840102ba78c74de317d3d47f6d568af5602ff6c1c54a20`  
		Last Modified: Fri, 07 Jan 2022 01:43:57 GMT  
		Size: 25.4 MB (25362136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d5d9207d0f328849a5bf2aec9290cf52dbfa8a48e3d39b130fd1471f46a16e`  
		Last Modified: Fri, 07 Jan 2022 02:23:17 GMT  
		Size: 2.7 MB (2676903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5948905ea3b7602d130be3b792486e9fa35aaf89ee11c6a87e63c7eabe5fdcf1`  
		Last Modified: Fri, 07 Jan 2022 02:23:25 GMT  
		Size: 125.7 MB (125737337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd61fa2a3e34c1f251eeb825db741748cb869eb5c1196679869febe1ec64d7c`  
		Last Modified: Tue, 25 Jan 2022 23:02:54 GMT  
		Size: 14.1 MB (14130397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9284e6c9904993c3203811a67b2c635e1bad3011aee96fa15aa19754efe58dd7`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8807d075a904f772644acadc1a8adc85b7a427c4e2d338446969052905495a4a`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 9.7 KB (9674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab336ecd772534b0c471553d84d95f9863daf44e36d0d8679e27414d28ee770`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3f429e652be594c3ce6efe1f666921da03c5b4f45b3e52bc8ea8c695c7789b`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 10.7 KB (10660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc741e14a82cbff06e34f42ad6d6ead805dc108549d5432ac9423b06d0ad79d3`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 5.8 MB (5806866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:712693c5f904a553c3d3e646ee408c89374bcd3dc1b012bb0d431fa2976ca9c6
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
$ docker pull websphere-liberty@sha256:76d4fa7140ecc383baaeee2376b6d9d1bd8d14a314885ff702879053be0839d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118932236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf9b11312264cdecd9ef7c59e16ff71a2478f456236dd3fca284065a91b4fb61`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:20:15 GMT
ADD file:014236839eaee978894ae0bd6aecc246177a0a2c11af73f86d9cfafe5478ce18 in / 
# Fri, 07 Jan 2022 02:20:19 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:29 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 04:22:19 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 01:23:02 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 01:26:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 01:26:46 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:26:48 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 01:27:31 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:37:48 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:37:49 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:37:51 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 01 Feb 2022 02:37:52 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 01 Feb 2022 02:37:53 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 01 Feb 2022 02:37:55 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:37:56 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 01 Feb 2022 02:37:57 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:37:59 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:38:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:38:23 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:38:25 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:38:26 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:38:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:38:35 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:38:36 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:38:42 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:38:57 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:39:00 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:39:02 GMT
USER 1001
# Tue, 01 Feb 2022 02:39:03 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:39:06 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:39:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e6e6dea5a8cc4bdc9e5e51e2bfa948159b69d5fbc2dca99bc41776fb04dab967`  
		Last Modified: Fri, 07 Jan 2022 02:22:43 GMT  
		Size: 33.3 MB (33286892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2db03674d664c4c13747eecf6ee9d3578adc9eb95e5a3993661ba5f37f676f8`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 17.2 MB (17206916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0441717da968406ddb594da0c1ad05e5f42434a3584422d7fab7e64763e30b4`  
		Last Modified: Tue, 01 Feb 2022 01:39:44 GMT  
		Size: 48.4 MB (48356102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6fe9db05a97733f7b24220942aef850723e6992236fcba495134a2fc03a312b`  
		Last Modified: Tue, 01 Feb 2022 01:39:36 GMT  
		Size: 3.3 MB (3331743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8c1ccdcc6fa005e08601a78df2c2c2dc66a26b3c98b205990fe93f874f2fc3`  
		Last Modified: Tue, 01 Feb 2022 02:59:19 GMT  
		Size: 14.2 MB (14229311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb27ceffbbfca5c4cf1ff0ecb2ed2ac2bb8d361bc5b9eb5710fba58612f9300`  
		Last Modified: Tue, 01 Feb 2022 02:59:15 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a7fce256b6bac271d8eca5daa9f2616c9155eabf30e665b72fe94b86ed64a3`  
		Last Modified: Tue, 01 Feb 2022 02:59:15 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e939b47f221027a6e4276f9bef4fa26cceae123bd74cf67b9f451853311c24d`  
		Last Modified: Tue, 01 Feb 2022 02:59:15 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3781ae8f25c5b975b098869c29df88b893751f727df92046e7aabf7adb8aaf8`  
		Last Modified: Tue, 01 Feb 2022 02:59:15 GMT  
		Size: 10.6 KB (10648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e1d7d246ecf25dabc1f88d90837560cb57593034e5a8f30c0dad2da5269571`  
		Last Modified: Tue, 01 Feb 2022 02:59:15 GMT  
		Size: 2.5 MB (2499995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:1394882f507fd6d6d085f4acdc1b60bc05e70af3cf635a9b83eae7200b974985
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110567601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a830781e6753b7a55533190d0c2333211aa5532b8651cdf39c6495c28397fb7f`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 01:42:20 GMT
ADD file:b6119f4fcd6a113749f515278b315ffd96aecce7006f086acb060f981e5c59db in / 
# Fri, 07 Jan 2022 01:42:22 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:15:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 02:24:31 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:00:54 GMT
ENV JAVA_VERSION=jdk-11.0.14+9_openj9-0.30.0
# Tue, 01 Feb 2022 02:01:59 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='35f00878b7e9eaf7c18f7e12f3f0dfb18e1af23523d8822cd4b50877394d0b52';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='367792c18cf864dd1938c85ed34fa206c9a760664bc3695b21c6c161b8bf245f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='05bf1cd12b0e599844f55c0cc6b33ad557090a6fd7f836caf299be9909438c2a';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='b2fdeac239dd16b4fd02bef83e843f78ac242f54e7c9b0ebc89cf3dbd1de2e19';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14%2B9_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_11.0.14_9_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 02:02:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:02:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 01 Feb 2022 02:02:34 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 01 Feb 2022 02:40:32 GMT
ARG VERBOSE=false
# Tue, 01 Feb 2022 02:40:32 GMT
ARG OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:40:33 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 01 Feb 2022 02:40:33 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 01 Feb 2022 02:40:33 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 01 Feb 2022 02:40:33 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 01 Feb 2022 02:40:33 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 01 Feb 2022 02:40:33 GMT
ARG LIBERTY_URL
# Tue, 01 Feb 2022 02:40:33 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 01 Feb 2022 02:40:45 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Feb 2022 02:40:45 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:40:46 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 01 Feb 2022 02:40:46 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 01 Feb 2022 02:40:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 01 Feb 2022 02:40:47 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 01 Feb 2022 02:40:47 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 01 Feb 2022 02:40:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 01 Feb 2022 02:40:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 01 Feb 2022 02:40:54 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 01 Feb 2022 02:40:54 GMT
USER 1001
# Tue, 01 Feb 2022 02:40:54 GMT
EXPOSE 9080 9443
# Tue, 01 Feb 2022 02:40:54 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 01 Feb 2022 02:40:55 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6d200361446626b53394c2a1a520a74a1221795562eac9b318c58e0abe147e23`  
		Last Modified: Fri, 07 Jan 2022 01:44:09 GMT  
		Size: 27.1 MB (27120999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2ea75c80fa68be6367734322b7c053932a41106663b880c832691c5c615f18`  
		Last Modified: Fri, 07 Jan 2022 02:32:46 GMT  
		Size: 15.7 MB (15739670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023197abac635771a2ec673c654381b9781d402f783200893ecc1cf31e3cbe62`  
		Last Modified: Tue, 01 Feb 2022 02:06:41 GMT  
		Size: 46.7 MB (46692338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943879201f267efb1789221ed57faefb9be861ea6702644113808ea5e86c79e4`  
		Last Modified: Tue, 01 Feb 2022 02:06:35 GMT  
		Size: 4.3 MB (4280295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971a9441a33f11684c3e9667cde258d46891756e1fb54127a4a64a59a6c07d87`  
		Last Modified: Tue, 01 Feb 2022 02:57:25 GMT  
		Size: 14.2 MB (14229001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01f7fc2e619b6062e5718b78398219595c5bb73f2e5dad10710ce4dc697e72d`  
		Last Modified: Tue, 01 Feb 2022 02:57:23 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08dfbc2aac22f01dc5b43f6ed1aab08579b7d84aeda82a0b56b4156666222fa1`  
		Last Modified: Tue, 01 Feb 2022 02:57:23 GMT  
		Size: 9.7 KB (9666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616d7e23c40c4bdacf94f3182587164f346b50dde78435436684068dfeddefab`  
		Last Modified: Tue, 01 Feb 2022 02:57:23 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfee6b39aa9ced83e885371f3d6d0d5ad3140af3f92cfd26b5d8ad6b5fc63d8e`  
		Last Modified: Tue, 01 Feb 2022 02:57:23 GMT  
		Size: 10.6 KB (10647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b95ce28aacacbfdb6b24b93a0ce60173005e08dfe97d8952254cec679c18b1`  
		Last Modified: Tue, 01 Feb 2022 02:57:23 GMT  
		Size: 2.5 MB (2484024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:latest`

```console
$ docker pull websphere-liberty@sha256:36c70d093f1a55754f170fce75ce4c1e2a626bbc43ae0bf1282a1578eb3066dd
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
$ docker pull websphere-liberty@sha256:e53082942ca99dbb3d0de59c77ea7de01aa084bdd7cf565d13ddab6fc4564af5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.0 MB (465979005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6622d26f3292c95a7626ba6ec9e83d0e89ee87dd77ce686bf3e6dfee9ff80a38`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 02:19:52 GMT
ADD file:e29b7078eb9c78ec6f3931c4beea820e4b7fe5d0d02e02e220c083dcd603aad1 in / 
# Fri, 07 Jan 2022 02:19:55 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:28:44 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 03:29:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:29:17 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 03:30:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 03:30:11 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 07:14:00 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 07:14:02 GMT
ARG OPENJ9_SCC=true
# Tue, 25 Jan 2022 23:37:02 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 25 Jan 2022 23:37:05 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 25 Jan 2022 23:37:06 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 25 Jan 2022 23:37:07 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 25 Jan 2022 23:37:10 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 25 Jan 2022 23:37:12 GMT
ARG LIBERTY_URL
# Tue, 25 Jan 2022 23:37:15 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 25 Jan 2022 23:37:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Jan 2022 23:37:55 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Jan 2022 23:37:56 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 25 Jan 2022 23:37:59 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 25 Jan 2022 23:38:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 25 Jan 2022 23:38:13 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 25 Jan 2022 23:38:15 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 25 Jan 2022 23:38:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 25 Jan 2022 23:38:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 25 Jan 2022 23:38:42 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 25 Jan 2022 23:38:45 GMT
USER 1001
# Tue, 25 Jan 2022 23:38:47 GMT
EXPOSE 9080 9443
# Tue, 25 Jan 2022 23:38:49 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 25 Jan 2022 23:38:51 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 25 Jan 2022 23:41:09 GMT
ARG VERBOSE=false
# Tue, 25 Jan 2022 23:41:11 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 25 Jan 2022 23:46:15 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 25 Jan 2022 23:46:19 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 25 Jan 2022 23:47:23 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:f130035f6453da800db2a1c34f617d35285297b1e549cc5fe138db9ecb704f0b`  
		Last Modified: Fri, 07 Jan 2022 02:22:21 GMT  
		Size: 30.4 MB (30432347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89db02523773279c64e3768c4c557e84eb48533e8cd88fa8b305a4631fe1620f`  
		Last Modified: Fri, 07 Jan 2022 03:32:43 GMT  
		Size: 3.1 MB (3081902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8372d0c07db9ee4af75625eda00922334eb122c9730ed278ccf2668f02d09f82`  
		Last Modified: Fri, 07 Jan 2022 03:32:57 GMT  
		Size: 128.3 MB (128256173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475bb3417bf6ff364123967a770248133ab925eb6395df236943481d7a65b732`  
		Last Modified: Tue, 25 Jan 2022 23:55:20 GMT  
		Size: 14.1 MB (14130769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11826c8657c1d52b0fb45e40297c6010a446b3d2ba1a761182812cdc9df6c864`  
		Last Modified: Tue, 25 Jan 2022 23:55:15 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841ef7af7eccf58dfe3bb7bcbc88dd1bf51463c49fc9e80612695a54f7327fa8`  
		Last Modified: Tue, 25 Jan 2022 23:55:15 GMT  
		Size: 9.7 KB (9672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c5019794d1dc8fe1a55f649e87c5902cbfff7f9327b0d0c9456486aa7d5862`  
		Last Modified: Tue, 25 Jan 2022 23:55:15 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae2e35a92f7b74dd19272d8ab64cf83beba92f2bdfc9531c4d5256d585046df`  
		Last Modified: Tue, 25 Jan 2022 23:55:15 GMT  
		Size: 10.7 KB (10666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c692a5a5f5829c5a72db011cf970f6b45297eb12ddecc2805bb21bf6393ffc`  
		Last Modified: Tue, 25 Jan 2022 23:55:16 GMT  
		Size: 5.2 MB (5214016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097824fed894a925d00c793b105d7d3817497995a7883d18d7f5bbff8ee9e7da`  
		Last Modified: Tue, 25 Jan 2022 23:56:05 GMT  
		Size: 271.1 MB (271128413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03ce43b8ff2c28e974a4f611d301bc15062ebb731cf88f55678f7087228b981`  
		Last Modified: Tue, 25 Jan 2022 23:55:41 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345db745ca862919ca086830317f462c563769b2a00ebd9e4e37b079bd77bf3e`  
		Last Modified: Tue, 25 Jan 2022 23:55:44 GMT  
		Size: 13.7 MB (13713124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:dbdee6a2eb85182ece5453817554bb7559c2e3b5a22ec37a6d9b8740b99c7f44
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.8 MB (460821847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ef688692daaca426c929ff18a43ba696aaa411da6dd168b323547b569cdb5c9`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 07 Jan 2022 01:42:09 GMT
ADD file:caefb9be68fabe0b9b7dba683dabb869e5165a5a13534742d73a489a3712d9a9 in / 
# Fri, 07 Jan 2022 01:42:12 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:20:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 07 Jan 2022 02:20:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:20:32 GMT
ENV JAVA_VERSION=8.0.7.0
# Fri, 07 Jan 2022 02:21:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='18d56640102a5e6b1326cc762dbf9ae19f00f81574f38ae1857d9f65761123ff';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='24af7fb9be209a68314dc341e5b62284d3625567872286f484cb296b9c551974';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='75ccfbaf6526ab854e193060110a9bef7878d186a95c3e0d57448ab96c09aa1a';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='200621b68eb39ae00ee875b31d6455bb2dcc5c8d050a4e4f8aa4fc7525a53d35';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='73f941590d60287d9d480884698120149bf2f9b8da04d2501b450f320a5be181';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 07 Jan 2022 02:21:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 07 Jan 2022 03:56:22 GMT
ARG VERBOSE=false
# Fri, 07 Jan 2022 03:56:22 GMT
ARG OPENJ9_SCC=true
# Tue, 25 Jan 2022 22:50:21 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Tue, 25 Jan 2022 22:50:21 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Tue, 25 Jan 2022 22:50:21 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Tue, 25 Jan 2022 22:50:21 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 25 Jan 2022 22:50:21 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Tue, 25 Jan 2022 22:50:21 GMT
ARG LIBERTY_URL
# Tue, 25 Jan 2022 22:50:22 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 25 Jan 2022 22:50:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Jan 2022 22:50:35 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Jan 2022 22:50:35 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Tue, 25 Jan 2022 22:50:35 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 25 Jan 2022 22:50:36 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 25 Jan 2022 22:50:36 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 25 Jan 2022 22:50:37 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 25 Jan 2022 22:50:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 25 Jan 2022 22:50:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 25 Jan 2022 22:50:44 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 25 Jan 2022 22:50:45 GMT
USER 1001
# Tue, 25 Jan 2022 22:50:45 GMT
EXPOSE 9080 9443
# Tue, 25 Jan 2022 22:50:45 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 25 Jan 2022 22:50:45 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 25 Jan 2022 22:51:17 GMT
ARG VERBOSE=false
# Tue, 25 Jan 2022 22:51:17 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 25 Jan 2022 22:55:34 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 25 Jan 2022 22:55:39 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 25 Jan 2022 22:56:04 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:7587f9252eef493a02840102ba78c74de317d3d47f6d568af5602ff6c1c54a20`  
		Last Modified: Fri, 07 Jan 2022 01:43:57 GMT  
		Size: 25.4 MB (25362136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d5d9207d0f328849a5bf2aec9290cf52dbfa8a48e3d39b130fd1471f46a16e`  
		Last Modified: Fri, 07 Jan 2022 02:23:17 GMT  
		Size: 2.7 MB (2676903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5948905ea3b7602d130be3b792486e9fa35aaf89ee11c6a87e63c7eabe5fdcf1`  
		Last Modified: Fri, 07 Jan 2022 02:23:25 GMT  
		Size: 125.7 MB (125737337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd61fa2a3e34c1f251eeb825db741748cb869eb5c1196679869febe1ec64d7c`  
		Last Modified: Tue, 25 Jan 2022 23:02:54 GMT  
		Size: 14.1 MB (14130397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9284e6c9904993c3203811a67b2c635e1bad3011aee96fa15aa19754efe58dd7`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8807d075a904f772644acadc1a8adc85b7a427c4e2d338446969052905495a4a`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 9.7 KB (9674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab336ecd772534b0c471553d84d95f9863daf44e36d0d8679e27414d28ee770`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3f429e652be594c3ce6efe1f666921da03c5b4f45b3e52bc8ea8c695c7789b`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 10.7 KB (10660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc741e14a82cbff06e34f42ad6d6ead805dc108549d5432ac9423b06d0ad79d3`  
		Last Modified: Tue, 25 Jan 2022 23:02:49 GMT  
		Size: 5.8 MB (5806866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a8a2b6e7b7e8d63d735861ecb0e8d6445d44b35f3c7bb0ea956ea4988363e4`  
		Last Modified: Tue, 25 Jan 2022 23:03:23 GMT  
		Size: 271.1 MB (271129421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c98224775bc1cd7055fdd38e429c48cf4a21073935e580f61bc9cea0520a82e`  
		Last Modified: Tue, 25 Jan 2022 23:03:11 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397d53729199787d7c84c576d051e881766470292036adb63f3bd931e8f4d057`  
		Last Modified: Tue, 25 Jan 2022 23:03:13 GMT  
		Size: 16.0 MB (15956529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
