<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `websphere-liberty`

-	[`websphere-liberty:21.0.0.10-full-java11-openj9`](#websphere-liberty210010-full-java11-openj9)
-	[`websphere-liberty:21.0.0.10-full-java8-ibmjava`](#websphere-liberty210010-full-java8-ibmjava)
-	[`websphere-liberty:21.0.0.10-kernel-java11-openj9`](#websphere-liberty210010-kernel-java11-openj9)
-	[`websphere-liberty:21.0.0.10-kernel-java8-ibmjava`](#websphere-liberty210010-kernel-java8-ibmjava)
-	[`websphere-liberty:21.0.0.6-full-java11-openj9`](#websphere-liberty21006-full-java11-openj9)
-	[`websphere-liberty:21.0.0.6-full-java8-ibmjava`](#websphere-liberty21006-full-java8-ibmjava)
-	[`websphere-liberty:21.0.0.6-kernel-java11-openj9`](#websphere-liberty21006-kernel-java11-openj9)
-	[`websphere-liberty:21.0.0.6-kernel-java8-ibmjava`](#websphere-liberty21006-kernel-java8-ibmjava)
-	[`websphere-liberty:21.0.0.9-full-java11-openj9`](#websphere-liberty21009-full-java11-openj9)
-	[`websphere-liberty:21.0.0.9-full-java8-ibmjava`](#websphere-liberty21009-full-java8-ibmjava)
-	[`websphere-liberty:21.0.0.9-kernel-java11-openj9`](#websphere-liberty21009-kernel-java11-openj9)
-	[`websphere-liberty:21.0.0.9-kernel-java8-ibmjava`](#websphere-liberty21009-kernel-java8-ibmjava)
-	[`websphere-liberty:full`](#websphere-libertyfull)
-	[`websphere-liberty:full-java11-openj9`](#websphere-libertyfull-java11-openj9)
-	[`websphere-liberty:kernel`](#websphere-libertykernel)
-	[`websphere-liberty:kernel-java11-openj9`](#websphere-libertykernel-java11-openj9)
-	[`websphere-liberty:latest`](#websphere-libertylatest)

## `websphere-liberty:21.0.0.10-full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:f302e727de207af2774e2caad973a7bfeb9ee8ba516da456ea351e6a2807ce86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.10-full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:15feed4dc7fe993fe74f7e02fce21143cae99c216f53b6e166431cdef4efb951
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.0 MB (334021394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61e1afe72dcd950a54a6209229284c82128c471ef8fad65721b66261228bbedf`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:44:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 02:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 00:31:11 GMT
ENV JAVA_VERSION=jdk-11.0.13+8_openj9-0.29.0
# Thu, 28 Oct 2021 00:33:11 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='3615940d4b26e8d11ff927dbf620a5247caecd84ba24c9d67f0e8b30ff463998';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_ppc64le_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        s390x)          ESUM='e942c0806163bbabe0b7ec8e630319489da400d58cd390011fc28428f468558e';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_s390x_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        amd64|x86_64)          ESUM='78eb54af15fac39eb2d254f51f0302aa213d3ad838f17766a9d081ca783edff4';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_x64_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 28 Oct 2021 00:33:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 00:33:11 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 28 Oct 2021 00:33:47 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 28 Oct 2021 01:07:18 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:07:18 GMT
ARG OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:07:18 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Thu, 28 Oct 2021 01:07:19 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Thu, 28 Oct 2021 01:07:19 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Thu, 28 Oct 2021 01:07:19 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 28 Oct 2021 01:07:19 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Thu, 28 Oct 2021 01:07:19 GMT
ARG LIBERTY_URL
# Thu, 28 Oct 2021 01:07:19 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 28 Oct 2021 01:07:28 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 01:07:29 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 01:07:29 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Thu, 28 Oct 2021 01:07:29 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:07:30 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 28 Oct 2021 01:07:30 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Thu, 28 Oct 2021 01:07:30 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 28 Oct 2021 01:07:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 28 Oct 2021 01:07:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 28 Oct 2021 01:07:39 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 28 Oct 2021 01:07:39 GMT
USER 1001
# Thu, 28 Oct 2021 01:07:40 GMT
EXPOSE 9080 9443
# Thu, 28 Oct 2021 01:07:40 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 28 Oct 2021 01:07:40 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 28 Oct 2021 01:07:47 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:07:48 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 28 Oct 2021 01:10:50 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Thu, 28 Oct 2021 01:10:51 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 28 Oct 2021 01:11:27 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237daeb1ae282fe20092079ef6d5de7924746d0f2e9ad88797d08524a4d842fd`  
		Last Modified: Sat, 16 Oct 2021 02:47:20 GMT  
		Size: 16.0 MB (16036029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82607fdca83d197b118a35c377753995ef0400ef8de999ed3b8675d5fa58ce2f`  
		Last Modified: Thu, 28 Oct 2021 00:37:33 GMT  
		Size: 44.7 MB (44737093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7e4f4f21da9c3eec66f54b7ec452e3ccf00f68d74a7287bb1cbfbd68d2b041`  
		Last Modified: Thu, 28 Oct 2021 00:37:28 GMT  
		Size: 4.2 MB (4202694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f320c18438947d83dc1f15e75d6225b16e4030be2f3f60b723231f7d507fea`  
		Last Modified: Thu, 28 Oct 2021 01:20:39 GMT  
		Size: 14.2 MB (14171331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74f02207975af9dde28884f091d0c74f1c9360ecd847c1c009a8b0ed2033da3`  
		Last Modified: Thu, 28 Oct 2021 01:20:36 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478f97fe27905bdbf70a5179455b31a085d4398c4679c15e2f6c0e8fecbb9a58`  
		Last Modified: Thu, 28 Oct 2021 01:20:35 GMT  
		Size: 9.7 KB (9666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948ab830722710af86fa613d3fa37a082644901281103a071d74cebb6bd7a9ea`  
		Last Modified: Thu, 28 Oct 2021 01:20:35 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3379a5452b604a9a1debf912875f4ebd9f1e6e7cf9af825c2c4decde12d33d`  
		Last Modified: Thu, 28 Oct 2021 01:20:35 GMT  
		Size: 10.7 KB (10654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e1c3e8451879781f16eeb22bd489cb303f75fdd57586410b1682cd5680c4f4`  
		Last Modified: Thu, 28 Oct 2021 01:20:36 GMT  
		Size: 2.5 MB (2491575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2afc7dd7b2a11c2039016978a4e88ff295b2d5f6c887a29807539446c67791`  
		Last Modified: Thu, 28 Oct 2021 01:20:58 GMT  
		Size: 209.3 MB (209275582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8cb9274d195319b29b576a14b6f7e0c52ffa18af32e3ff3d7c81e22b204bbb`  
		Last Modified: Thu, 28 Oct 2021 01:20:47 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cec193b5ef149348342fe1d5bc3e439b7b840fb7d9e160ccae274082e717ca3`  
		Last Modified: Thu, 28 Oct 2021 01:20:49 GMT  
		Size: 14.5 MB (14517762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.10-full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:67adfadf6d017abdac145015162d86f601564d0d056f07900bbb4a36a366fa84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.9 MB (337874654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f9a4d56a09dd4e30cd54eddcbafad347cc4d0a64f5ea5a0c71547097c93f82a`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:54:47 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 00:55:56 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Oct 2021 01:45:21 GMT
ENV JAVA_VERSION=jdk-11.0.12+7_openj9-0.27.0
# Thu, 21 Oct 2021 01:48:48 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='285bd388a497db61408d26a9f3328f62004714ede94456718cf6440a109e25d2';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_ppc64le_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        s390x)          ESUM='6e5829aeb37abfb122e0944e438ecb2043c56df14fcdcce39bd4e3c9a55571a8';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_s390x_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        amd64|x86_64)          ESUM='f352998f6fdf0b84f63c563608be57f30aa3f14c8117c1219422dbc712ad4f81';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_x64_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 21 Oct 2021 01:49:04 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 21 Oct 2021 01:49:23 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 21 Oct 2021 01:50:18 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 26 Oct 2021 00:02:27 GMT
ARG VERBOSE=false
# Tue, 26 Oct 2021 00:02:29 GMT
ARG OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:02:31 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Tue, 26 Oct 2021 00:02:33 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Tue, 26 Oct 2021 00:02:34 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Tue, 26 Oct 2021 00:02:35 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 26 Oct 2021 00:02:37 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Tue, 26 Oct 2021 00:02:40 GMT
ARG LIBERTY_URL
# Tue, 26 Oct 2021 00:02:42 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 26 Oct 2021 00:03:11 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 26 Oct 2021 00:03:14 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 26 Oct 2021 00:03:18 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Tue, 26 Oct 2021 00:03:23 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:03:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 26 Oct 2021 00:03:39 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 26 Oct 2021 00:03:40 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 26 Oct 2021 00:03:50 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 26 Oct 2021 00:04:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 26 Oct 2021 00:04:11 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 26 Oct 2021 00:04:14 GMT
USER 1001
# Tue, 26 Oct 2021 00:04:16 GMT
EXPOSE 9080 9443
# Tue, 26 Oct 2021 00:04:17 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 26 Oct 2021 00:04:19 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 26 Oct 2021 00:09:47 GMT
ARG VERBOSE=false
# Tue, 26 Oct 2021 00:09:53 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 26 Oct 2021 00:13:55 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 26 Oct 2021 00:14:00 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 26 Oct 2021 00:14:54 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c930749dacf55e37561edab7967f5a2f51660034fee0da501c2d71cb783301`  
		Last Modified: Sat, 16 Oct 2021 01:03:26 GMT  
		Size: 17.2 MB (17210510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d519f9110a27224937cddf5826128ca092be8957e9a8c13546df0dc596ba42`  
		Last Modified: Thu, 21 Oct 2021 02:03:00 GMT  
		Size: 45.1 MB (45107808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afebfecbc9bc8dad01d6486a0e236777ff1b2a82229ff13363f70a0827f07160`  
		Last Modified: Thu, 21 Oct 2021 02:02:53 GMT  
		Size: 3.3 MB (3286490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c959c7913b358daa8d638d574cfed5c19cc6fb4779f71b43debea7cb425f78`  
		Last Modified: Tue, 26 Oct 2021 00:44:25 GMT  
		Size: 14.2 MB (14171675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29638a4016c15c1f7a42994d97fb39804a5d41ae894b550b1353eb6ac21f45fb`  
		Last Modified: Tue, 26 Oct 2021 00:44:20 GMT  
		Size: 690.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91b025d347f73e0851038db7723a694dc2c472341019140169aa25a378a59a2`  
		Last Modified: Tue, 26 Oct 2021 00:44:20 GMT  
		Size: 9.7 KB (9670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56be72fe50f64e22ae2d25ba9f167dc85452ab42662d744b9124903f45eaa5bf`  
		Last Modified: Tue, 26 Oct 2021 00:44:20 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7340186166530eddc6450a7abcdeb1b9eab34407a9beb4a6ed3c513a95ba810f`  
		Last Modified: Tue, 26 Oct 2021 00:44:20 GMT  
		Size: 10.7 KB (10658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28516018017a50371e38a72026e7e2899fe67161aedd2bc9d3368ed652d4ccec`  
		Last Modified: Tue, 26 Oct 2021 00:44:21 GMT  
		Size: 2.5 MB (2475923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462aa0189a031a7bbcb306ad930bb28d61963cee9e9950aa7b1947a276784f05`  
		Last Modified: Tue, 26 Oct 2021 00:45:23 GMT  
		Size: 209.3 MB (209276177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519107cecbb8c60717229b031939efbc424b885dc07311b09022dc099c11867a`  
		Last Modified: Tue, 26 Oct 2021 00:45:04 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcaaf51bdc0275b006bd24a8346913db391b8610d655368da5160487618a02f3`  
		Last Modified: Tue, 26 Oct 2021 00:45:07 GMT  
		Size: 13.0 MB (13036592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.10-full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:5253ca0dd20abc67573cfdeff50925fe9dd5599f50bcf349975eb598c12fa2f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.2 MB (331160402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23c05ce41ba5b2379e46381d07438a0c8e47ed3efb6dec86806ea2577bb7ce35`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:58:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 00:58:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 00:58:27 GMT
ENV JAVA_VERSION=jdk-11.0.13+8_openj9-0.29.0
# Thu, 28 Oct 2021 00:59:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='3615940d4b26e8d11ff927dbf620a5247caecd84ba24c9d67f0e8b30ff463998';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_ppc64le_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        s390x)          ESUM='e942c0806163bbabe0b7ec8e630319489da400d58cd390011fc28428f468558e';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_s390x_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        amd64|x86_64)          ESUM='78eb54af15fac39eb2d254f51f0302aa213d3ad838f17766a9d081ca783edff4';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_x64_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 28 Oct 2021 00:59:28 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 00:59:28 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 28 Oct 2021 01:00:01 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 28 Oct 2021 01:43:09 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:43:09 GMT
ARG OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:43:09 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Thu, 28 Oct 2021 01:43:09 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Thu, 28 Oct 2021 01:43:09 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Thu, 28 Oct 2021 01:43:09 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 28 Oct 2021 01:43:10 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Thu, 28 Oct 2021 01:43:10 GMT
ARG LIBERTY_URL
# Thu, 28 Oct 2021 01:43:10 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 28 Oct 2021 01:43:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 01:43:20 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 01:43:20 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Thu, 28 Oct 2021 01:43:20 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:43:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 28 Oct 2021 01:43:21 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Thu, 28 Oct 2021 01:43:21 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 28 Oct 2021 01:43:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 28 Oct 2021 01:43:26 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 28 Oct 2021 01:43:27 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 28 Oct 2021 01:43:27 GMT
USER 1001
# Thu, 28 Oct 2021 01:43:27 GMT
EXPOSE 9080 9443
# Thu, 28 Oct 2021 01:43:27 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 28 Oct 2021 01:43:27 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 28 Oct 2021 01:43:38 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:43:38 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 28 Oct 2021 01:47:03 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Thu, 28 Oct 2021 01:47:07 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 28 Oct 2021 01:47:29 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276dbe4459a060d2c186c43e5e92d98fa6f181617c55cce69da393b9d5dd6200`  
		Last Modified: Sat, 16 Oct 2021 01:01:03 GMT  
		Size: 15.7 MB (15742080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bef20936d077045a96f4b0694d1470b79e8825348eb06b3a0ef4207079d17d`  
		Last Modified: Thu, 28 Oct 2021 01:02:07 GMT  
		Size: 43.8 MB (43800069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8547dc44147bfe37bde98eef473a2916985469204db561ebefa3e3d92fee029a`  
		Last Modified: Thu, 28 Oct 2021 01:02:01 GMT  
		Size: 4.3 MB (4284720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8fe7f49f8a6320a829b59b87b8e6d2f5c623b8926fa5cbbd62cb3e14326e58`  
		Last Modified: Thu, 28 Oct 2021 01:58:02 GMT  
		Size: 14.2 MB (14170913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ea4b6d21bf75f5dc6643a5940ef5db23c15356b23f70a0adfcd0e80230ac8a`  
		Last Modified: Thu, 28 Oct 2021 01:57:59 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4198f3548e614a889bcf03b30adebe8652f6a27b339dde077ee4ebb8babfd2e`  
		Last Modified: Thu, 28 Oct 2021 01:57:59 GMT  
		Size: 9.7 KB (9668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633cdc0ee2e63d0df1b1e693ecf3947ca01f9c1843cd1e1f21d9b16958effdf5`  
		Last Modified: Thu, 28 Oct 2021 01:58:00 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57ec9e4f1b5721677f0cd7e5bd77c8d364c04bd78e96a528830486ebe9a74cf`  
		Last Modified: Thu, 28 Oct 2021 01:57:59 GMT  
		Size: 10.7 KB (10652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644a5090ddfa1106a57b25fe1251aa3af652c6bc002ed938c69efa8d13ceec86`  
		Last Modified: Thu, 28 Oct 2021 01:58:00 GMT  
		Size: 2.5 MB (2493018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ddccd96b1bcd0ef89a1fcfc003f8071e42ef47778717762b45abab0f749e6e`  
		Last Modified: Thu, 28 Oct 2021 01:58:23 GMT  
		Size: 209.3 MB (209276393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceff33fdbbf860efdae045e2fa402c1986f8eed375ec80cee3dd05c01974c68a`  
		Last Modified: Thu, 28 Oct 2021 01:58:09 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d506cfc35b6b1b727c4047c84da9292845ed6159ba6c2bcc939e06c10ea8a77`  
		Last Modified: Thu, 28 Oct 2021 01:58:11 GMT  
		Size: 14.3 MB (14250125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.10-full-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:33c296334c7ed9540a402f77a02eb5f383f4b3f07be7db1b687eddcaad4faa38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.10-full-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:b1115005499014bf1a10d5355e4d098ba6f4226783f08ea11272c326186fdd7f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.3 MB (403315070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf37216acf115eb9b9aff1a9f65dffc623e75c16a56cb1584bfd62ccf90a8094`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:55:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 02:55:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:55:32 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 02:56:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:56:08 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 01 Oct 2021 07:13:40 GMT
ARG VERBOSE=false
# Fri, 01 Oct 2021 07:13:40 GMT
ARG OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:39:24 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Mon, 25 Oct 2021 22:39:24 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Mon, 25 Oct 2021 22:39:24 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Mon, 25 Oct 2021 22:39:24 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 22:39:24 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Mon, 25 Oct 2021 22:39:25 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 22:39:25 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 25 Oct 2021 22:39:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 25 Oct 2021 22:39:42 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Oct 2021 22:39:42 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Mon, 25 Oct 2021 22:39:42 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:39:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 25 Oct 2021 22:39:44 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Mon, 25 Oct 2021 22:39:44 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 25 Oct 2021 22:39:45 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 25 Oct 2021 22:39:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 25 Oct 2021 22:39:58 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Mon, 25 Oct 2021 22:39:58 GMT
USER 1001
# Mon, 25 Oct 2021 22:39:59 GMT
EXPOSE 9080 9443
# Mon, 25 Oct 2021 22:39:59 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 25 Oct 2021 22:39:59 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Mon, 25 Oct 2021 22:40:32 GMT
ARG VERBOSE=false
# Mon, 25 Oct 2021 22:40:32 GMT
ARG REPOSITORIES_PROPERTIES=
# Mon, 25 Oct 2021 22:43:34 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Mon, 25 Oct 2021 22:43:35 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Mon, 25 Oct 2021 22:44:22 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf7ef5b4a4700901695d7489ffa25c9a36a0c54f7003664412a2a582dd362fa`  
		Last Modified: Fri, 01 Oct 2021 02:59:16 GMT  
		Size: 3.0 MB (2959872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58286f2e604db89582fc1898b2d2a229d5920927e7705c94e32f38a70e29902e`  
		Last Modified: Fri, 01 Oct 2021 02:59:26 GMT  
		Size: 128.4 MB (128395032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb130bd160d991d174701aa1d12d4c1f75c81705bd6ae5b036ae6e50a248d88e`  
		Last Modified: Mon, 25 Oct 2021 23:05:29 GMT  
		Size: 14.1 MB (14072794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7beabf2dd59365e93d8abbb027ae0f1b98d39e3ea91de31bded58a8c1f92448`  
		Last Modified: Mon, 25 Oct 2021 23:05:25 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f040313f6379bc9c04a2b94631e0bf2906ed5a99289186e898117021c507384`  
		Last Modified: Mon, 25 Oct 2021 23:05:26 GMT  
		Size: 9.7 KB (9677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fe7348629a8b7a683f0e06d11fd83be6b5349bfcecda69c0e3aac2d45ec8ae`  
		Last Modified: Mon, 25 Oct 2021 23:05:25 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054c2e49311baee037b9f9b7a4c1860cc61c840b03b81c38b83a63dac906a86d`  
		Last Modified: Mon, 25 Oct 2021 23:05:25 GMT  
		Size: 10.7 KB (10667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e464e836a01729d2494c3dc860e6e078d5d69fe1819cc5a4b8c9042c73d6a4`  
		Last Modified: Mon, 25 Oct 2021 23:05:26 GMT  
		Size: 5.9 MB (5869965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c845db47bbb20043cf2fd0baed54e15d4fdcc9659d3028b0d1ac7de9f87084f`  
		Last Modified: Mon, 25 Oct 2021 23:05:58 GMT  
		Size: 209.3 MB (209275727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c30de2c69d7ebc9cdb54e55b3d6a59437590a6fe6567f3bdf252ad06f6cd7d`  
		Last Modified: Mon, 25 Oct 2021 23:05:47 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b9160a1a04cb7a1afff92f9ceee48a39b1138f6751e1b860b52fe4e1c2236b`  
		Last Modified: Mon, 25 Oct 2021 23:05:49 GMT  
		Size: 16.0 MB (16014336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.10-full-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:3ebbd27afd1c227833f438d21f9636d883949eb2b952f08fdd6e0ba66b7dd4ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.0 MB (403966097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c78740a0ed156d7ac4d80645081da020f7c953c822c860f315773a5411af4e92`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 17:55:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Oct 2021 17:56:05 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 17:56:16 GMT
ENV JAVA_VERSION=8.0.6.36
# Wed, 06 Oct 2021 17:57:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Oct 2021 17:57:38 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 07 Oct 2021 10:35:31 GMT
ARG VERBOSE=false
# Thu, 07 Oct 2021 10:35:33 GMT
ARG OPENJ9_SCC=true
# Mon, 25 Oct 2021 23:59:34 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Mon, 25 Oct 2021 23:59:39 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Mon, 25 Oct 2021 23:59:43 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Mon, 25 Oct 2021 23:59:46 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 23:59:51 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Mon, 25 Oct 2021 23:59:54 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 23:59:57 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 26 Oct 2021 00:00:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 26 Oct 2021 00:00:59 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 26 Oct 2021 00:01:02 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Tue, 26 Oct 2021 00:01:07 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:01:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 26 Oct 2021 00:01:22 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 26 Oct 2021 00:01:23 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 26 Oct 2021 00:01:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 26 Oct 2021 00:01:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 26 Oct 2021 00:01:56 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 26 Oct 2021 00:01:59 GMT
USER 1001
# Tue, 26 Oct 2021 00:02:02 GMT
EXPOSE 9080 9443
# Tue, 26 Oct 2021 00:02:04 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 26 Oct 2021 00:02:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 26 Oct 2021 00:04:38 GMT
ARG VERBOSE=false
# Tue, 26 Oct 2021 00:04:41 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 26 Oct 2021 00:08:18 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 26 Oct 2021 00:08:26 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 26 Oct 2021 00:09:32 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce6e130fd3d09fd3fe6d741e0fa3f77120aa82717cf6d0a1cb49439939243a6`  
		Last Modified: Wed, 06 Oct 2021 18:04:08 GMT  
		Size: 3.1 MB (3081580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8fc8962750bc0e8c7c6ca6d1498e303c66e1f0b3f9613d204da9abf0200933`  
		Last Modified: Wed, 06 Oct 2021 18:04:22 GMT  
		Size: 127.9 MB (127898987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd371e52f22155313b0f3ae5f5c13597ca17fa0417c214eaf1e16df95bb678a8`  
		Last Modified: Tue, 26 Oct 2021 00:44:12 GMT  
		Size: 14.1 MB (14073366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee227af6d9277d187f05bd7fe3a7148fc127fd5be9bc040db19738760f9c12f`  
		Last Modified: Tue, 26 Oct 2021 00:44:08 GMT  
		Size: 697.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984133fc0355d34799cda371d5d2a8153e614767af49aa3cb7f8c98414e18950`  
		Last Modified: Tue, 26 Oct 2021 00:44:08 GMT  
		Size: 9.7 KB (9677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f9cacb1facc8e3097f176849d860aef3b7ebd23f9c9114047be96ca087ba97`  
		Last Modified: Tue, 26 Oct 2021 00:44:08 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfced5f1e31cfb68f3450e4211967c2c966cecdef7ccb633cb8a52a2c0cc710`  
		Last Modified: Tue, 26 Oct 2021 00:44:08 GMT  
		Size: 10.7 KB (10670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281fb76285f797555b5334b1d7f5596ec01e7137a6d55e8f31365b9fe39c2352`  
		Last Modified: Tue, 26 Oct 2021 00:44:09 GMT  
		Size: 5.3 MB (5339397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4562f8c3c1dade81475edf6207aea4f9c941c6b7c037c67810ebd4ee1c8098a3`  
		Last Modified: Tue, 26 Oct 2021 00:44:52 GMT  
		Size: 209.3 MB (209276516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09802a7cb8ad05d0191cf0a29e24e2e79b4306e2654390c0460db8311b15baa4`  
		Last Modified: Tue, 26 Oct 2021 00:44:33 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfae2d34298fb1bd2f919e6859a8e487b8d641e70379ba24107b763ad45558fe`  
		Last Modified: Tue, 26 Oct 2021 00:44:35 GMT  
		Size: 13.8 MB (13841061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.10-full-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:2456846170fe619056099175052bbc1115ade0e8a159250e76a21941cae6068d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.3 MB (398292262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed3ce5d13fb58bdf360ce6367ee827a0b76c2b099e4a24a7d693097f201d5545`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:17 GMT
ADD file:d248d4b5739ee5d07e920ec481dc4af81b314aa52e64618322197a642394a41d in / 
# Fri, 01 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:23:32 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 02:23:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:23:37 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 02:24:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:24:19 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 01 Oct 2021 03:40:55 GMT
ARG VERBOSE=false
# Fri, 01 Oct 2021 03:40:55 GMT
ARG OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:12:45 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Mon, 25 Oct 2021 22:12:45 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Mon, 25 Oct 2021 22:12:45 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Mon, 25 Oct 2021 22:12:45 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 22:12:45 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Mon, 25 Oct 2021 22:12:45 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 22:12:45 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 25 Oct 2021 22:12:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 25 Oct 2021 22:12:57 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Oct 2021 22:12:57 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Mon, 25 Oct 2021 22:12:57 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:12:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 25 Oct 2021 22:12:58 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Mon, 25 Oct 2021 22:12:58 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 25 Oct 2021 22:12:59 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 25 Oct 2021 22:13:06 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 25 Oct 2021 22:13:07 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Mon, 25 Oct 2021 22:13:07 GMT
USER 1001
# Mon, 25 Oct 2021 22:13:07 GMT
EXPOSE 9080 9443
# Mon, 25 Oct 2021 22:13:07 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 25 Oct 2021 22:13:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Mon, 25 Oct 2021 22:13:39 GMT
ARG VERBOSE=false
# Mon, 25 Oct 2021 22:13:40 GMT
ARG REPOSITORIES_PROPERTIES=
# Mon, 25 Oct 2021 22:17:03 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Mon, 25 Oct 2021 22:17:07 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Mon, 25 Oct 2021 22:17:31 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:97372e5b313b6b8bab9913de546bc50f73818d8275c94fc6491993c97b9d8bad`  
		Last Modified: Fri, 01 Oct 2021 01:43:49 GMT  
		Size: 25.4 MB (25362918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf425722012c2264c66ba97a53ff25a2f196330fbcc0872474e5e4562fa95f0`  
		Last Modified: Fri, 01 Oct 2021 02:27:43 GMT  
		Size: 2.7 MB (2676365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d432d8be662b9a55c0dfed6d79d328a62b58be822a9888d1b7d0d16dc6c248`  
		Last Modified: Fri, 01 Oct 2021 02:27:51 GMT  
		Size: 125.4 MB (125395531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969119abed0aabe761027277ec6fb7718eba553a1b072f7b1c13fbc7ad2643ce`  
		Last Modified: Mon, 25 Oct 2021 22:40:41 GMT  
		Size: 14.1 MB (14072637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6345425373ca667c20a30007a8292172e2b4eab13044ca41d184e4af52ff61e6`  
		Last Modified: Mon, 25 Oct 2021 22:40:39 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371f939cc39d32f824f40420cc6c72cee355cfa91155275e712b4632b2f7bc05`  
		Last Modified: Mon, 25 Oct 2021 22:40:39 GMT  
		Size: 9.7 KB (9674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f290e6c52139c0593dbbcd890fbc67f5b59bb711b97ea14886a2833a5a49ff93`  
		Last Modified: Mon, 25 Oct 2021 22:40:39 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4389715a5776e4d60e9b0bd807528101d253d83f6a4f2e5f9da17258ad41422c`  
		Last Modified: Mon, 25 Oct 2021 22:40:39 GMT  
		Size: 10.7 KB (10660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d732cb763586ba0cd58e22ae8ca4d3c4051b7370e0a5b974869d092a0d3a6b`  
		Last Modified: Mon, 25 Oct 2021 22:40:40 GMT  
		Size: 5.9 MB (5868523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3471c7e056a5f605febd60fea600313267b0f15c9c8449d042119817212638bb`  
		Last Modified: Mon, 25 Oct 2021 22:41:02 GMT  
		Size: 209.3 MB (209276442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb25227e9262c819dd066fb48ebfc7b4e86cfe76a0939caf9895ac2836c0531d`  
		Last Modified: Mon, 25 Oct 2021 22:40:53 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc404276fd2ceb3aac5a837f879edd92a65c6cdda45b95937e3ca3d7f1bd01c`  
		Last Modified: Mon, 25 Oct 2021 22:40:56 GMT  
		Size: 15.6 MB (15617590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.10-kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:68eca94c7794582aec5f5211dc28e7e494bbb30fb8aa4057655ba4d5af5ef770
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.10-kernel-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:f86373f06ed1a16f3e8881886fc5de954a53559713dc66340b1c3cc708963246
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110227106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf72306691ccc6f1e2cd442b72f3cd1d0e61d077bcec92a645cc9a3d2981ee9b`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:44:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 02:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 00:31:11 GMT
ENV JAVA_VERSION=jdk-11.0.13+8_openj9-0.29.0
# Thu, 28 Oct 2021 00:33:11 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='3615940d4b26e8d11ff927dbf620a5247caecd84ba24c9d67f0e8b30ff463998';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_ppc64le_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        s390x)          ESUM='e942c0806163bbabe0b7ec8e630319489da400d58cd390011fc28428f468558e';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_s390x_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        amd64|x86_64)          ESUM='78eb54af15fac39eb2d254f51f0302aa213d3ad838f17766a9d081ca783edff4';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_x64_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 28 Oct 2021 00:33:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 00:33:11 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 28 Oct 2021 00:33:47 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 28 Oct 2021 01:07:18 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:07:18 GMT
ARG OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:07:18 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Thu, 28 Oct 2021 01:07:19 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Thu, 28 Oct 2021 01:07:19 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Thu, 28 Oct 2021 01:07:19 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 28 Oct 2021 01:07:19 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Thu, 28 Oct 2021 01:07:19 GMT
ARG LIBERTY_URL
# Thu, 28 Oct 2021 01:07:19 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 28 Oct 2021 01:07:28 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 01:07:29 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 01:07:29 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Thu, 28 Oct 2021 01:07:29 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:07:30 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 28 Oct 2021 01:07:30 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Thu, 28 Oct 2021 01:07:30 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 28 Oct 2021 01:07:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 28 Oct 2021 01:07:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 28 Oct 2021 01:07:39 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 28 Oct 2021 01:07:39 GMT
USER 1001
# Thu, 28 Oct 2021 01:07:40 GMT
EXPOSE 9080 9443
# Thu, 28 Oct 2021 01:07:40 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 28 Oct 2021 01:07:40 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237daeb1ae282fe20092079ef6d5de7924746d0f2e9ad88797d08524a4d842fd`  
		Last Modified: Sat, 16 Oct 2021 02:47:20 GMT  
		Size: 16.0 MB (16036029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82607fdca83d197b118a35c377753995ef0400ef8de999ed3b8675d5fa58ce2f`  
		Last Modified: Thu, 28 Oct 2021 00:37:33 GMT  
		Size: 44.7 MB (44737093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7e4f4f21da9c3eec66f54b7ec452e3ccf00f68d74a7287bb1cbfbd68d2b041`  
		Last Modified: Thu, 28 Oct 2021 00:37:28 GMT  
		Size: 4.2 MB (4202694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f320c18438947d83dc1f15e75d6225b16e4030be2f3f60b723231f7d507fea`  
		Last Modified: Thu, 28 Oct 2021 01:20:39 GMT  
		Size: 14.2 MB (14171331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74f02207975af9dde28884f091d0c74f1c9360ecd847c1c009a8b0ed2033da3`  
		Last Modified: Thu, 28 Oct 2021 01:20:36 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478f97fe27905bdbf70a5179455b31a085d4398c4679c15e2f6c0e8fecbb9a58`  
		Last Modified: Thu, 28 Oct 2021 01:20:35 GMT  
		Size: 9.7 KB (9666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948ab830722710af86fa613d3fa37a082644901281103a071d74cebb6bd7a9ea`  
		Last Modified: Thu, 28 Oct 2021 01:20:35 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3379a5452b604a9a1debf912875f4ebd9f1e6e7cf9af825c2c4decde12d33d`  
		Last Modified: Thu, 28 Oct 2021 01:20:35 GMT  
		Size: 10.7 KB (10654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e1c3e8451879781f16eeb22bd489cb303f75fdd57586410b1682cd5680c4f4`  
		Last Modified: Thu, 28 Oct 2021 01:20:36 GMT  
		Size: 2.5 MB (2491575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.10-kernel-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:2501c8103e674cde4e96b7a89765c7eecae507e5a14c96e1a6e34f2e3d80fa55
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115560935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bb4841dc48174a8550e37905a79527f37536c9d4722e022a888004146d478c6`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:54:47 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 00:55:56 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Oct 2021 01:45:21 GMT
ENV JAVA_VERSION=jdk-11.0.12+7_openj9-0.27.0
# Thu, 21 Oct 2021 01:48:48 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='285bd388a497db61408d26a9f3328f62004714ede94456718cf6440a109e25d2';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_ppc64le_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        s390x)          ESUM='6e5829aeb37abfb122e0944e438ecb2043c56df14fcdcce39bd4e3c9a55571a8';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_s390x_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        amd64|x86_64)          ESUM='f352998f6fdf0b84f63c563608be57f30aa3f14c8117c1219422dbc712ad4f81';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_x64_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 21 Oct 2021 01:49:04 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 21 Oct 2021 01:49:23 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 21 Oct 2021 01:50:18 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 26 Oct 2021 00:02:27 GMT
ARG VERBOSE=false
# Tue, 26 Oct 2021 00:02:29 GMT
ARG OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:02:31 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Tue, 26 Oct 2021 00:02:33 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Tue, 26 Oct 2021 00:02:34 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Tue, 26 Oct 2021 00:02:35 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 26 Oct 2021 00:02:37 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Tue, 26 Oct 2021 00:02:40 GMT
ARG LIBERTY_URL
# Tue, 26 Oct 2021 00:02:42 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 26 Oct 2021 00:03:11 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 26 Oct 2021 00:03:14 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 26 Oct 2021 00:03:18 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Tue, 26 Oct 2021 00:03:23 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:03:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 26 Oct 2021 00:03:39 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 26 Oct 2021 00:03:40 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 26 Oct 2021 00:03:50 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 26 Oct 2021 00:04:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 26 Oct 2021 00:04:11 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 26 Oct 2021 00:04:14 GMT
USER 1001
# Tue, 26 Oct 2021 00:04:16 GMT
EXPOSE 9080 9443
# Tue, 26 Oct 2021 00:04:17 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 26 Oct 2021 00:04:19 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c930749dacf55e37561edab7967f5a2f51660034fee0da501c2d71cb783301`  
		Last Modified: Sat, 16 Oct 2021 01:03:26 GMT  
		Size: 17.2 MB (17210510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d519f9110a27224937cddf5826128ca092be8957e9a8c13546df0dc596ba42`  
		Last Modified: Thu, 21 Oct 2021 02:03:00 GMT  
		Size: 45.1 MB (45107808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afebfecbc9bc8dad01d6486a0e236777ff1b2a82229ff13363f70a0827f07160`  
		Last Modified: Thu, 21 Oct 2021 02:02:53 GMT  
		Size: 3.3 MB (3286490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c959c7913b358daa8d638d574cfed5c19cc6fb4779f71b43debea7cb425f78`  
		Last Modified: Tue, 26 Oct 2021 00:44:25 GMT  
		Size: 14.2 MB (14171675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29638a4016c15c1f7a42994d97fb39804a5d41ae894b550b1353eb6ac21f45fb`  
		Last Modified: Tue, 26 Oct 2021 00:44:20 GMT  
		Size: 690.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91b025d347f73e0851038db7723a694dc2c472341019140169aa25a378a59a2`  
		Last Modified: Tue, 26 Oct 2021 00:44:20 GMT  
		Size: 9.7 KB (9670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56be72fe50f64e22ae2d25ba9f167dc85452ab42662d744b9124903f45eaa5bf`  
		Last Modified: Tue, 26 Oct 2021 00:44:20 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7340186166530eddc6450a7abcdeb1b9eab34407a9beb4a6ed3c513a95ba810f`  
		Last Modified: Tue, 26 Oct 2021 00:44:20 GMT  
		Size: 10.7 KB (10658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28516018017a50371e38a72026e7e2899fe67161aedd2bc9d3368ed652d4ccec`  
		Last Modified: Tue, 26 Oct 2021 00:44:21 GMT  
		Size: 2.5 MB (2475923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.10-kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:da38ea19011c301b6927a7df2bd51ea85dcb3dc5e28278c4d314df21af5067ba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107632940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:030b09faee4fa1f3f5100082bbf2a954cf3e17b508408d1b1f6d36b813c26ca8`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:58:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 00:58:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 00:58:27 GMT
ENV JAVA_VERSION=jdk-11.0.13+8_openj9-0.29.0
# Thu, 28 Oct 2021 00:59:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='3615940d4b26e8d11ff927dbf620a5247caecd84ba24c9d67f0e8b30ff463998';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_ppc64le_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        s390x)          ESUM='e942c0806163bbabe0b7ec8e630319489da400d58cd390011fc28428f468558e';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_s390x_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        amd64|x86_64)          ESUM='78eb54af15fac39eb2d254f51f0302aa213d3ad838f17766a9d081ca783edff4';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_x64_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 28 Oct 2021 00:59:28 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 00:59:28 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 28 Oct 2021 01:00:01 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 28 Oct 2021 01:43:09 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:43:09 GMT
ARG OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:43:09 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Thu, 28 Oct 2021 01:43:09 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Thu, 28 Oct 2021 01:43:09 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Thu, 28 Oct 2021 01:43:09 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 28 Oct 2021 01:43:10 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Thu, 28 Oct 2021 01:43:10 GMT
ARG LIBERTY_URL
# Thu, 28 Oct 2021 01:43:10 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 28 Oct 2021 01:43:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 01:43:20 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 01:43:20 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Thu, 28 Oct 2021 01:43:20 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:43:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 28 Oct 2021 01:43:21 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Thu, 28 Oct 2021 01:43:21 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 28 Oct 2021 01:43:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 28 Oct 2021 01:43:26 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 28 Oct 2021 01:43:27 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 28 Oct 2021 01:43:27 GMT
USER 1001
# Thu, 28 Oct 2021 01:43:27 GMT
EXPOSE 9080 9443
# Thu, 28 Oct 2021 01:43:27 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 28 Oct 2021 01:43:27 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276dbe4459a060d2c186c43e5e92d98fa6f181617c55cce69da393b9d5dd6200`  
		Last Modified: Sat, 16 Oct 2021 01:01:03 GMT  
		Size: 15.7 MB (15742080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bef20936d077045a96f4b0694d1470b79e8825348eb06b3a0ef4207079d17d`  
		Last Modified: Thu, 28 Oct 2021 01:02:07 GMT  
		Size: 43.8 MB (43800069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8547dc44147bfe37bde98eef473a2916985469204db561ebefa3e3d92fee029a`  
		Last Modified: Thu, 28 Oct 2021 01:02:01 GMT  
		Size: 4.3 MB (4284720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8fe7f49f8a6320a829b59b87b8e6d2f5c623b8926fa5cbbd62cb3e14326e58`  
		Last Modified: Thu, 28 Oct 2021 01:58:02 GMT  
		Size: 14.2 MB (14170913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ea4b6d21bf75f5dc6643a5940ef5db23c15356b23f70a0adfcd0e80230ac8a`  
		Last Modified: Thu, 28 Oct 2021 01:57:59 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4198f3548e614a889bcf03b30adebe8652f6a27b339dde077ee4ebb8babfd2e`  
		Last Modified: Thu, 28 Oct 2021 01:57:59 GMT  
		Size: 9.7 KB (9668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633cdc0ee2e63d0df1b1e693ecf3947ca01f9c1843cd1e1f21d9b16958effdf5`  
		Last Modified: Thu, 28 Oct 2021 01:58:00 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57ec9e4f1b5721677f0cd7e5bd77c8d364c04bd78e96a528830486ebe9a74cf`  
		Last Modified: Thu, 28 Oct 2021 01:57:59 GMT  
		Size: 10.7 KB (10652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644a5090ddfa1106a57b25fe1251aa3af652c6bc002ed938c69efa8d13ceec86`  
		Last Modified: Thu, 28 Oct 2021 01:58:00 GMT  
		Size: 2.5 MB (2493018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.10-kernel-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:0da109d3e98329c7775b838cae83418391084908c0ca7d35f367275275808860
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.10-kernel-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:ee464c34f97bb768b4104598f3c1e0346bbce1d73048030b0ac77812c9489df9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.0 MB (178024060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:333e4a5e92a1e3e0601cebe2cb6d40eab384517ca9f3a497db31afde565b25d9`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:55:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 02:55:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:55:32 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 02:56:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:56:08 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 01 Oct 2021 07:13:40 GMT
ARG VERBOSE=false
# Fri, 01 Oct 2021 07:13:40 GMT
ARG OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:39:24 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Mon, 25 Oct 2021 22:39:24 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Mon, 25 Oct 2021 22:39:24 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Mon, 25 Oct 2021 22:39:24 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 22:39:24 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Mon, 25 Oct 2021 22:39:25 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 22:39:25 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 25 Oct 2021 22:39:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 25 Oct 2021 22:39:42 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Oct 2021 22:39:42 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Mon, 25 Oct 2021 22:39:42 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:39:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 25 Oct 2021 22:39:44 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Mon, 25 Oct 2021 22:39:44 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 25 Oct 2021 22:39:45 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 25 Oct 2021 22:39:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 25 Oct 2021 22:39:58 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Mon, 25 Oct 2021 22:39:58 GMT
USER 1001
# Mon, 25 Oct 2021 22:39:59 GMT
EXPOSE 9080 9443
# Mon, 25 Oct 2021 22:39:59 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 25 Oct 2021 22:39:59 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf7ef5b4a4700901695d7489ffa25c9a36a0c54f7003664412a2a582dd362fa`  
		Last Modified: Fri, 01 Oct 2021 02:59:16 GMT  
		Size: 3.0 MB (2959872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58286f2e604db89582fc1898b2d2a229d5920927e7705c94e32f38a70e29902e`  
		Last Modified: Fri, 01 Oct 2021 02:59:26 GMT  
		Size: 128.4 MB (128395032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb130bd160d991d174701aa1d12d4c1f75c81705bd6ae5b036ae6e50a248d88e`  
		Last Modified: Mon, 25 Oct 2021 23:05:29 GMT  
		Size: 14.1 MB (14072794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7beabf2dd59365e93d8abbb027ae0f1b98d39e3ea91de31bded58a8c1f92448`  
		Last Modified: Mon, 25 Oct 2021 23:05:25 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f040313f6379bc9c04a2b94631e0bf2906ed5a99289186e898117021c507384`  
		Last Modified: Mon, 25 Oct 2021 23:05:26 GMT  
		Size: 9.7 KB (9677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fe7348629a8b7a683f0e06d11fd83be6b5349bfcecda69c0e3aac2d45ec8ae`  
		Last Modified: Mon, 25 Oct 2021 23:05:25 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054c2e49311baee037b9f9b7a4c1860cc61c840b03b81c38b83a63dac906a86d`  
		Last Modified: Mon, 25 Oct 2021 23:05:25 GMT  
		Size: 10.7 KB (10667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e464e836a01729d2494c3dc860e6e078d5d69fe1819cc5a4b8c9042c73d6a4`  
		Last Modified: Mon, 25 Oct 2021 23:05:26 GMT  
		Size: 5.9 MB (5869965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.10-kernel-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:25ca6bf0c3ee273a34363059fcd67f58b41431e117a6ca0534ddb60eec70b18a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.8 MB (180847570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fb086abfd307b5aa8180d3eeb31548f2b856d9885bfdceeabdce3e72e714f77`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 17:55:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Oct 2021 17:56:05 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 17:56:16 GMT
ENV JAVA_VERSION=8.0.6.36
# Wed, 06 Oct 2021 17:57:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Oct 2021 17:57:38 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 07 Oct 2021 10:35:31 GMT
ARG VERBOSE=false
# Thu, 07 Oct 2021 10:35:33 GMT
ARG OPENJ9_SCC=true
# Mon, 25 Oct 2021 23:59:34 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Mon, 25 Oct 2021 23:59:39 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Mon, 25 Oct 2021 23:59:43 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Mon, 25 Oct 2021 23:59:46 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 23:59:51 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Mon, 25 Oct 2021 23:59:54 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 23:59:57 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 26 Oct 2021 00:00:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 26 Oct 2021 00:00:59 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 26 Oct 2021 00:01:02 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Tue, 26 Oct 2021 00:01:07 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:01:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 26 Oct 2021 00:01:22 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 26 Oct 2021 00:01:23 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 26 Oct 2021 00:01:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 26 Oct 2021 00:01:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 26 Oct 2021 00:01:56 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 26 Oct 2021 00:01:59 GMT
USER 1001
# Tue, 26 Oct 2021 00:02:02 GMT
EXPOSE 9080 9443
# Tue, 26 Oct 2021 00:02:04 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 26 Oct 2021 00:02:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce6e130fd3d09fd3fe6d741e0fa3f77120aa82717cf6d0a1cb49439939243a6`  
		Last Modified: Wed, 06 Oct 2021 18:04:08 GMT  
		Size: 3.1 MB (3081580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8fc8962750bc0e8c7c6ca6d1498e303c66e1f0b3f9613d204da9abf0200933`  
		Last Modified: Wed, 06 Oct 2021 18:04:22 GMT  
		Size: 127.9 MB (127898987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd371e52f22155313b0f3ae5f5c13597ca17fa0417c214eaf1e16df95bb678a8`  
		Last Modified: Tue, 26 Oct 2021 00:44:12 GMT  
		Size: 14.1 MB (14073366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee227af6d9277d187f05bd7fe3a7148fc127fd5be9bc040db19738760f9c12f`  
		Last Modified: Tue, 26 Oct 2021 00:44:08 GMT  
		Size: 697.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984133fc0355d34799cda371d5d2a8153e614767af49aa3cb7f8c98414e18950`  
		Last Modified: Tue, 26 Oct 2021 00:44:08 GMT  
		Size: 9.7 KB (9677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f9cacb1facc8e3097f176849d860aef3b7ebd23f9c9114047be96ca087ba97`  
		Last Modified: Tue, 26 Oct 2021 00:44:08 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfced5f1e31cfb68f3450e4211967c2c966cecdef7ccb633cb8a52a2c0cc710`  
		Last Modified: Tue, 26 Oct 2021 00:44:08 GMT  
		Size: 10.7 KB (10670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281fb76285f797555b5334b1d7f5596ec01e7137a6d55e8f31365b9fe39c2352`  
		Last Modified: Tue, 26 Oct 2021 00:44:09 GMT  
		Size: 5.3 MB (5339397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.10-kernel-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:06e38d016a5cebe53ca6fcd2e1e2072b96beed8b72eea08d9f54241d4d0c9cd5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.4 MB (173397283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab4fe7318aca4b94aa29bbde69e8cb5286b94a4f7a8073256f30c13c1c0e570a`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:17 GMT
ADD file:d248d4b5739ee5d07e920ec481dc4af81b314aa52e64618322197a642394a41d in / 
# Fri, 01 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:23:32 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 02:23:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:23:37 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 02:24:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:24:19 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 01 Oct 2021 03:40:55 GMT
ARG VERBOSE=false
# Fri, 01 Oct 2021 03:40:55 GMT
ARG OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:12:45 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Mon, 25 Oct 2021 22:12:45 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Mon, 25 Oct 2021 22:12:45 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Mon, 25 Oct 2021 22:12:45 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 22:12:45 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Mon, 25 Oct 2021 22:12:45 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 22:12:45 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 25 Oct 2021 22:12:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 25 Oct 2021 22:12:57 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Oct 2021 22:12:57 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Mon, 25 Oct 2021 22:12:57 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:12:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 25 Oct 2021 22:12:58 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Mon, 25 Oct 2021 22:12:58 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 25 Oct 2021 22:12:59 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 25 Oct 2021 22:13:06 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 25 Oct 2021 22:13:07 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Mon, 25 Oct 2021 22:13:07 GMT
USER 1001
# Mon, 25 Oct 2021 22:13:07 GMT
EXPOSE 9080 9443
# Mon, 25 Oct 2021 22:13:07 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 25 Oct 2021 22:13:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:97372e5b313b6b8bab9913de546bc50f73818d8275c94fc6491993c97b9d8bad`  
		Last Modified: Fri, 01 Oct 2021 01:43:49 GMT  
		Size: 25.4 MB (25362918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf425722012c2264c66ba97a53ff25a2f196330fbcc0872474e5e4562fa95f0`  
		Last Modified: Fri, 01 Oct 2021 02:27:43 GMT  
		Size: 2.7 MB (2676365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d432d8be662b9a55c0dfed6d79d328a62b58be822a9888d1b7d0d16dc6c248`  
		Last Modified: Fri, 01 Oct 2021 02:27:51 GMT  
		Size: 125.4 MB (125395531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969119abed0aabe761027277ec6fb7718eba553a1b072f7b1c13fbc7ad2643ce`  
		Last Modified: Mon, 25 Oct 2021 22:40:41 GMT  
		Size: 14.1 MB (14072637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6345425373ca667c20a30007a8292172e2b4eab13044ca41d184e4af52ff61e6`  
		Last Modified: Mon, 25 Oct 2021 22:40:39 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371f939cc39d32f824f40420cc6c72cee355cfa91155275e712b4632b2f7bc05`  
		Last Modified: Mon, 25 Oct 2021 22:40:39 GMT  
		Size: 9.7 KB (9674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f290e6c52139c0593dbbcd890fbc67f5b59bb711b97ea14886a2833a5a49ff93`  
		Last Modified: Mon, 25 Oct 2021 22:40:39 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4389715a5776e4d60e9b0bd807528101d253d83f6a4f2e5f9da17258ad41422c`  
		Last Modified: Mon, 25 Oct 2021 22:40:39 GMT  
		Size: 10.7 KB (10660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d732cb763586ba0cd58e22ae8ca4d3c4051b7370e0a5b974869d092a0d3a6b`  
		Last Modified: Mon, 25 Oct 2021 22:40:40 GMT  
		Size: 5.9 MB (5868523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.6-full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:2d48571b2ff5f90ddf26d2f39e6e74d8e48936816d660bd32546de42d21623c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.6-full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:9538654c2e39c6a61f9e84cfcefa7ae9b35e5b5c2f01adbd0ffd690b61ababad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.6 MB (332645643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fb833425c34b2ad4f1822e5a8bf9060a0419a4f99acece84c477e2161968060`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:44:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 02:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 00:31:11 GMT
ENV JAVA_VERSION=jdk-11.0.13+8_openj9-0.29.0
# Thu, 28 Oct 2021 00:33:11 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='3615940d4b26e8d11ff927dbf620a5247caecd84ba24c9d67f0e8b30ff463998';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_ppc64le_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        s390x)          ESUM='e942c0806163bbabe0b7ec8e630319489da400d58cd390011fc28428f468558e';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_s390x_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        amd64|x86_64)          ESUM='78eb54af15fac39eb2d254f51f0302aa213d3ad838f17766a9d081ca783edff4';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_x64_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 28 Oct 2021 00:33:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 00:33:11 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 28 Oct 2021 00:33:47 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 28 Oct 2021 01:07:18 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:07:18 GMT
ARG OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:15:53 GMT
ARG EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27
# Thu, 28 Oct 2021 01:15:53 GMT
ARG NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c
# Thu, 28 Oct 2021 01:15:53 GMT
ARG NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499
# Thu, 28 Oct 2021 01:15:53 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.6 org.opencontainers.image.revision=cl210620210527-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 28 Oct 2021 01:15:53 GMT
ENV LIBERTY_VERSION=21.0.0_06
# Thu, 28 Oct 2021 01:15:53 GMT
ARG LIBERTY_URL
# Thu, 28 Oct 2021 01:15:54 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 28 Oct 2021 01:16:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 01:16:03 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 01:16:03 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.6 BuildLabel=cl210620210527-1900
# Thu, 28 Oct 2021 01:16:03 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:16:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 28 Oct 2021 01:16:04 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Thu, 28 Oct 2021 01:16:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 28 Oct 2021 01:16:05 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 28 Oct 2021 01:16:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 28 Oct 2021 01:16:13 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 28 Oct 2021 01:16:14 GMT
USER 1001
# Thu, 28 Oct 2021 01:16:14 GMT
EXPOSE 9080 9443
# Thu, 28 Oct 2021 01:16:14 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 28 Oct 2021 01:16:14 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 28 Oct 2021 01:16:22 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:16:22 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 28 Oct 2021 01:19:24 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Thu, 28 Oct 2021 01:19:25 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 28 Oct 2021 01:20:01 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237daeb1ae282fe20092079ef6d5de7924746d0f2e9ad88797d08524a4d842fd`  
		Last Modified: Sat, 16 Oct 2021 02:47:20 GMT  
		Size: 16.0 MB (16036029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82607fdca83d197b118a35c377753995ef0400ef8de999ed3b8675d5fa58ce2f`  
		Last Modified: Thu, 28 Oct 2021 00:37:33 GMT  
		Size: 44.7 MB (44737093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7e4f4f21da9c3eec66f54b7ec452e3ccf00f68d74a7287bb1cbfbd68d2b041`  
		Last Modified: Thu, 28 Oct 2021 00:37:28 GMT  
		Size: 4.2 MB (4202694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6622e397e6bb51d9dc37e6dd0cf22ab476ef4c2e3c709c1f57f962a43c362881`  
		Last Modified: Thu, 28 Oct 2021 01:21:47 GMT  
		Size: 14.2 MB (14170433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65d10d381b726b348f861449ca2fe65ac55cfaf9324af07fe6670c997112924`  
		Last Modified: Thu, 28 Oct 2021 01:21:44 GMT  
		Size: 688.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6269d7e59287ca1196e4bd0c947d44b2f939048b335f77425dd62df101e15e8`  
		Last Modified: Thu, 28 Oct 2021 01:21:44 GMT  
		Size: 9.7 KB (9667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80755773242e268fd352271869ea66c6fa74cabb950e252a372f8cd67573a94`  
		Last Modified: Thu, 28 Oct 2021 01:21:44 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e49ff4c5091e2cc2b48066e7a89c36959148d58c6411f1c727851a1ff9367e8`  
		Last Modified: Thu, 28 Oct 2021 01:21:44 GMT  
		Size: 10.6 KB (10647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156a38b10d4279e3561c50812c97c992cb04d5e44fd719483b0b509cacbc36f7`  
		Last Modified: Thu, 28 Oct 2021 01:21:44 GMT  
		Size: 2.5 MB (2523559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198298622ba2b65af28abc84868b3500e1a4455e6329ecc6d5dfe7416bb49f40`  
		Last Modified: Thu, 28 Oct 2021 01:22:06 GMT  
		Size: 207.8 MB (207777364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb5704bc96ea4eb214c3095e6bdce00ba4d92cd8055c56b644104fc2c57b760`  
		Last Modified: Thu, 28 Oct 2021 01:21:55 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5768dd8b617b089c6697147c235fbca79abf7de062b56a5a0b249a633d965f`  
		Last Modified: Thu, 28 Oct 2021 01:21:57 GMT  
		Size: 14.6 MB (14609156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.6-full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:521146ac5129f57a301d0965bbd9ba93549065f83dda877216a42bcab1ca6262
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.7 MB (335748210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ced34354047fe1a2cc9514aba2564decf3e6f4658bf9817404215ed9e0d3f0a`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:54:47 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 00:55:56 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Oct 2021 01:45:21 GMT
ENV JAVA_VERSION=jdk-11.0.12+7_openj9-0.27.0
# Thu, 21 Oct 2021 01:48:48 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='285bd388a497db61408d26a9f3328f62004714ede94456718cf6440a109e25d2';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_ppc64le_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        s390x)          ESUM='6e5829aeb37abfb122e0944e438ecb2043c56df14fcdcce39bd4e3c9a55571a8';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_s390x_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        amd64|x86_64)          ESUM='f352998f6fdf0b84f63c563608be57f30aa3f14c8117c1219422dbc712ad4f81';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_x64_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 21 Oct 2021 01:49:04 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 21 Oct 2021 01:49:23 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 21 Oct 2021 01:50:18 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 26 Oct 2021 00:02:27 GMT
ARG VERBOSE=false
# Tue, 26 Oct 2021 00:02:29 GMT
ARG OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:31:36 GMT
ARG EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27
# Tue, 26 Oct 2021 00:31:43 GMT
ARG NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c
# Tue, 26 Oct 2021 00:31:45 GMT
ARG NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499
# Tue, 26 Oct 2021 00:31:48 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.6 org.opencontainers.image.revision=cl210620210527-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 26 Oct 2021 00:31:51 GMT
ENV LIBERTY_VERSION=21.0.0_06
# Tue, 26 Oct 2021 00:31:53 GMT
ARG LIBERTY_URL
# Tue, 26 Oct 2021 00:31:57 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 26 Oct 2021 00:32:25 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 26 Oct 2021 00:32:28 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 26 Oct 2021 00:32:32 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.6 BuildLabel=cl210620210527-1900
# Tue, 26 Oct 2021 00:32:34 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:32:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 26 Oct 2021 00:32:42 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 26 Oct 2021 00:32:44 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 26 Oct 2021 00:32:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 26 Oct 2021 00:33:14 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 26 Oct 2021 00:33:17 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 26 Oct 2021 00:33:19 GMT
USER 1001
# Tue, 26 Oct 2021 00:33:21 GMT
EXPOSE 9080 9443
# Tue, 26 Oct 2021 00:33:24 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 26 Oct 2021 00:33:27 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 26 Oct 2021 00:38:42 GMT
ARG VERBOSE=false
# Tue, 26 Oct 2021 00:38:47 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 26 Oct 2021 00:42:12 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 26 Oct 2021 00:42:18 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 26 Oct 2021 00:43:10 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c930749dacf55e37561edab7967f5a2f51660034fee0da501c2d71cb783301`  
		Last Modified: Sat, 16 Oct 2021 01:03:26 GMT  
		Size: 17.2 MB (17210510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d519f9110a27224937cddf5826128ca092be8957e9a8c13546df0dc596ba42`  
		Last Modified: Thu, 21 Oct 2021 02:03:00 GMT  
		Size: 45.1 MB (45107808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afebfecbc9bc8dad01d6486a0e236777ff1b2a82229ff13363f70a0827f07160`  
		Last Modified: Thu, 21 Oct 2021 02:02:53 GMT  
		Size: 3.3 MB (3286490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe9e25c140c6be09f6231808fc81e0efa6ed5ae38417ee0eca62564eabfc0a1`  
		Last Modified: Tue, 26 Oct 2021 00:47:21 GMT  
		Size: 14.2 MB (14170401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a96545a202495b9b4cdba4fa2d2b3f182e19d514c664a660f46b5650d4c77b8`  
		Last Modified: Tue, 26 Oct 2021 00:47:17 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d95fb332deaa47f41089f51b9a15535796a7b90829bc2253c5cb5fe6a9201be`  
		Last Modified: Tue, 26 Oct 2021 00:47:17 GMT  
		Size: 9.7 KB (9668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8d576ea60b888dd5893cf254a9bae933f86ce585acc11aa578b4c0fb16af26`  
		Last Modified: Tue, 26 Oct 2021 00:47:17 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3ff933d15821edff36a5ee5010094877ef4c98265e1f4601a1fe981ecc7edd`  
		Last Modified: Tue, 26 Oct 2021 00:47:17 GMT  
		Size: 10.6 KB (10646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aaa52636908415eb3d38c289800ec6ecc3315827d8abdeb909dc1004e67d06f`  
		Last Modified: Tue, 26 Oct 2021 00:47:17 GMT  
		Size: 2.5 MB (2460238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79666f41c054a80a9e19e10caf7d54712b5bbf9170c69af6f86e0f34f4202b04`  
		Last Modified: Tue, 26 Oct 2021 00:48:14 GMT  
		Size: 207.8 MB (207777540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79655cbfa389f3ba1937337c6ada920653d13b38cdd33249c05c1603b2c3c179`  
		Last Modified: Tue, 26 Oct 2021 00:47:56 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19a61e6d52e4074e17e8f9a7069c612948265a42590a4ffdac717e98207b86e`  
		Last Modified: Tue, 26 Oct 2021 00:47:59 GMT  
		Size: 12.4 MB (12425763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.6-full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:a46ff475c5ee06c1ca235f1bf61f72add19c527a4ab90356ebc9e7d5e7df4fa1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.7 MB (329681658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e1b5470f48921e8ca3c2b401a0b30eb5784860626dbb3f9525a6741e6ba618b`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:58:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 00:58:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 00:58:27 GMT
ENV JAVA_VERSION=jdk-11.0.13+8_openj9-0.29.0
# Thu, 28 Oct 2021 00:59:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='3615940d4b26e8d11ff927dbf620a5247caecd84ba24c9d67f0e8b30ff463998';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_ppc64le_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        s390x)          ESUM='e942c0806163bbabe0b7ec8e630319489da400d58cd390011fc28428f468558e';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_s390x_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        amd64|x86_64)          ESUM='78eb54af15fac39eb2d254f51f0302aa213d3ad838f17766a9d081ca783edff4';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_x64_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 28 Oct 2021 00:59:28 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 00:59:28 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 28 Oct 2021 01:00:01 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 28 Oct 2021 01:43:09 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:43:09 GMT
ARG OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:52:46 GMT
ARG EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27
# Thu, 28 Oct 2021 01:52:46 GMT
ARG NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c
# Thu, 28 Oct 2021 01:52:46 GMT
ARG NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499
# Thu, 28 Oct 2021 01:52:46 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.6 org.opencontainers.image.revision=cl210620210527-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 28 Oct 2021 01:52:46 GMT
ENV LIBERTY_VERSION=21.0.0_06
# Thu, 28 Oct 2021 01:52:46 GMT
ARG LIBERTY_URL
# Thu, 28 Oct 2021 01:52:46 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 28 Oct 2021 01:52:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 01:52:55 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 01:52:55 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.6 BuildLabel=cl210620210527-1900
# Thu, 28 Oct 2021 01:52:55 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:52:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 28 Oct 2021 01:52:56 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Thu, 28 Oct 2021 01:52:56 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 28 Oct 2021 01:52:57 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 28 Oct 2021 01:53:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 28 Oct 2021 01:53:02 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 28 Oct 2021 01:53:02 GMT
USER 1001
# Thu, 28 Oct 2021 01:53:02 GMT
EXPOSE 9080 9443
# Thu, 28 Oct 2021 01:53:02 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 28 Oct 2021 01:53:02 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 28 Oct 2021 01:53:14 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:53:14 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 28 Oct 2021 01:56:40 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Thu, 28 Oct 2021 01:56:44 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 28 Oct 2021 01:57:07 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276dbe4459a060d2c186c43e5e92d98fa6f181617c55cce69da393b9d5dd6200`  
		Last Modified: Sat, 16 Oct 2021 01:01:03 GMT  
		Size: 15.7 MB (15742080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bef20936d077045a96f4b0694d1470b79e8825348eb06b3a0ef4207079d17d`  
		Last Modified: Thu, 28 Oct 2021 01:02:07 GMT  
		Size: 43.8 MB (43800069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8547dc44147bfe37bde98eef473a2916985469204db561ebefa3e3d92fee029a`  
		Last Modified: Thu, 28 Oct 2021 01:02:01 GMT  
		Size: 4.3 MB (4284720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c6269035de2a2ae68251fef891100b4f90d848cc7e5756129ed2a129490710`  
		Last Modified: Thu, 28 Oct 2021 01:59:04 GMT  
		Size: 14.2 MB (14170121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba336883ee9b632b0619412eaf3badde28f6055015167ab3fff29e1858a3cd9`  
		Last Modified: Thu, 28 Oct 2021 01:59:02 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c851801448baa7051180bce048eed67e287409df1ad4357ba8b44b0161885e`  
		Last Modified: Thu, 28 Oct 2021 01:59:02 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a59076e80744480249879a4a6bb1cdbe4df35dda41c76dc718555a0dc2845ec`  
		Last Modified: Thu, 28 Oct 2021 01:59:02 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e54b1669e7c95c2e98d837805135fbe24a09de022fdc4ac94e09280da43bf0c`  
		Last Modified: Thu, 28 Oct 2021 01:59:02 GMT  
		Size: 10.6 KB (10647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a70b8437e2349f6453d71474ae0e76ee6afa42fccd0cabff0cefe9ef5118008`  
		Last Modified: Thu, 28 Oct 2021 01:59:02 GMT  
		Size: 2.5 MB (2503840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e60848b6ceaf7567a9a6427e338aa88929b5e50f8c2362c0d463ebf43694115`  
		Last Modified: Thu, 28 Oct 2021 01:59:22 GMT  
		Size: 207.8 MB (207777488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a000a4c9a49e6d483234b8c7a8c6355cb7da81298db01be4b10e170a6e6b9d`  
		Last Modified: Thu, 28 Oct 2021 01:59:10 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ff386cdf6f4b3f5994138ac471b5fa3fc1ce498ea5d1930151f798930bc21f`  
		Last Modified: Thu, 28 Oct 2021 01:59:12 GMT  
		Size: 14.3 MB (14260260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.6-full-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:a8e3ecf4ac9925f747a64ce6589d3854bd5430798922c285ed734662de20f820
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.6-full-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:0cbe8103c8e99f5971224e57b96e4bd4a65a65e8025c989971ea0bb1eaaae686
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **401.7 MB (401743010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03e58b5683eb84ba51b289c892f14849fe4195d639ff846bbc5a9572aa45ba66`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:55:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 02:55:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:55:32 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 02:56:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:56:08 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 01 Oct 2021 07:13:40 GMT
ARG VERBOSE=false
# Fri, 01 Oct 2021 07:13:40 GMT
ARG OPENJ9_SCC=true
# Fri, 01 Oct 2021 07:22:40 GMT
ARG EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27
# Fri, 01 Oct 2021 07:22:40 GMT
ARG NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c
# Fri, 01 Oct 2021 07:22:40 GMT
ARG NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499
# Mon, 25 Oct 2021 22:56:59 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.6 org.opencontainers.image.revision=cl210620210527-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 22:56:59 GMT
ENV LIBERTY_VERSION=21.0.0_06
# Mon, 25 Oct 2021 22:56:59 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 22:57:00 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 25 Oct 2021 22:57:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 25 Oct 2021 22:57:11 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Oct 2021 22:57:11 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.6 BuildLabel=cl210620210527-1900
# Mon, 25 Oct 2021 22:57:11 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:57:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 25 Oct 2021 22:57:13 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Mon, 25 Oct 2021 22:57:13 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 25 Oct 2021 22:57:14 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 25 Oct 2021 22:57:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 25 Oct 2021 22:57:23 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Mon, 25 Oct 2021 22:57:24 GMT
USER 1001
# Mon, 25 Oct 2021 22:57:24 GMT
EXPOSE 9080 9443
# Mon, 25 Oct 2021 22:57:24 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 25 Oct 2021 22:57:24 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Mon, 25 Oct 2021 22:57:50 GMT
ARG VERBOSE=false
# Mon, 25 Oct 2021 22:57:50 GMT
ARG REPOSITORIES_PROPERTIES=
# Mon, 25 Oct 2021 23:00:42 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Mon, 25 Oct 2021 23:00:43 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Mon, 25 Oct 2021 23:01:20 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf7ef5b4a4700901695d7489ffa25c9a36a0c54f7003664412a2a582dd362fa`  
		Last Modified: Fri, 01 Oct 2021 02:59:16 GMT  
		Size: 3.0 MB (2959872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58286f2e604db89582fc1898b2d2a229d5920927e7705c94e32f38a70e29902e`  
		Last Modified: Fri, 01 Oct 2021 02:59:26 GMT  
		Size: 128.4 MB (128395032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d9b3674446553288745201810a45b12d455d60f25fb7781c189fe1cd0df6a5`  
		Last Modified: Mon, 25 Oct 2021 23:07:41 GMT  
		Size: 14.1 MB (14073331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16336408a8e380e3f541c8020aee3f513b5e69e5a18233507df6cdd22a1fc0e5`  
		Last Modified: Mon, 25 Oct 2021 23:07:37 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459d0261a5ac122d0ca1631812f6dd203aa20559e524b6ea85f661c58e42f6a4`  
		Last Modified: Mon, 25 Oct 2021 23:07:38 GMT  
		Size: 9.7 KB (9676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b86b60ee9345ab1aba1cb3dbf0de1548f32c8bc3dd40eca65e7a65ad0b891b8`  
		Last Modified: Mon, 25 Oct 2021 23:07:37 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f003a342b48d85a24addcdd8ab33c372650b227b88b03a544adf6da569b5f4`  
		Last Modified: Mon, 25 Oct 2021 23:07:37 GMT  
		Size: 10.7 KB (10656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d36ee135e799a38aafcb6546d0b445a5985a3512685c6842c25c2d59677a79`  
		Last Modified: Mon, 25 Oct 2021 23:07:38 GMT  
		Size: 5.8 MB (5768773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ba3f7b3566f20cb1e8c829baf1f80e6b2d77963ea3f86ce275fec8fcfc50d9`  
		Last Modified: Mon, 25 Oct 2021 23:08:09 GMT  
		Size: 207.8 MB (207777431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49720694ae2e5e274f833d173addfa79dfb5c6d9000567fd10d9f8199e2691b8`  
		Last Modified: Mon, 25 Oct 2021 23:07:57 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c68634af56080de048fcb827270c92e7c0bba6789e8d6fd26e730159f1cd7f`  
		Last Modified: Mon, 25 Oct 2021 23:08:00 GMT  
		Size: 16.0 MB (16041243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.6-full-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:5452dcc6ece32878fdf57b707084badc2cfed51c96cb55dcd7d2ecea62629c9e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.1 MB (402074302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b0b2c1013111ab87dc99d0388eda6d9a23329eaffd9d812c7d1e0e9126e6606`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 17:55:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Oct 2021 17:56:05 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 17:56:16 GMT
ENV JAVA_VERSION=8.0.6.36
# Wed, 06 Oct 2021 17:57:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Oct 2021 17:57:38 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 07 Oct 2021 10:35:31 GMT
ARG VERBOSE=false
# Thu, 07 Oct 2021 10:35:33 GMT
ARG OPENJ9_SCC=true
# Thu, 07 Oct 2021 10:53:29 GMT
ARG EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27
# Thu, 07 Oct 2021 10:53:34 GMT
ARG NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c
# Thu, 07 Oct 2021 10:53:38 GMT
ARG NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499
# Tue, 26 Oct 2021 00:29:41 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.6 org.opencontainers.image.revision=cl210620210527-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 26 Oct 2021 00:29:45 GMT
ENV LIBERTY_VERSION=21.0.0_06
# Tue, 26 Oct 2021 00:29:48 GMT
ARG LIBERTY_URL
# Tue, 26 Oct 2021 00:29:50 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 26 Oct 2021 00:30:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 26 Oct 2021 00:30:26 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 26 Oct 2021 00:30:29 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.6 BuildLabel=cl210620210527-1900
# Tue, 26 Oct 2021 00:30:32 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:30:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 26 Oct 2021 00:30:43 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 26 Oct 2021 00:30:44 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 26 Oct 2021 00:30:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 26 Oct 2021 00:31:06 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 26 Oct 2021 00:31:09 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 26 Oct 2021 00:31:11 GMT
USER 1001
# Tue, 26 Oct 2021 00:31:14 GMT
EXPOSE 9080 9443
# Tue, 26 Oct 2021 00:31:17 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 26 Oct 2021 00:31:20 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 26 Oct 2021 00:33:47 GMT
ARG VERBOSE=false
# Tue, 26 Oct 2021 00:33:51 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 26 Oct 2021 00:37:27 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 26 Oct 2021 00:37:34 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 26 Oct 2021 00:38:31 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce6e130fd3d09fd3fe6d741e0fa3f77120aa82717cf6d0a1cb49439939243a6`  
		Last Modified: Wed, 06 Oct 2021 18:04:08 GMT  
		Size: 3.1 MB (3081580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8fc8962750bc0e8c7c6ca6d1498e303c66e1f0b3f9613d204da9abf0200933`  
		Last Modified: Wed, 06 Oct 2021 18:04:22 GMT  
		Size: 127.9 MB (127898987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9a714d8d1c09dab3f00c3c90466fe0981a767ced5cd99a96ed534ef4b07f87`  
		Last Modified: Tue, 26 Oct 2021 00:47:09 GMT  
		Size: 14.1 MB (14073892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5bc49a1220526acb930c481b8eb42c5b32ed2f2adc9f92e8e83bcb079330377`  
		Last Modified: Tue, 26 Oct 2021 00:47:06 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:543fcf18cd04c58cf6439872fd5b6073cc8865ee4f5e8cbfdbacee12e4329485`  
		Last Modified: Tue, 26 Oct 2021 00:47:05 GMT  
		Size: 9.7 KB (9678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7beb0573f06b60f0fd3c72107ac4640580e85d3f6d058dc13843840df9eb5eca`  
		Last Modified: Tue, 26 Oct 2021 00:47:05 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af50aeebdb33be93075c4211bb87a9a90639833db6aed3e7f9af6817c78daaae`  
		Last Modified: Tue, 26 Oct 2021 00:47:05 GMT  
		Size: 10.7 KB (10669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4f48a87091840e7b3656221d1ef1ad06eb4231bcd7bfb3f5d2a8472ab81b4b`  
		Last Modified: Tue, 26 Oct 2021 00:47:06 GMT  
		Size: 5.3 MB (5333323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5e97aa3277a9b9730efe95551cb5409193cd3b9230a1a8c119030fcb85957d`  
		Last Modified: Tue, 26 Oct 2021 00:47:48 GMT  
		Size: 207.8 MB (207778032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64bed44b76705eb556f0fe8e083b9452b4ec1c9824a726ececcc64167d2a542`  
		Last Modified: Tue, 26 Oct 2021 00:47:29 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebfc3903906b886b6deb143e554165ddcaeba78730675e4b27819c74ff581f6`  
		Last Modified: Tue, 26 Oct 2021 00:47:32 GMT  
		Size: 13.5 MB (13453290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.6-full-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:50df597743016bdd789d245ace0e6f7bad0c02e31e3b121cd00ce202206f6817
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.8 MB (396773391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1faaa6727bd551e86dc257a0034d82a0be8b611f6116fd6b9459f88eb60774d4`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:17 GMT
ADD file:d248d4b5739ee5d07e920ec481dc4af81b314aa52e64618322197a642394a41d in / 
# Fri, 01 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:23:32 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 02:23:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:23:37 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 02:24:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:24:19 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 01 Oct 2021 03:40:55 GMT
ARG VERBOSE=false
# Fri, 01 Oct 2021 03:40:55 GMT
ARG OPENJ9_SCC=true
# Fri, 01 Oct 2021 03:50:20 GMT
ARG EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27
# Fri, 01 Oct 2021 03:50:20 GMT
ARG NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c
# Fri, 01 Oct 2021 03:50:20 GMT
ARG NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499
# Mon, 25 Oct 2021 22:31:15 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.6 org.opencontainers.image.revision=cl210620210527-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 22:31:15 GMT
ENV LIBERTY_VERSION=21.0.0_06
# Mon, 25 Oct 2021 22:31:15 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 22:31:15 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 25 Oct 2021 22:31:25 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 25 Oct 2021 22:31:25 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Oct 2021 22:31:26 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.6 BuildLabel=cl210620210527-1900
# Mon, 25 Oct 2021 22:31:26 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:31:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 25 Oct 2021 22:31:27 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Mon, 25 Oct 2021 22:31:27 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 25 Oct 2021 22:31:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 25 Oct 2021 22:31:35 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 25 Oct 2021 22:31:35 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Mon, 25 Oct 2021 22:31:35 GMT
USER 1001
# Mon, 25 Oct 2021 22:31:35 GMT
EXPOSE 9080 9443
# Mon, 25 Oct 2021 22:31:36 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 25 Oct 2021 22:31:36 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Mon, 25 Oct 2021 22:32:05 GMT
ARG VERBOSE=false
# Mon, 25 Oct 2021 22:32:05 GMT
ARG REPOSITORIES_PROPERTIES=
# Mon, 25 Oct 2021 22:35:27 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Mon, 25 Oct 2021 22:35:30 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Mon, 25 Oct 2021 22:35:55 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:97372e5b313b6b8bab9913de546bc50f73818d8275c94fc6491993c97b9d8bad`  
		Last Modified: Fri, 01 Oct 2021 01:43:49 GMT  
		Size: 25.4 MB (25362918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf425722012c2264c66ba97a53ff25a2f196330fbcc0872474e5e4562fa95f0`  
		Last Modified: Fri, 01 Oct 2021 02:27:43 GMT  
		Size: 2.7 MB (2676365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d432d8be662b9a55c0dfed6d79d328a62b58be822a9888d1b7d0d16dc6c248`  
		Last Modified: Fri, 01 Oct 2021 02:27:51 GMT  
		Size: 125.4 MB (125395531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6f9a6936d04d8fd52520d90bface2cd0ef7690c0fdd45d0d63542e0f7ea252`  
		Last Modified: Mon, 25 Oct 2021 22:42:15 GMT  
		Size: 14.1 MB (14073226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d78b500f457420bad1b0324ba36fc1169238a7fe0e9a51b5a1527b2af87c34`  
		Last Modified: Mon, 25 Oct 2021 22:42:13 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587c1a82b142329126fc44964841511d06def6e71e321c95273e4338b8429381`  
		Last Modified: Mon, 25 Oct 2021 22:42:12 GMT  
		Size: 9.7 KB (9676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4593dbc11e774416fa080f1999b4ca2e6de94a640c4be56b99c349a4811f001`  
		Last Modified: Mon, 25 Oct 2021 22:42:13 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db9620e172e444f9bfa2c19838e59309e0eb2c537f8b2bf1db9f30c4a8647c6`  
		Last Modified: Mon, 25 Oct 2021 22:42:12 GMT  
		Size: 10.7 KB (10657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250c18b1575acc94a1a249ba90b5a2869922305994df8dc5bb51020f8a86880e`  
		Last Modified: Mon, 25 Oct 2021 22:42:13 GMT  
		Size: 5.9 MB (5850710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58197483ffd7d9470b6c13f2cf16d36668cf289c993068888e881cafdcf138a5`  
		Last Modified: Mon, 25 Oct 2021 22:42:37 GMT  
		Size: 207.8 MB (207778253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7424f9098727e32c41f9e1e34b91d72888d9b30ceeab14c2da7d558cd172bc`  
		Last Modified: Mon, 25 Oct 2021 22:42:28 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df355913235a7edd71821ee8b01f5bfafe4ea745b043dd7e08797e10fd25960`  
		Last Modified: Mon, 25 Oct 2021 22:42:29 GMT  
		Size: 15.6 MB (15614138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.6-kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:24228c6a96fc025b6221c7e0393835df7351cbad26122cb0a2e9338de09cc95f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.6-kernel-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:767a83d845b751237a7267d0a48e70a92e53c366f4dee67711f5dc3229df57f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.3 MB (110258180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa6d21e38c5cedfb6b8f7dd3d7caa548f00dce4f9a3ed0687278a66fa246ee6`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:44:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 02:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 00:31:11 GMT
ENV JAVA_VERSION=jdk-11.0.13+8_openj9-0.29.0
# Thu, 28 Oct 2021 00:33:11 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='3615940d4b26e8d11ff927dbf620a5247caecd84ba24c9d67f0e8b30ff463998';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_ppc64le_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        s390x)          ESUM='e942c0806163bbabe0b7ec8e630319489da400d58cd390011fc28428f468558e';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_s390x_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        amd64|x86_64)          ESUM='78eb54af15fac39eb2d254f51f0302aa213d3ad838f17766a9d081ca783edff4';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_x64_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 28 Oct 2021 00:33:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 00:33:11 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 28 Oct 2021 00:33:47 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 28 Oct 2021 01:07:18 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:07:18 GMT
ARG OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:15:53 GMT
ARG EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27
# Thu, 28 Oct 2021 01:15:53 GMT
ARG NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c
# Thu, 28 Oct 2021 01:15:53 GMT
ARG NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499
# Thu, 28 Oct 2021 01:15:53 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.6 org.opencontainers.image.revision=cl210620210527-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 28 Oct 2021 01:15:53 GMT
ENV LIBERTY_VERSION=21.0.0_06
# Thu, 28 Oct 2021 01:15:53 GMT
ARG LIBERTY_URL
# Thu, 28 Oct 2021 01:15:54 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 28 Oct 2021 01:16:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 01:16:03 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 01:16:03 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.6 BuildLabel=cl210620210527-1900
# Thu, 28 Oct 2021 01:16:03 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:16:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 28 Oct 2021 01:16:04 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Thu, 28 Oct 2021 01:16:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 28 Oct 2021 01:16:05 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 28 Oct 2021 01:16:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 28 Oct 2021 01:16:13 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 28 Oct 2021 01:16:14 GMT
USER 1001
# Thu, 28 Oct 2021 01:16:14 GMT
EXPOSE 9080 9443
# Thu, 28 Oct 2021 01:16:14 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 28 Oct 2021 01:16:14 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237daeb1ae282fe20092079ef6d5de7924746d0f2e9ad88797d08524a4d842fd`  
		Last Modified: Sat, 16 Oct 2021 02:47:20 GMT  
		Size: 16.0 MB (16036029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82607fdca83d197b118a35c377753995ef0400ef8de999ed3b8675d5fa58ce2f`  
		Last Modified: Thu, 28 Oct 2021 00:37:33 GMT  
		Size: 44.7 MB (44737093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7e4f4f21da9c3eec66f54b7ec452e3ccf00f68d74a7287bb1cbfbd68d2b041`  
		Last Modified: Thu, 28 Oct 2021 00:37:28 GMT  
		Size: 4.2 MB (4202694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6622e397e6bb51d9dc37e6dd0cf22ab476ef4c2e3c709c1f57f962a43c362881`  
		Last Modified: Thu, 28 Oct 2021 01:21:47 GMT  
		Size: 14.2 MB (14170433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65d10d381b726b348f861449ca2fe65ac55cfaf9324af07fe6670c997112924`  
		Last Modified: Thu, 28 Oct 2021 01:21:44 GMT  
		Size: 688.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6269d7e59287ca1196e4bd0c947d44b2f939048b335f77425dd62df101e15e8`  
		Last Modified: Thu, 28 Oct 2021 01:21:44 GMT  
		Size: 9.7 KB (9667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80755773242e268fd352271869ea66c6fa74cabb950e252a372f8cd67573a94`  
		Last Modified: Thu, 28 Oct 2021 01:21:44 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e49ff4c5091e2cc2b48066e7a89c36959148d58c6411f1c727851a1ff9367e8`  
		Last Modified: Thu, 28 Oct 2021 01:21:44 GMT  
		Size: 10.6 KB (10647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156a38b10d4279e3561c50812c97c992cb04d5e44fd719483b0b509cacbc36f7`  
		Last Modified: Thu, 28 Oct 2021 01:21:44 GMT  
		Size: 2.5 MB (2523559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.6-kernel-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:c2910320944c1ca71d9a5f106018cd5c39ad8d227cd8b5edf11474b3c4109270
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115543963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bd5f32b25d0f0630fa80eb51de38d3b0d03e384f756b49c59ef8c4bf40b5481`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:54:47 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 00:55:56 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Oct 2021 01:45:21 GMT
ENV JAVA_VERSION=jdk-11.0.12+7_openj9-0.27.0
# Thu, 21 Oct 2021 01:48:48 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='285bd388a497db61408d26a9f3328f62004714ede94456718cf6440a109e25d2';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_ppc64le_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        s390x)          ESUM='6e5829aeb37abfb122e0944e438ecb2043c56df14fcdcce39bd4e3c9a55571a8';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_s390x_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        amd64|x86_64)          ESUM='f352998f6fdf0b84f63c563608be57f30aa3f14c8117c1219422dbc712ad4f81';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_x64_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 21 Oct 2021 01:49:04 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 21 Oct 2021 01:49:23 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 21 Oct 2021 01:50:18 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 26 Oct 2021 00:02:27 GMT
ARG VERBOSE=false
# Tue, 26 Oct 2021 00:02:29 GMT
ARG OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:31:36 GMT
ARG EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27
# Tue, 26 Oct 2021 00:31:43 GMT
ARG NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c
# Tue, 26 Oct 2021 00:31:45 GMT
ARG NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499
# Tue, 26 Oct 2021 00:31:48 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.6 org.opencontainers.image.revision=cl210620210527-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 26 Oct 2021 00:31:51 GMT
ENV LIBERTY_VERSION=21.0.0_06
# Tue, 26 Oct 2021 00:31:53 GMT
ARG LIBERTY_URL
# Tue, 26 Oct 2021 00:31:57 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 26 Oct 2021 00:32:25 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 26 Oct 2021 00:32:28 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 26 Oct 2021 00:32:32 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.6 BuildLabel=cl210620210527-1900
# Tue, 26 Oct 2021 00:32:34 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:32:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 26 Oct 2021 00:32:42 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 26 Oct 2021 00:32:44 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 26 Oct 2021 00:32:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 26 Oct 2021 00:33:14 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 26 Oct 2021 00:33:17 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 26 Oct 2021 00:33:19 GMT
USER 1001
# Tue, 26 Oct 2021 00:33:21 GMT
EXPOSE 9080 9443
# Tue, 26 Oct 2021 00:33:24 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 26 Oct 2021 00:33:27 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c930749dacf55e37561edab7967f5a2f51660034fee0da501c2d71cb783301`  
		Last Modified: Sat, 16 Oct 2021 01:03:26 GMT  
		Size: 17.2 MB (17210510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d519f9110a27224937cddf5826128ca092be8957e9a8c13546df0dc596ba42`  
		Last Modified: Thu, 21 Oct 2021 02:03:00 GMT  
		Size: 45.1 MB (45107808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afebfecbc9bc8dad01d6486a0e236777ff1b2a82229ff13363f70a0827f07160`  
		Last Modified: Thu, 21 Oct 2021 02:02:53 GMT  
		Size: 3.3 MB (3286490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe9e25c140c6be09f6231808fc81e0efa6ed5ae38417ee0eca62564eabfc0a1`  
		Last Modified: Tue, 26 Oct 2021 00:47:21 GMT  
		Size: 14.2 MB (14170401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a96545a202495b9b4cdba4fa2d2b3f182e19d514c664a660f46b5650d4c77b8`  
		Last Modified: Tue, 26 Oct 2021 00:47:17 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d95fb332deaa47f41089f51b9a15535796a7b90829bc2253c5cb5fe6a9201be`  
		Last Modified: Tue, 26 Oct 2021 00:47:17 GMT  
		Size: 9.7 KB (9668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8d576ea60b888dd5893cf254a9bae933f86ce585acc11aa578b4c0fb16af26`  
		Last Modified: Tue, 26 Oct 2021 00:47:17 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3ff933d15821edff36a5ee5010094877ef4c98265e1f4601a1fe981ecc7edd`  
		Last Modified: Tue, 26 Oct 2021 00:47:17 GMT  
		Size: 10.6 KB (10646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aaa52636908415eb3d38c289800ec6ecc3315827d8abdeb909dc1004e67d06f`  
		Last Modified: Tue, 26 Oct 2021 00:47:17 GMT  
		Size: 2.5 MB (2460238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.6-kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:aa7d656eb563ce482ba02e90cb5b4d558b6ef5eefec1117bccd9e2249e7a6682
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107642963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc6774aedcbbcd56ef14aa892517898155821ba4a0afa34bf5c65ea2878aa751`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:58:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 00:58:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 00:58:27 GMT
ENV JAVA_VERSION=jdk-11.0.13+8_openj9-0.29.0
# Thu, 28 Oct 2021 00:59:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='3615940d4b26e8d11ff927dbf620a5247caecd84ba24c9d67f0e8b30ff463998';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_ppc64le_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        s390x)          ESUM='e942c0806163bbabe0b7ec8e630319489da400d58cd390011fc28428f468558e';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_s390x_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        amd64|x86_64)          ESUM='78eb54af15fac39eb2d254f51f0302aa213d3ad838f17766a9d081ca783edff4';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_x64_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 28 Oct 2021 00:59:28 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 00:59:28 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 28 Oct 2021 01:00:01 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 28 Oct 2021 01:43:09 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:43:09 GMT
ARG OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:52:46 GMT
ARG EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27
# Thu, 28 Oct 2021 01:52:46 GMT
ARG NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c
# Thu, 28 Oct 2021 01:52:46 GMT
ARG NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499
# Thu, 28 Oct 2021 01:52:46 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.6 org.opencontainers.image.revision=cl210620210527-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 28 Oct 2021 01:52:46 GMT
ENV LIBERTY_VERSION=21.0.0_06
# Thu, 28 Oct 2021 01:52:46 GMT
ARG LIBERTY_URL
# Thu, 28 Oct 2021 01:52:46 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 28 Oct 2021 01:52:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 01:52:55 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 01:52:55 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.6 BuildLabel=cl210620210527-1900
# Thu, 28 Oct 2021 01:52:55 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:52:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 28 Oct 2021 01:52:56 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Thu, 28 Oct 2021 01:52:56 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 28 Oct 2021 01:52:57 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 28 Oct 2021 01:53:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 28 Oct 2021 01:53:02 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 28 Oct 2021 01:53:02 GMT
USER 1001
# Thu, 28 Oct 2021 01:53:02 GMT
EXPOSE 9080 9443
# Thu, 28 Oct 2021 01:53:02 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 28 Oct 2021 01:53:02 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276dbe4459a060d2c186c43e5e92d98fa6f181617c55cce69da393b9d5dd6200`  
		Last Modified: Sat, 16 Oct 2021 01:01:03 GMT  
		Size: 15.7 MB (15742080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bef20936d077045a96f4b0694d1470b79e8825348eb06b3a0ef4207079d17d`  
		Last Modified: Thu, 28 Oct 2021 01:02:07 GMT  
		Size: 43.8 MB (43800069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8547dc44147bfe37bde98eef473a2916985469204db561ebefa3e3d92fee029a`  
		Last Modified: Thu, 28 Oct 2021 01:02:01 GMT  
		Size: 4.3 MB (4284720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c6269035de2a2ae68251fef891100b4f90d848cc7e5756129ed2a129490710`  
		Last Modified: Thu, 28 Oct 2021 01:59:04 GMT  
		Size: 14.2 MB (14170121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba336883ee9b632b0619412eaf3badde28f6055015167ab3fff29e1858a3cd9`  
		Last Modified: Thu, 28 Oct 2021 01:59:02 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c851801448baa7051180bce048eed67e287409df1ad4357ba8b44b0161885e`  
		Last Modified: Thu, 28 Oct 2021 01:59:02 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a59076e80744480249879a4a6bb1cdbe4df35dda41c76dc718555a0dc2845ec`  
		Last Modified: Thu, 28 Oct 2021 01:59:02 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e54b1669e7c95c2e98d837805135fbe24a09de022fdc4ac94e09280da43bf0c`  
		Last Modified: Thu, 28 Oct 2021 01:59:02 GMT  
		Size: 10.6 KB (10647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a70b8437e2349f6453d71474ae0e76ee6afa42fccd0cabff0cefe9ef5118008`  
		Last Modified: Thu, 28 Oct 2021 01:59:02 GMT  
		Size: 2.5 MB (2503840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.6-kernel-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:07d30af06a9fb488943b61a57f2629de9f34c0302abc956d168351c0b3a4e1fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.6-kernel-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:3ea39a0d3c08bc5a3d5b37d0c04b1b411c0f056dd2dafbcccb0dcc4740e7c88f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.9 MB (177923388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70bf182f30bf7fa13886e7716179738367fd7d862a0a009a530dd54e9b7cd120`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:55:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 02:55:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:55:32 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 02:56:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:56:08 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 01 Oct 2021 07:13:40 GMT
ARG VERBOSE=false
# Fri, 01 Oct 2021 07:13:40 GMT
ARG OPENJ9_SCC=true
# Fri, 01 Oct 2021 07:22:40 GMT
ARG EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27
# Fri, 01 Oct 2021 07:22:40 GMT
ARG NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c
# Fri, 01 Oct 2021 07:22:40 GMT
ARG NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499
# Mon, 25 Oct 2021 22:56:59 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.6 org.opencontainers.image.revision=cl210620210527-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 22:56:59 GMT
ENV LIBERTY_VERSION=21.0.0_06
# Mon, 25 Oct 2021 22:56:59 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 22:57:00 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 25 Oct 2021 22:57:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 25 Oct 2021 22:57:11 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Oct 2021 22:57:11 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.6 BuildLabel=cl210620210527-1900
# Mon, 25 Oct 2021 22:57:11 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:57:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 25 Oct 2021 22:57:13 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Mon, 25 Oct 2021 22:57:13 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 25 Oct 2021 22:57:14 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 25 Oct 2021 22:57:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 25 Oct 2021 22:57:23 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Mon, 25 Oct 2021 22:57:24 GMT
USER 1001
# Mon, 25 Oct 2021 22:57:24 GMT
EXPOSE 9080 9443
# Mon, 25 Oct 2021 22:57:24 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 25 Oct 2021 22:57:24 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf7ef5b4a4700901695d7489ffa25c9a36a0c54f7003664412a2a582dd362fa`  
		Last Modified: Fri, 01 Oct 2021 02:59:16 GMT  
		Size: 3.0 MB (2959872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58286f2e604db89582fc1898b2d2a229d5920927e7705c94e32f38a70e29902e`  
		Last Modified: Fri, 01 Oct 2021 02:59:26 GMT  
		Size: 128.4 MB (128395032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d9b3674446553288745201810a45b12d455d60f25fb7781c189fe1cd0df6a5`  
		Last Modified: Mon, 25 Oct 2021 23:07:41 GMT  
		Size: 14.1 MB (14073331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16336408a8e380e3f541c8020aee3f513b5e69e5a18233507df6cdd22a1fc0e5`  
		Last Modified: Mon, 25 Oct 2021 23:07:37 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459d0261a5ac122d0ca1631812f6dd203aa20559e524b6ea85f661c58e42f6a4`  
		Last Modified: Mon, 25 Oct 2021 23:07:38 GMT  
		Size: 9.7 KB (9676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b86b60ee9345ab1aba1cb3dbf0de1548f32c8bc3dd40eca65e7a65ad0b891b8`  
		Last Modified: Mon, 25 Oct 2021 23:07:37 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f003a342b48d85a24addcdd8ab33c372650b227b88b03a544adf6da569b5f4`  
		Last Modified: Mon, 25 Oct 2021 23:07:37 GMT  
		Size: 10.7 KB (10656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d36ee135e799a38aafcb6546d0b445a5985a3512685c6842c25c2d59677a79`  
		Last Modified: Mon, 25 Oct 2021 23:07:38 GMT  
		Size: 5.8 MB (5768773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.6-kernel-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:a7a289fffe863eb6dc57c34a4a5d1e8a29e2f377acda016235d6782324fb10cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.8 MB (180842031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:326599bb7d02337d44cdb7166142def89d225f144fa7ac5e6cfd5daf0f3d3b69`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 17:55:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Oct 2021 17:56:05 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 17:56:16 GMT
ENV JAVA_VERSION=8.0.6.36
# Wed, 06 Oct 2021 17:57:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Oct 2021 17:57:38 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 07 Oct 2021 10:35:31 GMT
ARG VERBOSE=false
# Thu, 07 Oct 2021 10:35:33 GMT
ARG OPENJ9_SCC=true
# Thu, 07 Oct 2021 10:53:29 GMT
ARG EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27
# Thu, 07 Oct 2021 10:53:34 GMT
ARG NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c
# Thu, 07 Oct 2021 10:53:38 GMT
ARG NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499
# Tue, 26 Oct 2021 00:29:41 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.6 org.opencontainers.image.revision=cl210620210527-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 26 Oct 2021 00:29:45 GMT
ENV LIBERTY_VERSION=21.0.0_06
# Tue, 26 Oct 2021 00:29:48 GMT
ARG LIBERTY_URL
# Tue, 26 Oct 2021 00:29:50 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 26 Oct 2021 00:30:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 26 Oct 2021 00:30:26 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 26 Oct 2021 00:30:29 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.6 BuildLabel=cl210620210527-1900
# Tue, 26 Oct 2021 00:30:32 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:30:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 26 Oct 2021 00:30:43 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 26 Oct 2021 00:30:44 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 26 Oct 2021 00:30:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 26 Oct 2021 00:31:06 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 26 Oct 2021 00:31:09 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 26 Oct 2021 00:31:11 GMT
USER 1001
# Tue, 26 Oct 2021 00:31:14 GMT
EXPOSE 9080 9443
# Tue, 26 Oct 2021 00:31:17 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 26 Oct 2021 00:31:20 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce6e130fd3d09fd3fe6d741e0fa3f77120aa82717cf6d0a1cb49439939243a6`  
		Last Modified: Wed, 06 Oct 2021 18:04:08 GMT  
		Size: 3.1 MB (3081580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8fc8962750bc0e8c7c6ca6d1498e303c66e1f0b3f9613d204da9abf0200933`  
		Last Modified: Wed, 06 Oct 2021 18:04:22 GMT  
		Size: 127.9 MB (127898987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9a714d8d1c09dab3f00c3c90466fe0981a767ced5cd99a96ed534ef4b07f87`  
		Last Modified: Tue, 26 Oct 2021 00:47:09 GMT  
		Size: 14.1 MB (14073892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5bc49a1220526acb930c481b8eb42c5b32ed2f2adc9f92e8e83bcb079330377`  
		Last Modified: Tue, 26 Oct 2021 00:47:06 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:543fcf18cd04c58cf6439872fd5b6073cc8865ee4f5e8cbfdbacee12e4329485`  
		Last Modified: Tue, 26 Oct 2021 00:47:05 GMT  
		Size: 9.7 KB (9678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7beb0573f06b60f0fd3c72107ac4640580e85d3f6d058dc13843840df9eb5eca`  
		Last Modified: Tue, 26 Oct 2021 00:47:05 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af50aeebdb33be93075c4211bb87a9a90639833db6aed3e7f9af6817c78daaae`  
		Last Modified: Tue, 26 Oct 2021 00:47:05 GMT  
		Size: 10.7 KB (10669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4f48a87091840e7b3656221d1ef1ad06eb4231bcd7bfb3f5d2a8472ab81b4b`  
		Last Modified: Tue, 26 Oct 2021 00:47:06 GMT  
		Size: 5.3 MB (5333323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.6-kernel-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:a83859c272cf395050e72bfb2a43de245787500114b7ae9181a8c57f88e23dc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.4 MB (173380053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39b352a6bb9b49e12a7856f5376c1c6de56a81373d7ded7ccb4fe0ce4b65a68d`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:17 GMT
ADD file:d248d4b5739ee5d07e920ec481dc4af81b314aa52e64618322197a642394a41d in / 
# Fri, 01 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:23:32 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 02:23:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:23:37 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 02:24:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:24:19 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 01 Oct 2021 03:40:55 GMT
ARG VERBOSE=false
# Fri, 01 Oct 2021 03:40:55 GMT
ARG OPENJ9_SCC=true
# Fri, 01 Oct 2021 03:50:20 GMT
ARG EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27
# Fri, 01 Oct 2021 03:50:20 GMT
ARG NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c
# Fri, 01 Oct 2021 03:50:20 GMT
ARG NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499
# Mon, 25 Oct 2021 22:31:15 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.6 org.opencontainers.image.revision=cl210620210527-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 22:31:15 GMT
ENV LIBERTY_VERSION=21.0.0_06
# Mon, 25 Oct 2021 22:31:15 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 22:31:15 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 25 Oct 2021 22:31:25 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 25 Oct 2021 22:31:25 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Oct 2021 22:31:26 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.6 BuildLabel=cl210620210527-1900
# Mon, 25 Oct 2021 22:31:26 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:31:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 25 Oct 2021 22:31:27 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Mon, 25 Oct 2021 22:31:27 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 25 Oct 2021 22:31:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 25 Oct 2021 22:31:35 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=c84028a2f075be3750c35ff2c384599c3d72f32f37ee77421a5a13650955bb27 NON_IBM_SHA=f67ddaaa8eb1aaeb68ca0ade04954a97dc5f9b18b4993f5be1181bae6639ac7c NOTICES_SHA=aa4d385fe77ad7c36447eb8e3c1318498bc5277f1a25ac7a3ccb3d9d47558499 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 25 Oct 2021 22:31:35 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Mon, 25 Oct 2021 22:31:35 GMT
USER 1001
# Mon, 25 Oct 2021 22:31:35 GMT
EXPOSE 9080 9443
# Mon, 25 Oct 2021 22:31:36 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 25 Oct 2021 22:31:36 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:97372e5b313b6b8bab9913de546bc50f73818d8275c94fc6491993c97b9d8bad`  
		Last Modified: Fri, 01 Oct 2021 01:43:49 GMT  
		Size: 25.4 MB (25362918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf425722012c2264c66ba97a53ff25a2f196330fbcc0872474e5e4562fa95f0`  
		Last Modified: Fri, 01 Oct 2021 02:27:43 GMT  
		Size: 2.7 MB (2676365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d432d8be662b9a55c0dfed6d79d328a62b58be822a9888d1b7d0d16dc6c248`  
		Last Modified: Fri, 01 Oct 2021 02:27:51 GMT  
		Size: 125.4 MB (125395531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6f9a6936d04d8fd52520d90bface2cd0ef7690c0fdd45d0d63542e0f7ea252`  
		Last Modified: Mon, 25 Oct 2021 22:42:15 GMT  
		Size: 14.1 MB (14073226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d78b500f457420bad1b0324ba36fc1169238a7fe0e9a51b5a1527b2af87c34`  
		Last Modified: Mon, 25 Oct 2021 22:42:13 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587c1a82b142329126fc44964841511d06def6e71e321c95273e4338b8429381`  
		Last Modified: Mon, 25 Oct 2021 22:42:12 GMT  
		Size: 9.7 KB (9676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4593dbc11e774416fa080f1999b4ca2e6de94a640c4be56b99c349a4811f001`  
		Last Modified: Mon, 25 Oct 2021 22:42:13 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db9620e172e444f9bfa2c19838e59309e0eb2c537f8b2bf1db9f30c4a8647c6`  
		Last Modified: Mon, 25 Oct 2021 22:42:12 GMT  
		Size: 10.7 KB (10657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250c18b1575acc94a1a249ba90b5a2869922305994df8dc5bb51020f8a86880e`  
		Last Modified: Mon, 25 Oct 2021 22:42:13 GMT  
		Size: 5.9 MB (5850710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.9-full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:61c8333e7be1f33c34350d96dfb3d82d40681b8127705da4e0c4a18f095c77c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.9-full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:2c9022b7db6ab207cd6b735334181f1f9d4366b8b252f8cb2c47808c699540e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.9 MB (333923868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba329bcfa025ab60c0728882a367aa8d2ff05ccc5081c9e754fb591c83480e4e`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:44:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 02:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 00:31:11 GMT
ENV JAVA_VERSION=jdk-11.0.13+8_openj9-0.29.0
# Thu, 28 Oct 2021 00:33:11 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='3615940d4b26e8d11ff927dbf620a5247caecd84ba24c9d67f0e8b30ff463998';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_ppc64le_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        s390x)          ESUM='e942c0806163bbabe0b7ec8e630319489da400d58cd390011fc28428f468558e';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_s390x_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        amd64|x86_64)          ESUM='78eb54af15fac39eb2d254f51f0302aa213d3ad838f17766a9d081ca783edff4';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_x64_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 28 Oct 2021 00:33:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 00:33:11 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 28 Oct 2021 00:33:47 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 28 Oct 2021 01:07:18 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:07:18 GMT
ARG OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:11:49 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Thu, 28 Oct 2021 01:11:49 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Thu, 28 Oct 2021 01:11:49 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Thu, 28 Oct 2021 01:11:49 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 28 Oct 2021 01:11:49 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Thu, 28 Oct 2021 01:11:50 GMT
ARG LIBERTY_URL
# Thu, 28 Oct 2021 01:11:50 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 28 Oct 2021 01:11:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 01:11:58 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 01:11:58 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Thu, 28 Oct 2021 01:11:58 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:11:59 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 28 Oct 2021 01:12:00 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Thu, 28 Oct 2021 01:12:00 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 28 Oct 2021 01:12:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 28 Oct 2021 01:12:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 28 Oct 2021 01:12:09 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 28 Oct 2021 01:12:09 GMT
USER 1001
# Thu, 28 Oct 2021 01:12:09 GMT
EXPOSE 9080 9443
# Thu, 28 Oct 2021 01:12:09 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 28 Oct 2021 01:12:10 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 28 Oct 2021 01:12:13 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:12:13 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 28 Oct 2021 01:15:12 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Thu, 28 Oct 2021 01:15:13 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 28 Oct 2021 01:15:49 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237daeb1ae282fe20092079ef6d5de7924746d0f2e9ad88797d08524a4d842fd`  
		Last Modified: Sat, 16 Oct 2021 02:47:20 GMT  
		Size: 16.0 MB (16036029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82607fdca83d197b118a35c377753995ef0400ef8de999ed3b8675d5fa58ce2f`  
		Last Modified: Thu, 28 Oct 2021 00:37:33 GMT  
		Size: 44.7 MB (44737093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7e4f4f21da9c3eec66f54b7ec452e3ccf00f68d74a7287bb1cbfbd68d2b041`  
		Last Modified: Thu, 28 Oct 2021 00:37:28 GMT  
		Size: 4.2 MB (4202694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3336d177bbffe22981144111fc0eef0a43b1505ffef716506854656e37286356`  
		Last Modified: Thu, 28 Oct 2021 01:21:17 GMT  
		Size: 14.2 MB (14154670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c4b52f389be8a2c78e0ab2d98627c652cf6848befed480f95e0a6ada70b627`  
		Last Modified: Thu, 28 Oct 2021 01:21:13 GMT  
		Size: 688.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea2050f99c3896ed695883c76758336c4ecd84fe3786bea63595cf8c8a5e924`  
		Last Modified: Thu, 28 Oct 2021 01:21:14 GMT  
		Size: 9.7 KB (9675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b4ef7dd35d03fff1004952f01b94fddaf7839e8b22f6726e34665b9adb3fbb`  
		Last Modified: Thu, 28 Oct 2021 01:21:13 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b55e8eb5f9387ee0a9aaf2f71223a594b3ac069f211d5b9b30e69c68a22372a`  
		Last Modified: Thu, 28 Oct 2021 01:21:13 GMT  
		Size: 10.6 KB (10637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:830a1b0e8f739453bb9363f4732cc496199f5520aee78917ff8e2e1874850d68`  
		Last Modified: Thu, 28 Oct 2021 01:21:14 GMT  
		Size: 2.5 MB (2530872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4d5e3a9e3d140d0f3688bc8c291a9d042385e2789eddc6ddf01d6c7865fee0`  
		Last Modified: Thu, 28 Oct 2021 01:21:36 GMT  
		Size: 209.2 MB (209236201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cb98a980d903fc5c8fa11a5c03256a63d6167a33b0a516f1557f39661aaf9d`  
		Last Modified: Thu, 28 Oct 2021 01:21:25 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7267f89f49c73cfa494b3aa48c443443c0c4585f20995785a2b72d4e9e860647`  
		Last Modified: Thu, 28 Oct 2021 01:21:26 GMT  
		Size: 14.4 MB (14436992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.9-full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:0341ab865bc208f34dad7b67bdc121e8670d175d41de27e8d4adac79c2688d3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.1 MB (339097242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dfa0d1dc96f4f6d7c38f5feba8f054ce90b75b6d3fbd661228043642dfad14e`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:54:47 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 00:55:56 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Oct 2021 01:45:21 GMT
ENV JAVA_VERSION=jdk-11.0.12+7_openj9-0.27.0
# Thu, 21 Oct 2021 01:48:48 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='285bd388a497db61408d26a9f3328f62004714ede94456718cf6440a109e25d2';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_ppc64le_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        s390x)          ESUM='6e5829aeb37abfb122e0944e438ecb2043c56df14fcdcce39bd4e3c9a55571a8';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_s390x_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        amd64|x86_64)          ESUM='f352998f6fdf0b84f63c563608be57f30aa3f14c8117c1219422dbc712ad4f81';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_x64_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 21 Oct 2021 01:49:04 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 21 Oct 2021 01:49:23 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 21 Oct 2021 01:50:18 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 26 Oct 2021 00:02:27 GMT
ARG VERBOSE=false
# Tue, 26 Oct 2021 00:02:29 GMT
ARG OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:17:26 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Tue, 26 Oct 2021 00:17:31 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Tue, 26 Oct 2021 00:17:34 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Tue, 26 Oct 2021 00:17:37 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 26 Oct 2021 00:17:40 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Tue, 26 Oct 2021 00:17:43 GMT
ARG LIBERTY_URL
# Tue, 26 Oct 2021 00:17:47 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 26 Oct 2021 00:18:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 26 Oct 2021 00:18:21 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 26 Oct 2021 00:18:23 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Tue, 26 Oct 2021 00:18:24 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:18:29 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 26 Oct 2021 00:18:30 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 26 Oct 2021 00:18:31 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 26 Oct 2021 00:18:38 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 26 Oct 2021 00:18:55 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 26 Oct 2021 00:18:59 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 26 Oct 2021 00:19:03 GMT
USER 1001
# Tue, 26 Oct 2021 00:19:06 GMT
EXPOSE 9080 9443
# Tue, 26 Oct 2021 00:19:08 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 26 Oct 2021 00:19:10 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 26 Oct 2021 00:24:30 GMT
ARG VERBOSE=false
# Tue, 26 Oct 2021 00:24:35 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 26 Oct 2021 00:28:02 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 26 Oct 2021 00:28:11 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 26 Oct 2021 00:29:23 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c930749dacf55e37561edab7967f5a2f51660034fee0da501c2d71cb783301`  
		Last Modified: Sat, 16 Oct 2021 01:03:26 GMT  
		Size: 17.2 MB (17210510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d519f9110a27224937cddf5826128ca092be8957e9a8c13546df0dc596ba42`  
		Last Modified: Thu, 21 Oct 2021 02:03:00 GMT  
		Size: 45.1 MB (45107808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afebfecbc9bc8dad01d6486a0e236777ff1b2a82229ff13363f70a0827f07160`  
		Last Modified: Thu, 21 Oct 2021 02:02:53 GMT  
		Size: 3.3 MB (3286490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2bbb876c50debfd5a770b2a023253c6b5841b51140118fdf1555ffc5f3196d`  
		Last Modified: Tue, 26 Oct 2021 00:46:02 GMT  
		Size: 14.2 MB (14155026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140048859b8a73b0a7702df71cf44d9a50883ea7827ed8d03706c4746dc12263`  
		Last Modified: Tue, 26 Oct 2021 00:45:57 GMT  
		Size: 697.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b686649f8d628437ccdfecad3a80c0dcdd3a793bdde05bdc592de982cd11bc2a`  
		Last Modified: Tue, 26 Oct 2021 00:45:57 GMT  
		Size: 9.7 KB (9672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226708f83081b74fc92b8f84783cc66376a275ff0d2e8b3aec2fabea730e3ec2`  
		Last Modified: Tue, 26 Oct 2021 00:45:57 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f2bafacacaceecd1d395d593f7acd69511203ba36df026fa2c5615062d0e6e`  
		Last Modified: Tue, 26 Oct 2021 00:45:57 GMT  
		Size: 10.7 KB (10660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b033eb87d2f3e8019ad942a2e334e3a5f96e35bd726204627a3c276920e14db`  
		Last Modified: Tue, 26 Oct 2021 00:45:57 GMT  
		Size: 2.5 MB (2479958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7a441ef2e69f2f2f215c1dc4adbec054882101419082b8cd2d08da63e657c8`  
		Last Modified: Tue, 26 Oct 2021 00:46:57 GMT  
		Size: 209.2 MB (209236026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6f14929e822899bfdcbb6503592937012cf713b2dac666bd12ae81a7abafaa`  
		Last Modified: Tue, 26 Oct 2021 00:46:38 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7bda66602c9d7f473960e7cfeb109871c11f0bd7f83694fcbff32b8e19ccfd`  
		Last Modified: Tue, 26 Oct 2021 00:46:42 GMT  
		Size: 14.3 MB (14311936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.9-full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:4d6062a46bb440282bd30e52d01cc03ee0bf65c2530717cf7ac0dd1875994b1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.1 MB (331100167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edeffd712390eb34db43eb9ee0c93771c0de40b94930768bf288d9570b59efe4`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:58:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 00:58:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 00:58:27 GMT
ENV JAVA_VERSION=jdk-11.0.13+8_openj9-0.29.0
# Thu, 28 Oct 2021 00:59:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='3615940d4b26e8d11ff927dbf620a5247caecd84ba24c9d67f0e8b30ff463998';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_ppc64le_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        s390x)          ESUM='e942c0806163bbabe0b7ec8e630319489da400d58cd390011fc28428f468558e';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_s390x_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        amd64|x86_64)          ESUM='78eb54af15fac39eb2d254f51f0302aa213d3ad838f17766a9d081ca783edff4';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_x64_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 28 Oct 2021 00:59:28 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 00:59:28 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 28 Oct 2021 01:00:01 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 28 Oct 2021 01:43:09 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:43:09 GMT
ARG OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:48:08 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Thu, 28 Oct 2021 01:48:08 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Thu, 28 Oct 2021 01:48:08 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Thu, 28 Oct 2021 01:48:08 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 28 Oct 2021 01:48:08 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Thu, 28 Oct 2021 01:48:08 GMT
ARG LIBERTY_URL
# Thu, 28 Oct 2021 01:48:08 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 28 Oct 2021 01:48:18 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 01:48:18 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 01:48:18 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Thu, 28 Oct 2021 01:48:18 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:48:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 28 Oct 2021 01:48:19 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Thu, 28 Oct 2021 01:48:19 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 28 Oct 2021 01:48:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 28 Oct 2021 01:48:25 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 28 Oct 2021 01:48:25 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 28 Oct 2021 01:48:25 GMT
USER 1001
# Thu, 28 Oct 2021 01:48:25 GMT
EXPOSE 9080 9443
# Thu, 28 Oct 2021 01:48:25 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 28 Oct 2021 01:48:25 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 28 Oct 2021 01:48:36 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:48:36 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 28 Oct 2021 01:52:05 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Thu, 28 Oct 2021 01:52:09 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 28 Oct 2021 01:52:32 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276dbe4459a060d2c186c43e5e92d98fa6f181617c55cce69da393b9d5dd6200`  
		Last Modified: Sat, 16 Oct 2021 01:01:03 GMT  
		Size: 15.7 MB (15742080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bef20936d077045a96f4b0694d1470b79e8825348eb06b3a0ef4207079d17d`  
		Last Modified: Thu, 28 Oct 2021 01:02:07 GMT  
		Size: 43.8 MB (43800069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8547dc44147bfe37bde98eef473a2916985469204db561ebefa3e3d92fee029a`  
		Last Modified: Thu, 28 Oct 2021 01:02:01 GMT  
		Size: 4.3 MB (4284720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1f40bdf8d3065335a6711be483011d3a2c6db876d44c02fe7b0809ec2386d4`  
		Last Modified: Thu, 28 Oct 2021 01:58:41 GMT  
		Size: 14.2 MB (14154247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2506960ba73954b1b9e3f1d70ab192fd19e66d138ca46a041fffc31ec2f3a2`  
		Last Modified: Thu, 28 Oct 2021 01:58:38 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cd49c1312502c3c1dfaa88066867c9ca17bdfcf1b9337e6295916d25d3125e`  
		Last Modified: Thu, 28 Oct 2021 01:58:39 GMT  
		Size: 9.7 KB (9673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d8529abd76153ce49ed0735547223bfa11751320827d0c34e0f65e15dda7ef`  
		Last Modified: Thu, 28 Oct 2021 01:58:38 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3c3f709c7c595ddeed628c390ea5f713025fc0afbec8a64cce8d0fe58cf465`  
		Last Modified: Thu, 28 Oct 2021 01:58:39 GMT  
		Size: 10.6 KB (10633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7061f36639c9e42ab9b73bb51e5cb1d667c32172d5f968e3dd87c8e72b6f269`  
		Last Modified: Thu, 28 Oct 2021 01:58:39 GMT  
		Size: 2.6 MB (2556747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ac1baca00d3817ae1c77440dbcedabe2cf530a859fb499b3de171d589d0bfb`  
		Last Modified: Thu, 28 Oct 2021 01:58:55 GMT  
		Size: 209.2 MB (209237504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb257eda50a5816ad5139916b381432a20d474d73c1f1acc178555eef7f265ad`  
		Last Modified: Thu, 28 Oct 2021 01:58:46 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab4180e5f4105f2804e1dc0dc960e41267ded12e07b6283be75633e7590e24f`  
		Last Modified: Thu, 28 Oct 2021 01:58:48 GMT  
		Size: 14.2 MB (14181732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.9-full-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:2b5e74c29a3ee4b65142de10b41aeafa7b4545f3583ed8c9a15f6f6a433dce28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.9-full-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:f08775162268143611eb8ee4bb0d99f20875ea4b4c66dda6cc2180b3b531f1c4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.2 MB (403204955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4da88422f300a09ba6b59324747c6e99dbd98ec75c7238f48222a2a89c71b8f`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:55:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 02:55:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:55:32 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 02:56:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:56:08 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 01 Oct 2021 07:13:40 GMT
ARG VERBOSE=false
# Fri, 01 Oct 2021 07:13:40 GMT
ARG OPENJ9_SCC=true
# Fri, 01 Oct 2021 07:13:41 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Fri, 01 Oct 2021 07:13:41 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Fri, 01 Oct 2021 07:13:41 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Mon, 25 Oct 2021 22:48:12 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 22:48:12 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Mon, 25 Oct 2021 22:48:12 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 22:48:13 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 25 Oct 2021 22:48:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 25 Oct 2021 22:48:23 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Oct 2021 22:48:23 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Mon, 25 Oct 2021 22:48:24 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:48:25 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 25 Oct 2021 22:48:25 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Mon, 25 Oct 2021 22:48:25 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 25 Oct 2021 22:48:26 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 25 Oct 2021 22:48:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 25 Oct 2021 22:48:39 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Mon, 25 Oct 2021 22:48:39 GMT
USER 1001
# Mon, 25 Oct 2021 22:48:39 GMT
EXPOSE 9080 9443
# Mon, 25 Oct 2021 22:48:39 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 25 Oct 2021 22:48:40 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Mon, 25 Oct 2021 22:49:13 GMT
ARG VERBOSE=false
# Mon, 25 Oct 2021 22:49:13 GMT
ARG REPOSITORIES_PROPERTIES=
# Mon, 25 Oct 2021 22:52:12 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Mon, 25 Oct 2021 22:52:13 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Mon, 25 Oct 2021 22:52:59 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf7ef5b4a4700901695d7489ffa25c9a36a0c54f7003664412a2a582dd362fa`  
		Last Modified: Fri, 01 Oct 2021 02:59:16 GMT  
		Size: 3.0 MB (2959872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58286f2e604db89582fc1898b2d2a229d5920927e7705c94e32f38a70e29902e`  
		Last Modified: Fri, 01 Oct 2021 02:59:26 GMT  
		Size: 128.4 MB (128395032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6b34b3fe1e2ac672fb71a817fa7b6266bbe76d88da83b6e38aaa6c20d9e05f`  
		Last Modified: Mon, 25 Oct 2021 23:06:43 GMT  
		Size: 14.1 MB (14055841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff676a6e06f8f0ab9ebb31c8abad4db4a81934bd7bd8bc3d0ac484b962eeabc7`  
		Last Modified: Mon, 25 Oct 2021 23:06:40 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be89447c7cd07521bfc85588c50472f60c408f7facd9fb0fb237a16b6acdfcb`  
		Last Modified: Mon, 25 Oct 2021 23:06:40 GMT  
		Size: 9.7 KB (9679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b208b084380a5fccc395ee069904ea3f308e4ea6897282cebcc63517746c6f`  
		Last Modified: Mon, 25 Oct 2021 23:06:40 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d43a88abc25a0df6edd20918a59d54bc350863b51ef4ddddb8df459c7395f34`  
		Last Modified: Mon, 25 Oct 2021 23:06:40 GMT  
		Size: 10.7 KB (10656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948bc49342b1aba0c5ffefd707205d45ee8098d91243daf584073879cb867159`  
		Last Modified: Mon, 25 Oct 2021 23:06:41 GMT  
		Size: 5.9 MB (5924912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd575bcf92a6dbdba1e5e5bfca37fcb55e5647878423dca63d6ae5d4a916da0`  
		Last Modified: Mon, 25 Oct 2021 23:07:12 GMT  
		Size: 209.2 MB (209236922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4420ee8e278ba15ea7f4c20839278adc59ff0ee2c91531b2000c3c32910c57e`  
		Last Modified: Mon, 25 Oct 2021 23:07:01 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db111b85ff3aa9f90adbcb59897435e6579cbef102275102210fddaac377b20`  
		Last Modified: Mon, 25 Oct 2021 23:07:03 GMT  
		Size: 15.9 MB (15905044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.9-full-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:3b1f7204413528a9cd270417655cc3dfdee3d5a491f55a39b9406705c065a9c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.5 MB (403531716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ec6bc68b0bd400d2321d3ec16052e5ba311cedb4ac14dbb030d90c4a422f810`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 17:55:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Oct 2021 17:56:05 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 17:56:16 GMT
ENV JAVA_VERSION=8.0.6.36
# Wed, 06 Oct 2021 17:57:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Oct 2021 17:57:38 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 07 Oct 2021 10:35:31 GMT
ARG VERBOSE=false
# Thu, 07 Oct 2021 10:35:33 GMT
ARG OPENJ9_SCC=true
# Thu, 07 Oct 2021 10:35:37 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Thu, 07 Oct 2021 10:35:40 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Thu, 07 Oct 2021 10:35:44 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Tue, 26 Oct 2021 00:15:30 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 26 Oct 2021 00:15:33 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Tue, 26 Oct 2021 00:15:41 GMT
ARG LIBERTY_URL
# Tue, 26 Oct 2021 00:15:44 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 26 Oct 2021 00:16:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 26 Oct 2021 00:16:16 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 26 Oct 2021 00:16:19 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Tue, 26 Oct 2021 00:16:22 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:16:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 26 Oct 2021 00:16:29 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 26 Oct 2021 00:16:30 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 26 Oct 2021 00:16:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 26 Oct 2021 00:17:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 26 Oct 2021 00:17:04 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 26 Oct 2021 00:17:08 GMT
USER 1001
# Tue, 26 Oct 2021 00:17:10 GMT
EXPOSE 9080 9443
# Tue, 26 Oct 2021 00:17:12 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 26 Oct 2021 00:17:15 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 26 Oct 2021 00:19:21 GMT
ARG VERBOSE=false
# Tue, 26 Oct 2021 00:19:24 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 26 Oct 2021 00:23:12 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 26 Oct 2021 00:23:19 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 26 Oct 2021 00:24:16 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce6e130fd3d09fd3fe6d741e0fa3f77120aa82717cf6d0a1cb49439939243a6`  
		Last Modified: Wed, 06 Oct 2021 18:04:08 GMT  
		Size: 3.1 MB (3081580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8fc8962750bc0e8c7c6ca6d1498e303c66e1f0b3f9613d204da9abf0200933`  
		Last Modified: Wed, 06 Oct 2021 18:04:22 GMT  
		Size: 127.9 MB (127898987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f55a4db9d34cf93dd60782337c13c76c8ee005bf5339aa599e11a4327f187f`  
		Last Modified: Tue, 26 Oct 2021 00:45:49 GMT  
		Size: 14.1 MB (14056411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8eeb13a7ada163c02afc93c5e69bde8338b653b68b154a43f6ecd1387e58ae`  
		Last Modified: Tue, 26 Oct 2021 00:45:45 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76fb073018ee13c91d1b735c3b7cb2d598bffe904df702f8a3449a44b2c1ab8`  
		Last Modified: Tue, 26 Oct 2021 00:45:45 GMT  
		Size: 9.7 KB (9678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d3691144cafeb2afb474b28084deaa7c58e8e8303e1eab03a62f6d8fd614a7`  
		Last Modified: Tue, 26 Oct 2021 00:45:45 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4730641c79dd1259bea562e04a9f1055cfa2c2ca5be6c48fdb49666d6d9f8c3a`  
		Last Modified: Tue, 26 Oct 2021 00:45:45 GMT  
		Size: 10.7 KB (10654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e1c01f839290ab733d015d2333f4d63bb4fec50d5ae49cb400108993b575b4`  
		Last Modified: Tue, 26 Oct 2021 00:45:46 GMT  
		Size: 5.3 MB (5319906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b083b65ca33cfd4ef3a907b332add8fb49b04885e8425895b211c9de5dcb909`  
		Last Modified: Tue, 26 Oct 2021 00:46:29 GMT  
		Size: 209.2 MB (209237411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439e7df6d20229d8840cfb2659972cfa62d5155a45f5f9338d7e2aed95aaab8b`  
		Last Modified: Tue, 26 Oct 2021 00:46:11 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f65b19512751409b1514e95c329f29e9137beb4c0e46cebb75b1f8725ddfe20`  
		Last Modified: Tue, 26 Oct 2021 00:46:15 GMT  
		Size: 13.5 MB (13482251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.9-full-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:c587e3434891f8e56d1c9b5f00c86a669e977a0443e34ca34e25276e2335a7ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.2 MB (398171448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab90fed6e7133f233210b963d2253ca53c1d3db873f69dd4881452e84c5ce91b`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:17 GMT
ADD file:d248d4b5739ee5d07e920ec481dc4af81b314aa52e64618322197a642394a41d in / 
# Fri, 01 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:23:32 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 02:23:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:23:37 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 02:24:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:24:19 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 01 Oct 2021 03:40:55 GMT
ARG VERBOSE=false
# Fri, 01 Oct 2021 03:40:55 GMT
ARG OPENJ9_SCC=true
# Fri, 01 Oct 2021 03:40:55 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Fri, 01 Oct 2021 03:40:55 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Fri, 01 Oct 2021 03:40:56 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Mon, 25 Oct 2021 22:22:13 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 22:22:13 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Mon, 25 Oct 2021 22:22:13 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 22:22:13 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 25 Oct 2021 22:22:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 25 Oct 2021 22:22:23 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Oct 2021 22:22:23 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Mon, 25 Oct 2021 22:22:23 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:22:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 25 Oct 2021 22:22:24 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Mon, 25 Oct 2021 22:22:24 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 25 Oct 2021 22:22:25 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 25 Oct 2021 22:22:32 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 25 Oct 2021 22:22:32 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Mon, 25 Oct 2021 22:22:33 GMT
USER 1001
# Mon, 25 Oct 2021 22:22:33 GMT
EXPOSE 9080 9443
# Mon, 25 Oct 2021 22:22:33 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 25 Oct 2021 22:22:33 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Mon, 25 Oct 2021 22:23:03 GMT
ARG VERBOSE=false
# Mon, 25 Oct 2021 22:23:04 GMT
ARG REPOSITORIES_PROPERTIES=
# Mon, 25 Oct 2021 22:26:23 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Mon, 25 Oct 2021 22:26:27 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Mon, 25 Oct 2021 22:26:51 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:97372e5b313b6b8bab9913de546bc50f73818d8275c94fc6491993c97b9d8bad`  
		Last Modified: Fri, 01 Oct 2021 01:43:49 GMT  
		Size: 25.4 MB (25362918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf425722012c2264c66ba97a53ff25a2f196330fbcc0872474e5e4562fa95f0`  
		Last Modified: Fri, 01 Oct 2021 02:27:43 GMT  
		Size: 2.7 MB (2676365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d432d8be662b9a55c0dfed6d79d328a62b58be822a9888d1b7d0d16dc6c248`  
		Last Modified: Fri, 01 Oct 2021 02:27:51 GMT  
		Size: 125.4 MB (125395531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1c407fef21834b60347997a27a33dd46260bb9a0dbd74913531b9bfa1018d7`  
		Last Modified: Mon, 25 Oct 2021 22:41:32 GMT  
		Size: 14.1 MB (14055683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e69603ecc97823e1c3e2fdd733acb6cc44a73d9a8789630027470157eb50624`  
		Last Modified: Mon, 25 Oct 2021 22:41:30 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd84e34c2ee9ac1b31a1eb011b616fdc23f2095245ccaa7abc7f9fd4ad5b4cc`  
		Last Modified: Mon, 25 Oct 2021 22:41:30 GMT  
		Size: 9.7 KB (9676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6729e19b1db5910b295b3eceb90cd56fb7453af5ba2b16cce7d3ed6093233a0`  
		Last Modified: Mon, 25 Oct 2021 22:41:30 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6906524465d542cc5f411e1de178ff5e0cfcd028e0a6e8ed38d9a339abb34db`  
		Last Modified: Mon, 25 Oct 2021 22:41:30 GMT  
		Size: 10.7 KB (10657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3a668e776118ad579c7d124d53ba234b2f4ea142c908ddf9696032b4ae29dc`  
		Last Modified: Mon, 25 Oct 2021 22:41:31 GMT  
		Size: 5.8 MB (5833067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219f9a8986e07980ecc15fa9bdfc0e84fa94577923d4aae07e5281a03d7c1911`  
		Last Modified: Mon, 25 Oct 2021 22:41:53 GMT  
		Size: 209.2 MB (209236952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4e983110a18591003f0e53e9f43847ea7201949e54a8a0abfa7dfdabe577d6`  
		Last Modified: Mon, 25 Oct 2021 22:41:44 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5410a28ca0464dc505d45a9fd68b95737e9b758148a575d6d0deeb26994021`  
		Last Modified: Mon, 25 Oct 2021 22:41:45 GMT  
		Size: 15.6 MB (15588683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.9-kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:be50b5ac4eeb068820f35eb8004f83038b09943f4399c8793c1ab4e4ca15e9f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.9-kernel-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:1e16216bc79424ff00a69766f9fbcacf264a53a0c3832eec4ec42aab2dea51c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110249729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48509f607ffa428b9610bed2e6a33085f53761fe124fa18f9a762a80abade123`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:44:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 02:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 00:31:11 GMT
ENV JAVA_VERSION=jdk-11.0.13+8_openj9-0.29.0
# Thu, 28 Oct 2021 00:33:11 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='3615940d4b26e8d11ff927dbf620a5247caecd84ba24c9d67f0e8b30ff463998';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_ppc64le_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        s390x)          ESUM='e942c0806163bbabe0b7ec8e630319489da400d58cd390011fc28428f468558e';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_s390x_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        amd64|x86_64)          ESUM='78eb54af15fac39eb2d254f51f0302aa213d3ad838f17766a9d081ca783edff4';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_x64_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 28 Oct 2021 00:33:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 00:33:11 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 28 Oct 2021 00:33:47 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 28 Oct 2021 01:07:18 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:07:18 GMT
ARG OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:11:49 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Thu, 28 Oct 2021 01:11:49 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Thu, 28 Oct 2021 01:11:49 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Thu, 28 Oct 2021 01:11:49 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 28 Oct 2021 01:11:49 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Thu, 28 Oct 2021 01:11:50 GMT
ARG LIBERTY_URL
# Thu, 28 Oct 2021 01:11:50 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 28 Oct 2021 01:11:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 01:11:58 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 01:11:58 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Thu, 28 Oct 2021 01:11:58 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:11:59 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 28 Oct 2021 01:12:00 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Thu, 28 Oct 2021 01:12:00 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 28 Oct 2021 01:12:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 28 Oct 2021 01:12:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 28 Oct 2021 01:12:09 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 28 Oct 2021 01:12:09 GMT
USER 1001
# Thu, 28 Oct 2021 01:12:09 GMT
EXPOSE 9080 9443
# Thu, 28 Oct 2021 01:12:09 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 28 Oct 2021 01:12:10 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237daeb1ae282fe20092079ef6d5de7924746d0f2e9ad88797d08524a4d842fd`  
		Last Modified: Sat, 16 Oct 2021 02:47:20 GMT  
		Size: 16.0 MB (16036029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82607fdca83d197b118a35c377753995ef0400ef8de999ed3b8675d5fa58ce2f`  
		Last Modified: Thu, 28 Oct 2021 00:37:33 GMT  
		Size: 44.7 MB (44737093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7e4f4f21da9c3eec66f54b7ec452e3ccf00f68d74a7287bb1cbfbd68d2b041`  
		Last Modified: Thu, 28 Oct 2021 00:37:28 GMT  
		Size: 4.2 MB (4202694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3336d177bbffe22981144111fc0eef0a43b1505ffef716506854656e37286356`  
		Last Modified: Thu, 28 Oct 2021 01:21:17 GMT  
		Size: 14.2 MB (14154670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c4b52f389be8a2c78e0ab2d98627c652cf6848befed480f95e0a6ada70b627`  
		Last Modified: Thu, 28 Oct 2021 01:21:13 GMT  
		Size: 688.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea2050f99c3896ed695883c76758336c4ecd84fe3786bea63595cf8c8a5e924`  
		Last Modified: Thu, 28 Oct 2021 01:21:14 GMT  
		Size: 9.7 KB (9675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b4ef7dd35d03fff1004952f01b94fddaf7839e8b22f6726e34665b9adb3fbb`  
		Last Modified: Thu, 28 Oct 2021 01:21:13 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b55e8eb5f9387ee0a9aaf2f71223a594b3ac069f211d5b9b30e69c68a22372a`  
		Last Modified: Thu, 28 Oct 2021 01:21:13 GMT  
		Size: 10.6 KB (10637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:830a1b0e8f739453bb9363f4732cc496199f5520aee78917ff8e2e1874850d68`  
		Last Modified: Thu, 28 Oct 2021 01:21:14 GMT  
		Size: 2.5 MB (2530872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.9-kernel-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:47ca2f543ffd735cb741798cb9ff278cd26416284d6b652cdae1b2a6094a6e06
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115548331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f711f1edc66d03da8efdeecba4bbe5da4f53750adaf0f5c9601ce7683d0978e`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:54:47 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 00:55:56 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Oct 2021 01:45:21 GMT
ENV JAVA_VERSION=jdk-11.0.12+7_openj9-0.27.0
# Thu, 21 Oct 2021 01:48:48 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='285bd388a497db61408d26a9f3328f62004714ede94456718cf6440a109e25d2';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_ppc64le_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        s390x)          ESUM='6e5829aeb37abfb122e0944e438ecb2043c56df14fcdcce39bd4e3c9a55571a8';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_s390x_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        amd64|x86_64)          ESUM='f352998f6fdf0b84f63c563608be57f30aa3f14c8117c1219422dbc712ad4f81';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_x64_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 21 Oct 2021 01:49:04 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 21 Oct 2021 01:49:23 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 21 Oct 2021 01:50:18 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 26 Oct 2021 00:02:27 GMT
ARG VERBOSE=false
# Tue, 26 Oct 2021 00:02:29 GMT
ARG OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:17:26 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Tue, 26 Oct 2021 00:17:31 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Tue, 26 Oct 2021 00:17:34 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Tue, 26 Oct 2021 00:17:37 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 26 Oct 2021 00:17:40 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Tue, 26 Oct 2021 00:17:43 GMT
ARG LIBERTY_URL
# Tue, 26 Oct 2021 00:17:47 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 26 Oct 2021 00:18:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 26 Oct 2021 00:18:21 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 26 Oct 2021 00:18:23 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Tue, 26 Oct 2021 00:18:24 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:18:29 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 26 Oct 2021 00:18:30 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 26 Oct 2021 00:18:31 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 26 Oct 2021 00:18:38 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 26 Oct 2021 00:18:55 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 26 Oct 2021 00:18:59 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 26 Oct 2021 00:19:03 GMT
USER 1001
# Tue, 26 Oct 2021 00:19:06 GMT
EXPOSE 9080 9443
# Tue, 26 Oct 2021 00:19:08 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 26 Oct 2021 00:19:10 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c930749dacf55e37561edab7967f5a2f51660034fee0da501c2d71cb783301`  
		Last Modified: Sat, 16 Oct 2021 01:03:26 GMT  
		Size: 17.2 MB (17210510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d519f9110a27224937cddf5826128ca092be8957e9a8c13546df0dc596ba42`  
		Last Modified: Thu, 21 Oct 2021 02:03:00 GMT  
		Size: 45.1 MB (45107808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afebfecbc9bc8dad01d6486a0e236777ff1b2a82229ff13363f70a0827f07160`  
		Last Modified: Thu, 21 Oct 2021 02:02:53 GMT  
		Size: 3.3 MB (3286490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2bbb876c50debfd5a770b2a023253c6b5841b51140118fdf1555ffc5f3196d`  
		Last Modified: Tue, 26 Oct 2021 00:46:02 GMT  
		Size: 14.2 MB (14155026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140048859b8a73b0a7702df71cf44d9a50883ea7827ed8d03706c4746dc12263`  
		Last Modified: Tue, 26 Oct 2021 00:45:57 GMT  
		Size: 697.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b686649f8d628437ccdfecad3a80c0dcdd3a793bdde05bdc592de982cd11bc2a`  
		Last Modified: Tue, 26 Oct 2021 00:45:57 GMT  
		Size: 9.7 KB (9672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226708f83081b74fc92b8f84783cc66376a275ff0d2e8b3aec2fabea730e3ec2`  
		Last Modified: Tue, 26 Oct 2021 00:45:57 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f2bafacacaceecd1d395d593f7acd69511203ba36df026fa2c5615062d0e6e`  
		Last Modified: Tue, 26 Oct 2021 00:45:57 GMT  
		Size: 10.7 KB (10660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b033eb87d2f3e8019ad942a2e334e3a5f96e35bd726204627a3c276920e14db`  
		Last Modified: Tue, 26 Oct 2021 00:45:57 GMT  
		Size: 2.5 MB (2479958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.9-kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:2338aaebd83061370e53b106a9307914cb35c7fa3dfa354ebf0b2d038dfcf025
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107679987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:049198f60a7814136e12478609dda4bcb8ff50fe1f0219bb9ef0d3863b779171`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:58:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 00:58:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 00:58:27 GMT
ENV JAVA_VERSION=jdk-11.0.13+8_openj9-0.29.0
# Thu, 28 Oct 2021 00:59:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='3615940d4b26e8d11ff927dbf620a5247caecd84ba24c9d67f0e8b30ff463998';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_ppc64le_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        s390x)          ESUM='e942c0806163bbabe0b7ec8e630319489da400d58cd390011fc28428f468558e';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_s390x_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        amd64|x86_64)          ESUM='78eb54af15fac39eb2d254f51f0302aa213d3ad838f17766a9d081ca783edff4';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_x64_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 28 Oct 2021 00:59:28 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 00:59:28 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 28 Oct 2021 01:00:01 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 28 Oct 2021 01:43:09 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:43:09 GMT
ARG OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:48:08 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Thu, 28 Oct 2021 01:48:08 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Thu, 28 Oct 2021 01:48:08 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Thu, 28 Oct 2021 01:48:08 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 28 Oct 2021 01:48:08 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Thu, 28 Oct 2021 01:48:08 GMT
ARG LIBERTY_URL
# Thu, 28 Oct 2021 01:48:08 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 28 Oct 2021 01:48:18 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 01:48:18 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 01:48:18 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Thu, 28 Oct 2021 01:48:18 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:48:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 28 Oct 2021 01:48:19 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Thu, 28 Oct 2021 01:48:19 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 28 Oct 2021 01:48:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 28 Oct 2021 01:48:25 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 28 Oct 2021 01:48:25 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 28 Oct 2021 01:48:25 GMT
USER 1001
# Thu, 28 Oct 2021 01:48:25 GMT
EXPOSE 9080 9443
# Thu, 28 Oct 2021 01:48:25 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 28 Oct 2021 01:48:25 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276dbe4459a060d2c186c43e5e92d98fa6f181617c55cce69da393b9d5dd6200`  
		Last Modified: Sat, 16 Oct 2021 01:01:03 GMT  
		Size: 15.7 MB (15742080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bef20936d077045a96f4b0694d1470b79e8825348eb06b3a0ef4207079d17d`  
		Last Modified: Thu, 28 Oct 2021 01:02:07 GMT  
		Size: 43.8 MB (43800069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8547dc44147bfe37bde98eef473a2916985469204db561ebefa3e3d92fee029a`  
		Last Modified: Thu, 28 Oct 2021 01:02:01 GMT  
		Size: 4.3 MB (4284720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1f40bdf8d3065335a6711be483011d3a2c6db876d44c02fe7b0809ec2386d4`  
		Last Modified: Thu, 28 Oct 2021 01:58:41 GMT  
		Size: 14.2 MB (14154247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2506960ba73954b1b9e3f1d70ab192fd19e66d138ca46a041fffc31ec2f3a2`  
		Last Modified: Thu, 28 Oct 2021 01:58:38 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cd49c1312502c3c1dfaa88066867c9ca17bdfcf1b9337e6295916d25d3125e`  
		Last Modified: Thu, 28 Oct 2021 01:58:39 GMT  
		Size: 9.7 KB (9673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d8529abd76153ce49ed0735547223bfa11751320827d0c34e0f65e15dda7ef`  
		Last Modified: Thu, 28 Oct 2021 01:58:38 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3c3f709c7c595ddeed628c390ea5f713025fc0afbec8a64cce8d0fe58cf465`  
		Last Modified: Thu, 28 Oct 2021 01:58:39 GMT  
		Size: 10.6 KB (10633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7061f36639c9e42ab9b73bb51e5cb1d667c32172d5f968e3dd87c8e72b6f269`  
		Last Modified: Thu, 28 Oct 2021 01:58:39 GMT  
		Size: 2.6 MB (2556747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.9-kernel-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:898447df484f7e95f7b1d65595022cd655b6b078602938e1c0d4f374d7e14143
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.9-kernel-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:5e08e7742d575a51eef730e5f84772c94f3f8b828adea4c9b491a5b673140dd5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.1 MB (178062040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c910292986937cbdf267b9c508944381262179114caf4eafe13d97052c93fe0`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:55:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 02:55:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:55:32 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 02:56:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:56:08 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 01 Oct 2021 07:13:40 GMT
ARG VERBOSE=false
# Fri, 01 Oct 2021 07:13:40 GMT
ARG OPENJ9_SCC=true
# Fri, 01 Oct 2021 07:13:41 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Fri, 01 Oct 2021 07:13:41 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Fri, 01 Oct 2021 07:13:41 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Mon, 25 Oct 2021 22:48:12 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 22:48:12 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Mon, 25 Oct 2021 22:48:12 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 22:48:13 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 25 Oct 2021 22:48:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 25 Oct 2021 22:48:23 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Oct 2021 22:48:23 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Mon, 25 Oct 2021 22:48:24 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:48:25 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 25 Oct 2021 22:48:25 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Mon, 25 Oct 2021 22:48:25 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 25 Oct 2021 22:48:26 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 25 Oct 2021 22:48:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 25 Oct 2021 22:48:39 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Mon, 25 Oct 2021 22:48:39 GMT
USER 1001
# Mon, 25 Oct 2021 22:48:39 GMT
EXPOSE 9080 9443
# Mon, 25 Oct 2021 22:48:39 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 25 Oct 2021 22:48:40 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf7ef5b4a4700901695d7489ffa25c9a36a0c54f7003664412a2a582dd362fa`  
		Last Modified: Fri, 01 Oct 2021 02:59:16 GMT  
		Size: 3.0 MB (2959872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58286f2e604db89582fc1898b2d2a229d5920927e7705c94e32f38a70e29902e`  
		Last Modified: Fri, 01 Oct 2021 02:59:26 GMT  
		Size: 128.4 MB (128395032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6b34b3fe1e2ac672fb71a817fa7b6266bbe76d88da83b6e38aaa6c20d9e05f`  
		Last Modified: Mon, 25 Oct 2021 23:06:43 GMT  
		Size: 14.1 MB (14055841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff676a6e06f8f0ab9ebb31c8abad4db4a81934bd7bd8bc3d0ac484b962eeabc7`  
		Last Modified: Mon, 25 Oct 2021 23:06:40 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be89447c7cd07521bfc85588c50472f60c408f7facd9fb0fb237a16b6acdfcb`  
		Last Modified: Mon, 25 Oct 2021 23:06:40 GMT  
		Size: 9.7 KB (9679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b208b084380a5fccc395ee069904ea3f308e4ea6897282cebcc63517746c6f`  
		Last Modified: Mon, 25 Oct 2021 23:06:40 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d43a88abc25a0df6edd20918a59d54bc350863b51ef4ddddb8df459c7395f34`  
		Last Modified: Mon, 25 Oct 2021 23:06:40 GMT  
		Size: 10.7 KB (10656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948bc49342b1aba0c5ffefd707205d45ee8098d91243daf584073879cb867159`  
		Last Modified: Mon, 25 Oct 2021 23:06:41 GMT  
		Size: 5.9 MB (5924912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.9-kernel-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:343e218e07b0601846dfe12146a7527ef41ef5d7ce4bd92ad9d2d2021b82ac87
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.8 MB (180811105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4be0c42e2c116e9af18185c36274f6a58369244844be1d8e77a47ef87d91688`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 17:55:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Oct 2021 17:56:05 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 17:56:16 GMT
ENV JAVA_VERSION=8.0.6.36
# Wed, 06 Oct 2021 17:57:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Oct 2021 17:57:38 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 07 Oct 2021 10:35:31 GMT
ARG VERBOSE=false
# Thu, 07 Oct 2021 10:35:33 GMT
ARG OPENJ9_SCC=true
# Thu, 07 Oct 2021 10:35:37 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Thu, 07 Oct 2021 10:35:40 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Thu, 07 Oct 2021 10:35:44 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Tue, 26 Oct 2021 00:15:30 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 26 Oct 2021 00:15:33 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Tue, 26 Oct 2021 00:15:41 GMT
ARG LIBERTY_URL
# Tue, 26 Oct 2021 00:15:44 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 26 Oct 2021 00:16:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 26 Oct 2021 00:16:16 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 26 Oct 2021 00:16:19 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Tue, 26 Oct 2021 00:16:22 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:16:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 26 Oct 2021 00:16:29 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 26 Oct 2021 00:16:30 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 26 Oct 2021 00:16:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 26 Oct 2021 00:17:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 26 Oct 2021 00:17:04 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 26 Oct 2021 00:17:08 GMT
USER 1001
# Tue, 26 Oct 2021 00:17:10 GMT
EXPOSE 9080 9443
# Tue, 26 Oct 2021 00:17:12 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 26 Oct 2021 00:17:15 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce6e130fd3d09fd3fe6d741e0fa3f77120aa82717cf6d0a1cb49439939243a6`  
		Last Modified: Wed, 06 Oct 2021 18:04:08 GMT  
		Size: 3.1 MB (3081580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8fc8962750bc0e8c7c6ca6d1498e303c66e1f0b3f9613d204da9abf0200933`  
		Last Modified: Wed, 06 Oct 2021 18:04:22 GMT  
		Size: 127.9 MB (127898987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f55a4db9d34cf93dd60782337c13c76c8ee005bf5339aa599e11a4327f187f`  
		Last Modified: Tue, 26 Oct 2021 00:45:49 GMT  
		Size: 14.1 MB (14056411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8eeb13a7ada163c02afc93c5e69bde8338b653b68b154a43f6ecd1387e58ae`  
		Last Modified: Tue, 26 Oct 2021 00:45:45 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76fb073018ee13c91d1b735c3b7cb2d598bffe904df702f8a3449a44b2c1ab8`  
		Last Modified: Tue, 26 Oct 2021 00:45:45 GMT  
		Size: 9.7 KB (9678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d3691144cafeb2afb474b28084deaa7c58e8e8303e1eab03a62f6d8fd614a7`  
		Last Modified: Tue, 26 Oct 2021 00:45:45 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4730641c79dd1259bea562e04a9f1055cfa2c2ca5be6c48fdb49666d6d9f8c3a`  
		Last Modified: Tue, 26 Oct 2021 00:45:45 GMT  
		Size: 10.7 KB (10654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e1c01f839290ab733d015d2333f4d63bb4fec50d5ae49cb400108993b575b4`  
		Last Modified: Tue, 26 Oct 2021 00:45:46 GMT  
		Size: 5.3 MB (5319906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.9-kernel-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:debab2ecdcd5b840fe3d88d67958e49f26a4eeb8fcf9f8ccfec3fe547f6ec21f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.3 MB (173344866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:435acdb6bcfb830b674cdc808917642c22f9c11cbc2725336e1805050301943f`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:17 GMT
ADD file:d248d4b5739ee5d07e920ec481dc4af81b314aa52e64618322197a642394a41d in / 
# Fri, 01 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:23:32 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 02:23:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:23:37 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 02:24:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:24:19 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 01 Oct 2021 03:40:55 GMT
ARG VERBOSE=false
# Fri, 01 Oct 2021 03:40:55 GMT
ARG OPENJ9_SCC=true
# Fri, 01 Oct 2021 03:40:55 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Fri, 01 Oct 2021 03:40:55 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Fri, 01 Oct 2021 03:40:56 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Mon, 25 Oct 2021 22:22:13 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 22:22:13 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Mon, 25 Oct 2021 22:22:13 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 22:22:13 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 25 Oct 2021 22:22:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 25 Oct 2021 22:22:23 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Oct 2021 22:22:23 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Mon, 25 Oct 2021 22:22:23 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:22:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 25 Oct 2021 22:22:24 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Mon, 25 Oct 2021 22:22:24 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 25 Oct 2021 22:22:25 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 25 Oct 2021 22:22:32 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 25 Oct 2021 22:22:32 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Mon, 25 Oct 2021 22:22:33 GMT
USER 1001
# Mon, 25 Oct 2021 22:22:33 GMT
EXPOSE 9080 9443
# Mon, 25 Oct 2021 22:22:33 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 25 Oct 2021 22:22:33 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:97372e5b313b6b8bab9913de546bc50f73818d8275c94fc6491993c97b9d8bad`  
		Last Modified: Fri, 01 Oct 2021 01:43:49 GMT  
		Size: 25.4 MB (25362918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf425722012c2264c66ba97a53ff25a2f196330fbcc0872474e5e4562fa95f0`  
		Last Modified: Fri, 01 Oct 2021 02:27:43 GMT  
		Size: 2.7 MB (2676365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d432d8be662b9a55c0dfed6d79d328a62b58be822a9888d1b7d0d16dc6c248`  
		Last Modified: Fri, 01 Oct 2021 02:27:51 GMT  
		Size: 125.4 MB (125395531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1c407fef21834b60347997a27a33dd46260bb9a0dbd74913531b9bfa1018d7`  
		Last Modified: Mon, 25 Oct 2021 22:41:32 GMT  
		Size: 14.1 MB (14055683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e69603ecc97823e1c3e2fdd733acb6cc44a73d9a8789630027470157eb50624`  
		Last Modified: Mon, 25 Oct 2021 22:41:30 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd84e34c2ee9ac1b31a1eb011b616fdc23f2095245ccaa7abc7f9fd4ad5b4cc`  
		Last Modified: Mon, 25 Oct 2021 22:41:30 GMT  
		Size: 9.7 KB (9676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6729e19b1db5910b295b3eceb90cd56fb7453af5ba2b16cce7d3ed6093233a0`  
		Last Modified: Mon, 25 Oct 2021 22:41:30 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6906524465d542cc5f411e1de178ff5e0cfcd028e0a6e8ed38d9a339abb34db`  
		Last Modified: Mon, 25 Oct 2021 22:41:30 GMT  
		Size: 10.7 KB (10657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3a668e776118ad579c7d124d53ba234b2f4ea142c908ddf9696032b4ae29dc`  
		Last Modified: Mon, 25 Oct 2021 22:41:31 GMT  
		Size: 5.8 MB (5833067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:full`

```console
$ docker pull websphere-liberty@sha256:942c68a160909bd10112af6af1a2ee0e17566295dc3030e8ecace60c75f14397
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:b1115005499014bf1a10d5355e4d098ba6f4226783f08ea11272c326186fdd7f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.3 MB (403315070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf37216acf115eb9b9aff1a9f65dffc623e75c16a56cb1584bfd62ccf90a8094`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:55:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 02:55:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:55:32 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 02:56:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:56:08 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 01 Oct 2021 07:13:40 GMT
ARG VERBOSE=false
# Fri, 01 Oct 2021 07:13:40 GMT
ARG OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:39:24 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Mon, 25 Oct 2021 22:39:24 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Mon, 25 Oct 2021 22:39:24 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Mon, 25 Oct 2021 22:39:24 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 22:39:24 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Mon, 25 Oct 2021 22:39:25 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 22:39:25 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 25 Oct 2021 22:39:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 25 Oct 2021 22:39:42 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Oct 2021 22:39:42 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Mon, 25 Oct 2021 22:39:42 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:39:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 25 Oct 2021 22:39:44 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Mon, 25 Oct 2021 22:39:44 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 25 Oct 2021 22:39:45 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 25 Oct 2021 22:39:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 25 Oct 2021 22:39:58 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Mon, 25 Oct 2021 22:39:58 GMT
USER 1001
# Mon, 25 Oct 2021 22:39:59 GMT
EXPOSE 9080 9443
# Mon, 25 Oct 2021 22:39:59 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 25 Oct 2021 22:39:59 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Mon, 25 Oct 2021 22:40:32 GMT
ARG VERBOSE=false
# Mon, 25 Oct 2021 22:40:32 GMT
ARG REPOSITORIES_PROPERTIES=
# Mon, 25 Oct 2021 22:43:34 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Mon, 25 Oct 2021 22:43:35 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Mon, 25 Oct 2021 22:44:22 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf7ef5b4a4700901695d7489ffa25c9a36a0c54f7003664412a2a582dd362fa`  
		Last Modified: Fri, 01 Oct 2021 02:59:16 GMT  
		Size: 3.0 MB (2959872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58286f2e604db89582fc1898b2d2a229d5920927e7705c94e32f38a70e29902e`  
		Last Modified: Fri, 01 Oct 2021 02:59:26 GMT  
		Size: 128.4 MB (128395032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb130bd160d991d174701aa1d12d4c1f75c81705bd6ae5b036ae6e50a248d88e`  
		Last Modified: Mon, 25 Oct 2021 23:05:29 GMT  
		Size: 14.1 MB (14072794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7beabf2dd59365e93d8abbb027ae0f1b98d39e3ea91de31bded58a8c1f92448`  
		Last Modified: Mon, 25 Oct 2021 23:05:25 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f040313f6379bc9c04a2b94631e0bf2906ed5a99289186e898117021c507384`  
		Last Modified: Mon, 25 Oct 2021 23:05:26 GMT  
		Size: 9.7 KB (9677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fe7348629a8b7a683f0e06d11fd83be6b5349bfcecda69c0e3aac2d45ec8ae`  
		Last Modified: Mon, 25 Oct 2021 23:05:25 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054c2e49311baee037b9f9b7a4c1860cc61c840b03b81c38b83a63dac906a86d`  
		Last Modified: Mon, 25 Oct 2021 23:05:25 GMT  
		Size: 10.7 KB (10667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e464e836a01729d2494c3dc860e6e078d5d69fe1819cc5a4b8c9042c73d6a4`  
		Last Modified: Mon, 25 Oct 2021 23:05:26 GMT  
		Size: 5.9 MB (5869965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c845db47bbb20043cf2fd0baed54e15d4fdcc9659d3028b0d1ac7de9f87084f`  
		Last Modified: Mon, 25 Oct 2021 23:05:58 GMT  
		Size: 209.3 MB (209275727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c30de2c69d7ebc9cdb54e55b3d6a59437590a6fe6567f3bdf252ad06f6cd7d`  
		Last Modified: Mon, 25 Oct 2021 23:05:47 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b9160a1a04cb7a1afff92f9ceee48a39b1138f6751e1b860b52fe4e1c2236b`  
		Last Modified: Mon, 25 Oct 2021 23:05:49 GMT  
		Size: 16.0 MB (16014336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; 386

```console
$ docker pull websphere-liberty@sha256:c847143995aec30ca5d4526544d7c41ca7a42a8baf8195848864d0128e96ecf3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.2 MB (349209019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6d2c9374be56a63d6e35820fec8676f2d4ed2b9bdaf09a49c8545b039479bb7`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 18:38:55 GMT
ADD file:d859d389e38b7ac70fd56f97e38d52a77b58e72b96237a4302d1984cdd912a55 in / 
# Fri, 20 Mar 2020 18:38:56 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:38:57 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:38:58 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:38:58 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:06:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 20 Mar 2020 19:06:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:06:42 GMT
ENV JAVA_VERSION=1.8.0_sr6fp6
# Fri, 20 Mar 2020 19:07:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='87f9d45b7e1fa65ec018479f3ca7da69a03b52b0da10b8d1555142eec8ab0093';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='b5f825047c9bb5d360fb83694f12e17b1a5a15abf94ac82cd0a3aea32c9a361c';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='f3c04cd07ef269c24373840eae6f59c7db7a16d2e206d393ba93efa6dbb8d74f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2bbefda96f7d1a5f1694893961e92ccc59dfa50375ae5450675d7a4213d5812e';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='d5b0508d53d1c7382c06f5bc1daf3d57c19c70d851e86e6b1162bcd93f616f7e';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 20 Mar 2020 19:07:26 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 20 Mar 2020 19:31:53 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.3 org.opencontainers.image.revision=cl200320200305-1433
# Fri, 20 Mar 2020 19:31:53 GMT
ENV LIBERTY_VERSION=20.0.0_03
# Fri, 20 Mar 2020 19:31:53 GMT
ARG LIBERTY_URL
# Fri, 20 Mar 2020 19:31:53 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 20 Mar 2020 19:32:02 GMT
# ARGS: DOWNLOAD_OPTIONS=
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:32:03 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:32:03 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.3 BuildLabel=cl200320200305-1433
# Fri, 20 Mar 2020 19:32:03 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output
# Fri, 20 Mar 2020 19:32:04 GMT
# ARGS: DOWNLOAD_OPTIONS=
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 20 Mar 2020 19:32:04 GMT
COPY dir:0d0cedab2fbb7208b9d81afa78e9f15b12b71232224a2fe9753c00b7b72bd72e in /opt/ibm/helpers/ 
# Fri, 20 Mar 2020 19:32:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 20 Mar 2020 19:32:05 GMT
COPY dir:9277507d983008afcf8df6e0bfe2735bd4e92717515dbb3a7e268c830f213489 in /licenses/ 
# Fri, 20 Mar 2020 19:32:06 GMT
# ARGS: DOWNLOAD_OPTIONS=
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 20 Mar 2020 19:32:06 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 20 Mar 2020 19:32:06 GMT
USER 1001
# Fri, 20 Mar 2020 19:32:06 GMT
EXPOSE 9080 9443
# Fri, 20 Mar 2020 19:32:07 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 20 Mar 2020 19:32:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 20 Mar 2020 19:32:10 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 20 Mar 2020 19:35:01 GMT
# ARGS: REPOSITORIES_PROPERTIES=
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Fri, 20 Mar 2020 19:35:01 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
```

-	Layers:
	-	`sha256:765ce743592771b94ad8ff27e281e66c13f6039962c7dde4dbe47123081e015b`  
		Last Modified: Mon, 16 Mar 2020 15:38:41 GMT  
		Size: 27.1 MB (27122453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dc9c4739090a3d2f7265f1f8184b1cbd8ae133b863f8aa93ec5cf1761ee7a5`  
		Last Modified: Fri, 20 Mar 2020 18:39:35 GMT  
		Size: 34.6 KB (34625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a5b698281c077f48fc598e698f0619e4d00a2fedc1832fc95e9cf281408f63`  
		Last Modified: Fri, 20 Mar 2020 18:39:34 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaebe599891b1e1befc10d752a117cc5615ec2dd3913d399fd66e26e0cace3e5`  
		Last Modified: Fri, 20 Mar 2020 18:39:34 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f829150bc8a53a37ac17eb34838fa33c990881a4031bc650a9dae26b3f7880e`  
		Last Modified: Fri, 20 Mar 2020 19:09:23 GMT  
		Size: 3.0 MB (2992132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17b9ccc4baf3a1ffa517a03c7c3d01900136b128b36a83558c67c42e6c1cbaa`  
		Last Modified: Fri, 20 Mar 2020 19:09:35 GMT  
		Size: 118.8 MB (118756706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5011972f1876d464fb62206211a5b5e162ba2603bf20fc4cd0f2b4ffd311cd9`  
		Last Modified: Fri, 20 Mar 2020 19:39:16 GMT  
		Size: 13.6 MB (13600436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5395b713d5baa0917182ca82077b6fa2a0c51789907f96cbb12455586d9fa9b`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389324a3d9489b2fbcd5946f9d24285c0171c3218470e4a5e2d45c731cefc522`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 3.5 KB (3515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38ea596499e1f23ce426826250984869e92da50aec5845a6233a76d7764bfd1`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea3197b55235384f836e31a605c460f6cb7196f68dc29c65640738d8aa50188`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 57.4 KB (57426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683f76bf565cdb9e59c325f24357eb6b164555ed8629a4b8383448239608966d`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 4.4 KB (4358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cd2560c76831311d13d197b4784e0826f6ffae62e3b9a22d2fa5675b9b71a2`  
		Last Modified: Fri, 20 Mar 2020 19:39:42 GMT  
		Size: 186.6 MB (186634496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9891aa2b3e904f8f514677372187983ac12c98c209c433ab5bf0862e09d6f4ef`  
		Last Modified: Fri, 20 Mar 2020 19:39:20 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:3ebbd27afd1c227833f438d21f9636d883949eb2b952f08fdd6e0ba66b7dd4ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.0 MB (403966097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c78740a0ed156d7ac4d80645081da020f7c953c822c860f315773a5411af4e92`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 17:55:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Oct 2021 17:56:05 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 17:56:16 GMT
ENV JAVA_VERSION=8.0.6.36
# Wed, 06 Oct 2021 17:57:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Oct 2021 17:57:38 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 07 Oct 2021 10:35:31 GMT
ARG VERBOSE=false
# Thu, 07 Oct 2021 10:35:33 GMT
ARG OPENJ9_SCC=true
# Mon, 25 Oct 2021 23:59:34 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Mon, 25 Oct 2021 23:59:39 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Mon, 25 Oct 2021 23:59:43 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Mon, 25 Oct 2021 23:59:46 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 23:59:51 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Mon, 25 Oct 2021 23:59:54 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 23:59:57 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 26 Oct 2021 00:00:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 26 Oct 2021 00:00:59 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 26 Oct 2021 00:01:02 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Tue, 26 Oct 2021 00:01:07 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:01:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 26 Oct 2021 00:01:22 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 26 Oct 2021 00:01:23 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 26 Oct 2021 00:01:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 26 Oct 2021 00:01:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 26 Oct 2021 00:01:56 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 26 Oct 2021 00:01:59 GMT
USER 1001
# Tue, 26 Oct 2021 00:02:02 GMT
EXPOSE 9080 9443
# Tue, 26 Oct 2021 00:02:04 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 26 Oct 2021 00:02:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 26 Oct 2021 00:04:38 GMT
ARG VERBOSE=false
# Tue, 26 Oct 2021 00:04:41 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 26 Oct 2021 00:08:18 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 26 Oct 2021 00:08:26 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 26 Oct 2021 00:09:32 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce6e130fd3d09fd3fe6d741e0fa3f77120aa82717cf6d0a1cb49439939243a6`  
		Last Modified: Wed, 06 Oct 2021 18:04:08 GMT  
		Size: 3.1 MB (3081580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8fc8962750bc0e8c7c6ca6d1498e303c66e1f0b3f9613d204da9abf0200933`  
		Last Modified: Wed, 06 Oct 2021 18:04:22 GMT  
		Size: 127.9 MB (127898987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd371e52f22155313b0f3ae5f5c13597ca17fa0417c214eaf1e16df95bb678a8`  
		Last Modified: Tue, 26 Oct 2021 00:44:12 GMT  
		Size: 14.1 MB (14073366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee227af6d9277d187f05bd7fe3a7148fc127fd5be9bc040db19738760f9c12f`  
		Last Modified: Tue, 26 Oct 2021 00:44:08 GMT  
		Size: 697.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984133fc0355d34799cda371d5d2a8153e614767af49aa3cb7f8c98414e18950`  
		Last Modified: Tue, 26 Oct 2021 00:44:08 GMT  
		Size: 9.7 KB (9677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f9cacb1facc8e3097f176849d860aef3b7ebd23f9c9114047be96ca087ba97`  
		Last Modified: Tue, 26 Oct 2021 00:44:08 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfced5f1e31cfb68f3450e4211967c2c966cecdef7ccb633cb8a52a2c0cc710`  
		Last Modified: Tue, 26 Oct 2021 00:44:08 GMT  
		Size: 10.7 KB (10670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281fb76285f797555b5334b1d7f5596ec01e7137a6d55e8f31365b9fe39c2352`  
		Last Modified: Tue, 26 Oct 2021 00:44:09 GMT  
		Size: 5.3 MB (5339397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4562f8c3c1dade81475edf6207aea4f9c941c6b7c037c67810ebd4ee1c8098a3`  
		Last Modified: Tue, 26 Oct 2021 00:44:52 GMT  
		Size: 209.3 MB (209276516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09802a7cb8ad05d0191cf0a29e24e2e79b4306e2654390c0460db8311b15baa4`  
		Last Modified: Tue, 26 Oct 2021 00:44:33 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfae2d34298fb1bd2f919e6859a8e487b8d641e70379ba24107b763ad45558fe`  
		Last Modified: Tue, 26 Oct 2021 00:44:35 GMT  
		Size: 13.8 MB (13841061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:2456846170fe619056099175052bbc1115ade0e8a159250e76a21941cae6068d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.3 MB (398292262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed3ce5d13fb58bdf360ce6367ee827a0b76c2b099e4a24a7d693097f201d5545`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:17 GMT
ADD file:d248d4b5739ee5d07e920ec481dc4af81b314aa52e64618322197a642394a41d in / 
# Fri, 01 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:23:32 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 02:23:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:23:37 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 02:24:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:24:19 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 01 Oct 2021 03:40:55 GMT
ARG VERBOSE=false
# Fri, 01 Oct 2021 03:40:55 GMT
ARG OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:12:45 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Mon, 25 Oct 2021 22:12:45 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Mon, 25 Oct 2021 22:12:45 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Mon, 25 Oct 2021 22:12:45 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 22:12:45 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Mon, 25 Oct 2021 22:12:45 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 22:12:45 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 25 Oct 2021 22:12:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 25 Oct 2021 22:12:57 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Oct 2021 22:12:57 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Mon, 25 Oct 2021 22:12:57 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:12:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 25 Oct 2021 22:12:58 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Mon, 25 Oct 2021 22:12:58 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 25 Oct 2021 22:12:59 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 25 Oct 2021 22:13:06 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 25 Oct 2021 22:13:07 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Mon, 25 Oct 2021 22:13:07 GMT
USER 1001
# Mon, 25 Oct 2021 22:13:07 GMT
EXPOSE 9080 9443
# Mon, 25 Oct 2021 22:13:07 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 25 Oct 2021 22:13:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Mon, 25 Oct 2021 22:13:39 GMT
ARG VERBOSE=false
# Mon, 25 Oct 2021 22:13:40 GMT
ARG REPOSITORIES_PROPERTIES=
# Mon, 25 Oct 2021 22:17:03 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Mon, 25 Oct 2021 22:17:07 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Mon, 25 Oct 2021 22:17:31 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:97372e5b313b6b8bab9913de546bc50f73818d8275c94fc6491993c97b9d8bad`  
		Last Modified: Fri, 01 Oct 2021 01:43:49 GMT  
		Size: 25.4 MB (25362918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf425722012c2264c66ba97a53ff25a2f196330fbcc0872474e5e4562fa95f0`  
		Last Modified: Fri, 01 Oct 2021 02:27:43 GMT  
		Size: 2.7 MB (2676365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d432d8be662b9a55c0dfed6d79d328a62b58be822a9888d1b7d0d16dc6c248`  
		Last Modified: Fri, 01 Oct 2021 02:27:51 GMT  
		Size: 125.4 MB (125395531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969119abed0aabe761027277ec6fb7718eba553a1b072f7b1c13fbc7ad2643ce`  
		Last Modified: Mon, 25 Oct 2021 22:40:41 GMT  
		Size: 14.1 MB (14072637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6345425373ca667c20a30007a8292172e2b4eab13044ca41d184e4af52ff61e6`  
		Last Modified: Mon, 25 Oct 2021 22:40:39 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371f939cc39d32f824f40420cc6c72cee355cfa91155275e712b4632b2f7bc05`  
		Last Modified: Mon, 25 Oct 2021 22:40:39 GMT  
		Size: 9.7 KB (9674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f290e6c52139c0593dbbcd890fbc67f5b59bb711b97ea14886a2833a5a49ff93`  
		Last Modified: Mon, 25 Oct 2021 22:40:39 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4389715a5776e4d60e9b0bd807528101d253d83f6a4f2e5f9da17258ad41422c`  
		Last Modified: Mon, 25 Oct 2021 22:40:39 GMT  
		Size: 10.7 KB (10660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d732cb763586ba0cd58e22ae8ca4d3c4051b7370e0a5b974869d092a0d3a6b`  
		Last Modified: Mon, 25 Oct 2021 22:40:40 GMT  
		Size: 5.9 MB (5868523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3471c7e056a5f605febd60fea600313267b0f15c9c8449d042119817212638bb`  
		Last Modified: Mon, 25 Oct 2021 22:41:02 GMT  
		Size: 209.3 MB (209276442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb25227e9262c819dd066fb48ebfc7b4e86cfe76a0939caf9895ac2836c0531d`  
		Last Modified: Mon, 25 Oct 2021 22:40:53 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc404276fd2ceb3aac5a837f879edd92a65c6cdda45b95937e3ca3d7f1bd01c`  
		Last Modified: Mon, 25 Oct 2021 22:40:56 GMT  
		Size: 15.6 MB (15617590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:f302e727de207af2774e2caad973a7bfeb9ee8ba516da456ea351e6a2807ce86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:15feed4dc7fe993fe74f7e02fce21143cae99c216f53b6e166431cdef4efb951
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.0 MB (334021394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61e1afe72dcd950a54a6209229284c82128c471ef8fad65721b66261228bbedf`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:44:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 02:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 00:31:11 GMT
ENV JAVA_VERSION=jdk-11.0.13+8_openj9-0.29.0
# Thu, 28 Oct 2021 00:33:11 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='3615940d4b26e8d11ff927dbf620a5247caecd84ba24c9d67f0e8b30ff463998';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_ppc64le_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        s390x)          ESUM='e942c0806163bbabe0b7ec8e630319489da400d58cd390011fc28428f468558e';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_s390x_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        amd64|x86_64)          ESUM='78eb54af15fac39eb2d254f51f0302aa213d3ad838f17766a9d081ca783edff4';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_x64_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 28 Oct 2021 00:33:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 00:33:11 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 28 Oct 2021 00:33:47 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 28 Oct 2021 01:07:18 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:07:18 GMT
ARG OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:07:18 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Thu, 28 Oct 2021 01:07:19 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Thu, 28 Oct 2021 01:07:19 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Thu, 28 Oct 2021 01:07:19 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 28 Oct 2021 01:07:19 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Thu, 28 Oct 2021 01:07:19 GMT
ARG LIBERTY_URL
# Thu, 28 Oct 2021 01:07:19 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 28 Oct 2021 01:07:28 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 01:07:29 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 01:07:29 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Thu, 28 Oct 2021 01:07:29 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:07:30 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 28 Oct 2021 01:07:30 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Thu, 28 Oct 2021 01:07:30 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 28 Oct 2021 01:07:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 28 Oct 2021 01:07:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 28 Oct 2021 01:07:39 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 28 Oct 2021 01:07:39 GMT
USER 1001
# Thu, 28 Oct 2021 01:07:40 GMT
EXPOSE 9080 9443
# Thu, 28 Oct 2021 01:07:40 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 28 Oct 2021 01:07:40 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 28 Oct 2021 01:07:47 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:07:48 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 28 Oct 2021 01:10:50 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Thu, 28 Oct 2021 01:10:51 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 28 Oct 2021 01:11:27 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237daeb1ae282fe20092079ef6d5de7924746d0f2e9ad88797d08524a4d842fd`  
		Last Modified: Sat, 16 Oct 2021 02:47:20 GMT  
		Size: 16.0 MB (16036029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82607fdca83d197b118a35c377753995ef0400ef8de999ed3b8675d5fa58ce2f`  
		Last Modified: Thu, 28 Oct 2021 00:37:33 GMT  
		Size: 44.7 MB (44737093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7e4f4f21da9c3eec66f54b7ec452e3ccf00f68d74a7287bb1cbfbd68d2b041`  
		Last Modified: Thu, 28 Oct 2021 00:37:28 GMT  
		Size: 4.2 MB (4202694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f320c18438947d83dc1f15e75d6225b16e4030be2f3f60b723231f7d507fea`  
		Last Modified: Thu, 28 Oct 2021 01:20:39 GMT  
		Size: 14.2 MB (14171331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74f02207975af9dde28884f091d0c74f1c9360ecd847c1c009a8b0ed2033da3`  
		Last Modified: Thu, 28 Oct 2021 01:20:36 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478f97fe27905bdbf70a5179455b31a085d4398c4679c15e2f6c0e8fecbb9a58`  
		Last Modified: Thu, 28 Oct 2021 01:20:35 GMT  
		Size: 9.7 KB (9666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948ab830722710af86fa613d3fa37a082644901281103a071d74cebb6bd7a9ea`  
		Last Modified: Thu, 28 Oct 2021 01:20:35 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3379a5452b604a9a1debf912875f4ebd9f1e6e7cf9af825c2c4decde12d33d`  
		Last Modified: Thu, 28 Oct 2021 01:20:35 GMT  
		Size: 10.7 KB (10654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e1c3e8451879781f16eeb22bd489cb303f75fdd57586410b1682cd5680c4f4`  
		Last Modified: Thu, 28 Oct 2021 01:20:36 GMT  
		Size: 2.5 MB (2491575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2afc7dd7b2a11c2039016978a4e88ff295b2d5f6c887a29807539446c67791`  
		Last Modified: Thu, 28 Oct 2021 01:20:58 GMT  
		Size: 209.3 MB (209275582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8cb9274d195319b29b576a14b6f7e0c52ffa18af32e3ff3d7c81e22b204bbb`  
		Last Modified: Thu, 28 Oct 2021 01:20:47 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cec193b5ef149348342fe1d5bc3e439b7b840fb7d9e160ccae274082e717ca3`  
		Last Modified: Thu, 28 Oct 2021 01:20:49 GMT  
		Size: 14.5 MB (14517762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:67adfadf6d017abdac145015162d86f601564d0d056f07900bbb4a36a366fa84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.9 MB (337874654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f9a4d56a09dd4e30cd54eddcbafad347cc4d0a64f5ea5a0c71547097c93f82a`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:54:47 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 00:55:56 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Oct 2021 01:45:21 GMT
ENV JAVA_VERSION=jdk-11.0.12+7_openj9-0.27.0
# Thu, 21 Oct 2021 01:48:48 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='285bd388a497db61408d26a9f3328f62004714ede94456718cf6440a109e25d2';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_ppc64le_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        s390x)          ESUM='6e5829aeb37abfb122e0944e438ecb2043c56df14fcdcce39bd4e3c9a55571a8';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_s390x_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        amd64|x86_64)          ESUM='f352998f6fdf0b84f63c563608be57f30aa3f14c8117c1219422dbc712ad4f81';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_x64_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 21 Oct 2021 01:49:04 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 21 Oct 2021 01:49:23 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 21 Oct 2021 01:50:18 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 26 Oct 2021 00:02:27 GMT
ARG VERBOSE=false
# Tue, 26 Oct 2021 00:02:29 GMT
ARG OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:02:31 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Tue, 26 Oct 2021 00:02:33 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Tue, 26 Oct 2021 00:02:34 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Tue, 26 Oct 2021 00:02:35 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 26 Oct 2021 00:02:37 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Tue, 26 Oct 2021 00:02:40 GMT
ARG LIBERTY_URL
# Tue, 26 Oct 2021 00:02:42 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 26 Oct 2021 00:03:11 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 26 Oct 2021 00:03:14 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 26 Oct 2021 00:03:18 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Tue, 26 Oct 2021 00:03:23 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:03:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 26 Oct 2021 00:03:39 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 26 Oct 2021 00:03:40 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 26 Oct 2021 00:03:50 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 26 Oct 2021 00:04:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 26 Oct 2021 00:04:11 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 26 Oct 2021 00:04:14 GMT
USER 1001
# Tue, 26 Oct 2021 00:04:16 GMT
EXPOSE 9080 9443
# Tue, 26 Oct 2021 00:04:17 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 26 Oct 2021 00:04:19 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 26 Oct 2021 00:09:47 GMT
ARG VERBOSE=false
# Tue, 26 Oct 2021 00:09:53 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 26 Oct 2021 00:13:55 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 26 Oct 2021 00:14:00 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 26 Oct 2021 00:14:54 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c930749dacf55e37561edab7967f5a2f51660034fee0da501c2d71cb783301`  
		Last Modified: Sat, 16 Oct 2021 01:03:26 GMT  
		Size: 17.2 MB (17210510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d519f9110a27224937cddf5826128ca092be8957e9a8c13546df0dc596ba42`  
		Last Modified: Thu, 21 Oct 2021 02:03:00 GMT  
		Size: 45.1 MB (45107808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afebfecbc9bc8dad01d6486a0e236777ff1b2a82229ff13363f70a0827f07160`  
		Last Modified: Thu, 21 Oct 2021 02:02:53 GMT  
		Size: 3.3 MB (3286490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c959c7913b358daa8d638d574cfed5c19cc6fb4779f71b43debea7cb425f78`  
		Last Modified: Tue, 26 Oct 2021 00:44:25 GMT  
		Size: 14.2 MB (14171675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29638a4016c15c1f7a42994d97fb39804a5d41ae894b550b1353eb6ac21f45fb`  
		Last Modified: Tue, 26 Oct 2021 00:44:20 GMT  
		Size: 690.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91b025d347f73e0851038db7723a694dc2c472341019140169aa25a378a59a2`  
		Last Modified: Tue, 26 Oct 2021 00:44:20 GMT  
		Size: 9.7 KB (9670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56be72fe50f64e22ae2d25ba9f167dc85452ab42662d744b9124903f45eaa5bf`  
		Last Modified: Tue, 26 Oct 2021 00:44:20 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7340186166530eddc6450a7abcdeb1b9eab34407a9beb4a6ed3c513a95ba810f`  
		Last Modified: Tue, 26 Oct 2021 00:44:20 GMT  
		Size: 10.7 KB (10658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28516018017a50371e38a72026e7e2899fe67161aedd2bc9d3368ed652d4ccec`  
		Last Modified: Tue, 26 Oct 2021 00:44:21 GMT  
		Size: 2.5 MB (2475923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462aa0189a031a7bbcb306ad930bb28d61963cee9e9950aa7b1947a276784f05`  
		Last Modified: Tue, 26 Oct 2021 00:45:23 GMT  
		Size: 209.3 MB (209276177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519107cecbb8c60717229b031939efbc424b885dc07311b09022dc099c11867a`  
		Last Modified: Tue, 26 Oct 2021 00:45:04 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcaaf51bdc0275b006bd24a8346913db391b8610d655368da5160487618a02f3`  
		Last Modified: Tue, 26 Oct 2021 00:45:07 GMT  
		Size: 13.0 MB (13036592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:5253ca0dd20abc67573cfdeff50925fe9dd5599f50bcf349975eb598c12fa2f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.2 MB (331160402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23c05ce41ba5b2379e46381d07438a0c8e47ed3efb6dec86806ea2577bb7ce35`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:58:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 00:58:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 00:58:27 GMT
ENV JAVA_VERSION=jdk-11.0.13+8_openj9-0.29.0
# Thu, 28 Oct 2021 00:59:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='3615940d4b26e8d11ff927dbf620a5247caecd84ba24c9d67f0e8b30ff463998';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_ppc64le_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        s390x)          ESUM='e942c0806163bbabe0b7ec8e630319489da400d58cd390011fc28428f468558e';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_s390x_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        amd64|x86_64)          ESUM='78eb54af15fac39eb2d254f51f0302aa213d3ad838f17766a9d081ca783edff4';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_x64_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 28 Oct 2021 00:59:28 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 00:59:28 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 28 Oct 2021 01:00:01 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 28 Oct 2021 01:43:09 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:43:09 GMT
ARG OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:43:09 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Thu, 28 Oct 2021 01:43:09 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Thu, 28 Oct 2021 01:43:09 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Thu, 28 Oct 2021 01:43:09 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 28 Oct 2021 01:43:10 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Thu, 28 Oct 2021 01:43:10 GMT
ARG LIBERTY_URL
# Thu, 28 Oct 2021 01:43:10 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 28 Oct 2021 01:43:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 01:43:20 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 01:43:20 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Thu, 28 Oct 2021 01:43:20 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:43:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 28 Oct 2021 01:43:21 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Thu, 28 Oct 2021 01:43:21 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 28 Oct 2021 01:43:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 28 Oct 2021 01:43:26 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 28 Oct 2021 01:43:27 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 28 Oct 2021 01:43:27 GMT
USER 1001
# Thu, 28 Oct 2021 01:43:27 GMT
EXPOSE 9080 9443
# Thu, 28 Oct 2021 01:43:27 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 28 Oct 2021 01:43:27 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 28 Oct 2021 01:43:38 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:43:38 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 28 Oct 2021 01:47:03 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Thu, 28 Oct 2021 01:47:07 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 28 Oct 2021 01:47:29 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276dbe4459a060d2c186c43e5e92d98fa6f181617c55cce69da393b9d5dd6200`  
		Last Modified: Sat, 16 Oct 2021 01:01:03 GMT  
		Size: 15.7 MB (15742080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bef20936d077045a96f4b0694d1470b79e8825348eb06b3a0ef4207079d17d`  
		Last Modified: Thu, 28 Oct 2021 01:02:07 GMT  
		Size: 43.8 MB (43800069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8547dc44147bfe37bde98eef473a2916985469204db561ebefa3e3d92fee029a`  
		Last Modified: Thu, 28 Oct 2021 01:02:01 GMT  
		Size: 4.3 MB (4284720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8fe7f49f8a6320a829b59b87b8e6d2f5c623b8926fa5cbbd62cb3e14326e58`  
		Last Modified: Thu, 28 Oct 2021 01:58:02 GMT  
		Size: 14.2 MB (14170913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ea4b6d21bf75f5dc6643a5940ef5db23c15356b23f70a0adfcd0e80230ac8a`  
		Last Modified: Thu, 28 Oct 2021 01:57:59 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4198f3548e614a889bcf03b30adebe8652f6a27b339dde077ee4ebb8babfd2e`  
		Last Modified: Thu, 28 Oct 2021 01:57:59 GMT  
		Size: 9.7 KB (9668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633cdc0ee2e63d0df1b1e693ecf3947ca01f9c1843cd1e1f21d9b16958effdf5`  
		Last Modified: Thu, 28 Oct 2021 01:58:00 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57ec9e4f1b5721677f0cd7e5bd77c8d364c04bd78e96a528830486ebe9a74cf`  
		Last Modified: Thu, 28 Oct 2021 01:57:59 GMT  
		Size: 10.7 KB (10652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644a5090ddfa1106a57b25fe1251aa3af652c6bc002ed938c69efa8d13ceec86`  
		Last Modified: Thu, 28 Oct 2021 01:58:00 GMT  
		Size: 2.5 MB (2493018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ddccd96b1bcd0ef89a1fcfc003f8071e42ef47778717762b45abab0f749e6e`  
		Last Modified: Thu, 28 Oct 2021 01:58:23 GMT  
		Size: 209.3 MB (209276393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceff33fdbbf860efdae045e2fa402c1986f8eed375ec80cee3dd05c01974c68a`  
		Last Modified: Thu, 28 Oct 2021 01:58:09 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d506cfc35b6b1b727c4047c84da9292845ed6159ba6c2bcc939e06c10ea8a77`  
		Last Modified: Thu, 28 Oct 2021 01:58:11 GMT  
		Size: 14.3 MB (14250125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:kernel`

```console
$ docker pull websphere-liberty@sha256:5097107e544b395a1a6592993ddd6711d4db9aaf9a47bd30d23ecbcbbe717de2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:kernel` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:ee464c34f97bb768b4104598f3c1e0346bbce1d73048030b0ac77812c9489df9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.0 MB (178024060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:333e4a5e92a1e3e0601cebe2cb6d40eab384517ca9f3a497db31afde565b25d9`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:55:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 02:55:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:55:32 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 02:56:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:56:08 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 01 Oct 2021 07:13:40 GMT
ARG VERBOSE=false
# Fri, 01 Oct 2021 07:13:40 GMT
ARG OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:39:24 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Mon, 25 Oct 2021 22:39:24 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Mon, 25 Oct 2021 22:39:24 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Mon, 25 Oct 2021 22:39:24 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 22:39:24 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Mon, 25 Oct 2021 22:39:25 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 22:39:25 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 25 Oct 2021 22:39:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 25 Oct 2021 22:39:42 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Oct 2021 22:39:42 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Mon, 25 Oct 2021 22:39:42 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:39:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 25 Oct 2021 22:39:44 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Mon, 25 Oct 2021 22:39:44 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 25 Oct 2021 22:39:45 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 25 Oct 2021 22:39:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 25 Oct 2021 22:39:58 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Mon, 25 Oct 2021 22:39:58 GMT
USER 1001
# Mon, 25 Oct 2021 22:39:59 GMT
EXPOSE 9080 9443
# Mon, 25 Oct 2021 22:39:59 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 25 Oct 2021 22:39:59 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf7ef5b4a4700901695d7489ffa25c9a36a0c54f7003664412a2a582dd362fa`  
		Last Modified: Fri, 01 Oct 2021 02:59:16 GMT  
		Size: 3.0 MB (2959872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58286f2e604db89582fc1898b2d2a229d5920927e7705c94e32f38a70e29902e`  
		Last Modified: Fri, 01 Oct 2021 02:59:26 GMT  
		Size: 128.4 MB (128395032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb130bd160d991d174701aa1d12d4c1f75c81705bd6ae5b036ae6e50a248d88e`  
		Last Modified: Mon, 25 Oct 2021 23:05:29 GMT  
		Size: 14.1 MB (14072794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7beabf2dd59365e93d8abbb027ae0f1b98d39e3ea91de31bded58a8c1f92448`  
		Last Modified: Mon, 25 Oct 2021 23:05:25 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f040313f6379bc9c04a2b94631e0bf2906ed5a99289186e898117021c507384`  
		Last Modified: Mon, 25 Oct 2021 23:05:26 GMT  
		Size: 9.7 KB (9677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fe7348629a8b7a683f0e06d11fd83be6b5349bfcecda69c0e3aac2d45ec8ae`  
		Last Modified: Mon, 25 Oct 2021 23:05:25 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054c2e49311baee037b9f9b7a4c1860cc61c840b03b81c38b83a63dac906a86d`  
		Last Modified: Mon, 25 Oct 2021 23:05:25 GMT  
		Size: 10.7 KB (10667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e464e836a01729d2494c3dc860e6e078d5d69fe1819cc5a4b8c9042c73d6a4`  
		Last Modified: Mon, 25 Oct 2021 23:05:26 GMT  
		Size: 5.9 MB (5869965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel` - linux; 386

```console
$ docker pull websphere-liberty@sha256:21c2835a021b91c09268f12dc8f3c61f590c1b34d7669aeacf3792d83a7ef016
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162573580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e89243446a76e85ea4bf274dd0ad9e6fd0e763e50ced541577b62bee7dfcb74`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 18:38:55 GMT
ADD file:d859d389e38b7ac70fd56f97e38d52a77b58e72b96237a4302d1984cdd912a55 in / 
# Fri, 20 Mar 2020 18:38:56 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:38:57 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:38:58 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:38:58 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:06:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 20 Mar 2020 19:06:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:06:42 GMT
ENV JAVA_VERSION=1.8.0_sr6fp6
# Fri, 20 Mar 2020 19:07:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='87f9d45b7e1fa65ec018479f3ca7da69a03b52b0da10b8d1555142eec8ab0093';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='b5f825047c9bb5d360fb83694f12e17b1a5a15abf94ac82cd0a3aea32c9a361c';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='f3c04cd07ef269c24373840eae6f59c7db7a16d2e206d393ba93efa6dbb8d74f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2bbefda96f7d1a5f1694893961e92ccc59dfa50375ae5450675d7a4213d5812e';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='d5b0508d53d1c7382c06f5bc1daf3d57c19c70d851e86e6b1162bcd93f616f7e';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 20 Mar 2020 19:07:26 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 20 Mar 2020 19:31:53 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.3 org.opencontainers.image.revision=cl200320200305-1433
# Fri, 20 Mar 2020 19:31:53 GMT
ENV LIBERTY_VERSION=20.0.0_03
# Fri, 20 Mar 2020 19:31:53 GMT
ARG LIBERTY_URL
# Fri, 20 Mar 2020 19:31:53 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 20 Mar 2020 19:32:02 GMT
# ARGS: DOWNLOAD_OPTIONS=
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:32:03 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:32:03 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.3 BuildLabel=cl200320200305-1433
# Fri, 20 Mar 2020 19:32:03 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output
# Fri, 20 Mar 2020 19:32:04 GMT
# ARGS: DOWNLOAD_OPTIONS=
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 20 Mar 2020 19:32:04 GMT
COPY dir:0d0cedab2fbb7208b9d81afa78e9f15b12b71232224a2fe9753c00b7b72bd72e in /opt/ibm/helpers/ 
# Fri, 20 Mar 2020 19:32:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 20 Mar 2020 19:32:05 GMT
COPY dir:9277507d983008afcf8df6e0bfe2735bd4e92717515dbb3a7e268c830f213489 in /licenses/ 
# Fri, 20 Mar 2020 19:32:06 GMT
# ARGS: DOWNLOAD_OPTIONS=
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 20 Mar 2020 19:32:06 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 20 Mar 2020 19:32:06 GMT
USER 1001
# Fri, 20 Mar 2020 19:32:06 GMT
EXPOSE 9080 9443
# Fri, 20 Mar 2020 19:32:07 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 20 Mar 2020 19:32:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:765ce743592771b94ad8ff27e281e66c13f6039962c7dde4dbe47123081e015b`  
		Last Modified: Mon, 16 Mar 2020 15:38:41 GMT  
		Size: 27.1 MB (27122453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dc9c4739090a3d2f7265f1f8184b1cbd8ae133b863f8aa93ec5cf1761ee7a5`  
		Last Modified: Fri, 20 Mar 2020 18:39:35 GMT  
		Size: 34.6 KB (34625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a5b698281c077f48fc598e698f0619e4d00a2fedc1832fc95e9cf281408f63`  
		Last Modified: Fri, 20 Mar 2020 18:39:34 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaebe599891b1e1befc10d752a117cc5615ec2dd3913d399fd66e26e0cace3e5`  
		Last Modified: Fri, 20 Mar 2020 18:39:34 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f829150bc8a53a37ac17eb34838fa33c990881a4031bc650a9dae26b3f7880e`  
		Last Modified: Fri, 20 Mar 2020 19:09:23 GMT  
		Size: 3.0 MB (2992132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17b9ccc4baf3a1ffa517a03c7c3d01900136b128b36a83558c67c42e6c1cbaa`  
		Last Modified: Fri, 20 Mar 2020 19:09:35 GMT  
		Size: 118.8 MB (118756706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5011972f1876d464fb62206211a5b5e162ba2603bf20fc4cd0f2b4ffd311cd9`  
		Last Modified: Fri, 20 Mar 2020 19:39:16 GMT  
		Size: 13.6 MB (13600436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5395b713d5baa0917182ca82077b6fa2a0c51789907f96cbb12455586d9fa9b`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389324a3d9489b2fbcd5946f9d24285c0171c3218470e4a5e2d45c731cefc522`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 3.5 KB (3515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38ea596499e1f23ce426826250984869e92da50aec5845a6233a76d7764bfd1`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea3197b55235384f836e31a605c460f6cb7196f68dc29c65640738d8aa50188`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 57.4 KB (57426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683f76bf565cdb9e59c325f24357eb6b164555ed8629a4b8383448239608966d`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 4.4 KB (4358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:25ca6bf0c3ee273a34363059fcd67f58b41431e117a6ca0534ddb60eec70b18a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.8 MB (180847570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fb086abfd307b5aa8180d3eeb31548f2b856d9885bfdceeabdce3e72e714f77`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 17:55:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Oct 2021 17:56:05 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 17:56:16 GMT
ENV JAVA_VERSION=8.0.6.36
# Wed, 06 Oct 2021 17:57:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Oct 2021 17:57:38 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 07 Oct 2021 10:35:31 GMT
ARG VERBOSE=false
# Thu, 07 Oct 2021 10:35:33 GMT
ARG OPENJ9_SCC=true
# Mon, 25 Oct 2021 23:59:34 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Mon, 25 Oct 2021 23:59:39 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Mon, 25 Oct 2021 23:59:43 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Mon, 25 Oct 2021 23:59:46 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 23:59:51 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Mon, 25 Oct 2021 23:59:54 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 23:59:57 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 26 Oct 2021 00:00:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 26 Oct 2021 00:00:59 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 26 Oct 2021 00:01:02 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Tue, 26 Oct 2021 00:01:07 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:01:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 26 Oct 2021 00:01:22 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 26 Oct 2021 00:01:23 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 26 Oct 2021 00:01:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 26 Oct 2021 00:01:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 26 Oct 2021 00:01:56 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 26 Oct 2021 00:01:59 GMT
USER 1001
# Tue, 26 Oct 2021 00:02:02 GMT
EXPOSE 9080 9443
# Tue, 26 Oct 2021 00:02:04 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 26 Oct 2021 00:02:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce6e130fd3d09fd3fe6d741e0fa3f77120aa82717cf6d0a1cb49439939243a6`  
		Last Modified: Wed, 06 Oct 2021 18:04:08 GMT  
		Size: 3.1 MB (3081580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8fc8962750bc0e8c7c6ca6d1498e303c66e1f0b3f9613d204da9abf0200933`  
		Last Modified: Wed, 06 Oct 2021 18:04:22 GMT  
		Size: 127.9 MB (127898987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd371e52f22155313b0f3ae5f5c13597ca17fa0417c214eaf1e16df95bb678a8`  
		Last Modified: Tue, 26 Oct 2021 00:44:12 GMT  
		Size: 14.1 MB (14073366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee227af6d9277d187f05bd7fe3a7148fc127fd5be9bc040db19738760f9c12f`  
		Last Modified: Tue, 26 Oct 2021 00:44:08 GMT  
		Size: 697.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984133fc0355d34799cda371d5d2a8153e614767af49aa3cb7f8c98414e18950`  
		Last Modified: Tue, 26 Oct 2021 00:44:08 GMT  
		Size: 9.7 KB (9677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f9cacb1facc8e3097f176849d860aef3b7ebd23f9c9114047be96ca087ba97`  
		Last Modified: Tue, 26 Oct 2021 00:44:08 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfced5f1e31cfb68f3450e4211967c2c966cecdef7ccb633cb8a52a2c0cc710`  
		Last Modified: Tue, 26 Oct 2021 00:44:08 GMT  
		Size: 10.7 KB (10670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281fb76285f797555b5334b1d7f5596ec01e7137a6d55e8f31365b9fe39c2352`  
		Last Modified: Tue, 26 Oct 2021 00:44:09 GMT  
		Size: 5.3 MB (5339397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:06e38d016a5cebe53ca6fcd2e1e2072b96beed8b72eea08d9f54241d4d0c9cd5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.4 MB (173397283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab4fe7318aca4b94aa29bbde69e8cb5286b94a4f7a8073256f30c13c1c0e570a`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:17 GMT
ADD file:d248d4b5739ee5d07e920ec481dc4af81b314aa52e64618322197a642394a41d in / 
# Fri, 01 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:23:32 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 02:23:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:23:37 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 02:24:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:24:19 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 01 Oct 2021 03:40:55 GMT
ARG VERBOSE=false
# Fri, 01 Oct 2021 03:40:55 GMT
ARG OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:12:45 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Mon, 25 Oct 2021 22:12:45 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Mon, 25 Oct 2021 22:12:45 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Mon, 25 Oct 2021 22:12:45 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 22:12:45 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Mon, 25 Oct 2021 22:12:45 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 22:12:45 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 25 Oct 2021 22:12:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 25 Oct 2021 22:12:57 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Oct 2021 22:12:57 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Mon, 25 Oct 2021 22:12:57 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:12:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 25 Oct 2021 22:12:58 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Mon, 25 Oct 2021 22:12:58 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 25 Oct 2021 22:12:59 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 25 Oct 2021 22:13:06 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 25 Oct 2021 22:13:07 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Mon, 25 Oct 2021 22:13:07 GMT
USER 1001
# Mon, 25 Oct 2021 22:13:07 GMT
EXPOSE 9080 9443
# Mon, 25 Oct 2021 22:13:07 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 25 Oct 2021 22:13:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:97372e5b313b6b8bab9913de546bc50f73818d8275c94fc6491993c97b9d8bad`  
		Last Modified: Fri, 01 Oct 2021 01:43:49 GMT  
		Size: 25.4 MB (25362918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf425722012c2264c66ba97a53ff25a2f196330fbcc0872474e5e4562fa95f0`  
		Last Modified: Fri, 01 Oct 2021 02:27:43 GMT  
		Size: 2.7 MB (2676365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d432d8be662b9a55c0dfed6d79d328a62b58be822a9888d1b7d0d16dc6c248`  
		Last Modified: Fri, 01 Oct 2021 02:27:51 GMT  
		Size: 125.4 MB (125395531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969119abed0aabe761027277ec6fb7718eba553a1b072f7b1c13fbc7ad2643ce`  
		Last Modified: Mon, 25 Oct 2021 22:40:41 GMT  
		Size: 14.1 MB (14072637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6345425373ca667c20a30007a8292172e2b4eab13044ca41d184e4af52ff61e6`  
		Last Modified: Mon, 25 Oct 2021 22:40:39 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371f939cc39d32f824f40420cc6c72cee355cfa91155275e712b4632b2f7bc05`  
		Last Modified: Mon, 25 Oct 2021 22:40:39 GMT  
		Size: 9.7 KB (9674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f290e6c52139c0593dbbcd890fbc67f5b59bb711b97ea14886a2833a5a49ff93`  
		Last Modified: Mon, 25 Oct 2021 22:40:39 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4389715a5776e4d60e9b0bd807528101d253d83f6a4f2e5f9da17258ad41422c`  
		Last Modified: Mon, 25 Oct 2021 22:40:39 GMT  
		Size: 10.7 KB (10660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d732cb763586ba0cd58e22ae8ca4d3c4051b7370e0a5b974869d092a0d3a6b`  
		Last Modified: Mon, 25 Oct 2021 22:40:40 GMT  
		Size: 5.9 MB (5868523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:68eca94c7794582aec5f5211dc28e7e494bbb30fb8aa4057655ba4d5af5ef770
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:kernel-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:f86373f06ed1a16f3e8881886fc5de954a53559713dc66340b1c3cc708963246
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110227106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf72306691ccc6f1e2cd442b72f3cd1d0e61d077bcec92a645cc9a3d2981ee9b`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:44:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 02:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 00:31:11 GMT
ENV JAVA_VERSION=jdk-11.0.13+8_openj9-0.29.0
# Thu, 28 Oct 2021 00:33:11 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='3615940d4b26e8d11ff927dbf620a5247caecd84ba24c9d67f0e8b30ff463998';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_ppc64le_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        s390x)          ESUM='e942c0806163bbabe0b7ec8e630319489da400d58cd390011fc28428f468558e';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_s390x_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        amd64|x86_64)          ESUM='78eb54af15fac39eb2d254f51f0302aa213d3ad838f17766a9d081ca783edff4';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_x64_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 28 Oct 2021 00:33:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 00:33:11 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 28 Oct 2021 00:33:47 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 28 Oct 2021 01:07:18 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:07:18 GMT
ARG OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:07:18 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Thu, 28 Oct 2021 01:07:19 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Thu, 28 Oct 2021 01:07:19 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Thu, 28 Oct 2021 01:07:19 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 28 Oct 2021 01:07:19 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Thu, 28 Oct 2021 01:07:19 GMT
ARG LIBERTY_URL
# Thu, 28 Oct 2021 01:07:19 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 28 Oct 2021 01:07:28 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 01:07:29 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 01:07:29 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Thu, 28 Oct 2021 01:07:29 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:07:30 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 28 Oct 2021 01:07:30 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Thu, 28 Oct 2021 01:07:30 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 28 Oct 2021 01:07:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 28 Oct 2021 01:07:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 28 Oct 2021 01:07:39 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 28 Oct 2021 01:07:39 GMT
USER 1001
# Thu, 28 Oct 2021 01:07:40 GMT
EXPOSE 9080 9443
# Thu, 28 Oct 2021 01:07:40 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 28 Oct 2021 01:07:40 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237daeb1ae282fe20092079ef6d5de7924746d0f2e9ad88797d08524a4d842fd`  
		Last Modified: Sat, 16 Oct 2021 02:47:20 GMT  
		Size: 16.0 MB (16036029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82607fdca83d197b118a35c377753995ef0400ef8de999ed3b8675d5fa58ce2f`  
		Last Modified: Thu, 28 Oct 2021 00:37:33 GMT  
		Size: 44.7 MB (44737093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7e4f4f21da9c3eec66f54b7ec452e3ccf00f68d74a7287bb1cbfbd68d2b041`  
		Last Modified: Thu, 28 Oct 2021 00:37:28 GMT  
		Size: 4.2 MB (4202694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f320c18438947d83dc1f15e75d6225b16e4030be2f3f60b723231f7d507fea`  
		Last Modified: Thu, 28 Oct 2021 01:20:39 GMT  
		Size: 14.2 MB (14171331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74f02207975af9dde28884f091d0c74f1c9360ecd847c1c009a8b0ed2033da3`  
		Last Modified: Thu, 28 Oct 2021 01:20:36 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478f97fe27905bdbf70a5179455b31a085d4398c4679c15e2f6c0e8fecbb9a58`  
		Last Modified: Thu, 28 Oct 2021 01:20:35 GMT  
		Size: 9.7 KB (9666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948ab830722710af86fa613d3fa37a082644901281103a071d74cebb6bd7a9ea`  
		Last Modified: Thu, 28 Oct 2021 01:20:35 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3379a5452b604a9a1debf912875f4ebd9f1e6e7cf9af825c2c4decde12d33d`  
		Last Modified: Thu, 28 Oct 2021 01:20:35 GMT  
		Size: 10.7 KB (10654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e1c3e8451879781f16eeb22bd489cb303f75fdd57586410b1682cd5680c4f4`  
		Last Modified: Thu, 28 Oct 2021 01:20:36 GMT  
		Size: 2.5 MB (2491575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:2501c8103e674cde4e96b7a89765c7eecae507e5a14c96e1a6e34f2e3d80fa55
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115560935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bb4841dc48174a8550e37905a79527f37536c9d4722e022a888004146d478c6`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:54:47 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 00:55:56 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Oct 2021 01:45:21 GMT
ENV JAVA_VERSION=jdk-11.0.12+7_openj9-0.27.0
# Thu, 21 Oct 2021 01:48:48 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='285bd388a497db61408d26a9f3328f62004714ede94456718cf6440a109e25d2';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_ppc64le_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        s390x)          ESUM='6e5829aeb37abfb122e0944e438ecb2043c56df14fcdcce39bd4e3c9a55571a8';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_s390x_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        amd64|x86_64)          ESUM='f352998f6fdf0b84f63c563608be57f30aa3f14c8117c1219422dbc712ad4f81';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.12%2B7_openj9-0.27.0/ibm-semeru-open-jre_x64_linux_11.0.12_7_openj9-0.27.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 21 Oct 2021 01:49:04 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 21 Oct 2021 01:49:23 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 21 Oct 2021 01:50:18 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 26 Oct 2021 00:02:27 GMT
ARG VERBOSE=false
# Tue, 26 Oct 2021 00:02:29 GMT
ARG OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:02:31 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Tue, 26 Oct 2021 00:02:33 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Tue, 26 Oct 2021 00:02:34 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Tue, 26 Oct 2021 00:02:35 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 26 Oct 2021 00:02:37 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Tue, 26 Oct 2021 00:02:40 GMT
ARG LIBERTY_URL
# Tue, 26 Oct 2021 00:02:42 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 26 Oct 2021 00:03:11 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 26 Oct 2021 00:03:14 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 26 Oct 2021 00:03:18 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Tue, 26 Oct 2021 00:03:23 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:03:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 26 Oct 2021 00:03:39 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 26 Oct 2021 00:03:40 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 26 Oct 2021 00:03:50 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 26 Oct 2021 00:04:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 26 Oct 2021 00:04:11 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 26 Oct 2021 00:04:14 GMT
USER 1001
# Tue, 26 Oct 2021 00:04:16 GMT
EXPOSE 9080 9443
# Tue, 26 Oct 2021 00:04:17 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 26 Oct 2021 00:04:19 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c930749dacf55e37561edab7967f5a2f51660034fee0da501c2d71cb783301`  
		Last Modified: Sat, 16 Oct 2021 01:03:26 GMT  
		Size: 17.2 MB (17210510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d519f9110a27224937cddf5826128ca092be8957e9a8c13546df0dc596ba42`  
		Last Modified: Thu, 21 Oct 2021 02:03:00 GMT  
		Size: 45.1 MB (45107808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afebfecbc9bc8dad01d6486a0e236777ff1b2a82229ff13363f70a0827f07160`  
		Last Modified: Thu, 21 Oct 2021 02:02:53 GMT  
		Size: 3.3 MB (3286490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c959c7913b358daa8d638d574cfed5c19cc6fb4779f71b43debea7cb425f78`  
		Last Modified: Tue, 26 Oct 2021 00:44:25 GMT  
		Size: 14.2 MB (14171675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29638a4016c15c1f7a42994d97fb39804a5d41ae894b550b1353eb6ac21f45fb`  
		Last Modified: Tue, 26 Oct 2021 00:44:20 GMT  
		Size: 690.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91b025d347f73e0851038db7723a694dc2c472341019140169aa25a378a59a2`  
		Last Modified: Tue, 26 Oct 2021 00:44:20 GMT  
		Size: 9.7 KB (9670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56be72fe50f64e22ae2d25ba9f167dc85452ab42662d744b9124903f45eaa5bf`  
		Last Modified: Tue, 26 Oct 2021 00:44:20 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7340186166530eddc6450a7abcdeb1b9eab34407a9beb4a6ed3c513a95ba810f`  
		Last Modified: Tue, 26 Oct 2021 00:44:20 GMT  
		Size: 10.7 KB (10658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28516018017a50371e38a72026e7e2899fe67161aedd2bc9d3368ed652d4ccec`  
		Last Modified: Tue, 26 Oct 2021 00:44:21 GMT  
		Size: 2.5 MB (2475923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:da38ea19011c301b6927a7df2bd51ea85dcb3dc5e28278c4d314df21af5067ba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107632940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:030b09faee4fa1f3f5100082bbf2a954cf3e17b508408d1b1f6d36b813c26ca8`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:58:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 00:58:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 00:58:27 GMT
ENV JAVA_VERSION=jdk-11.0.13+8_openj9-0.29.0
# Thu, 28 Oct 2021 00:59:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='3615940d4b26e8d11ff927dbf620a5247caecd84ba24c9d67f0e8b30ff463998';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_ppc64le_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        s390x)          ESUM='e942c0806163bbabe0b7ec8e630319489da400d58cd390011fc28428f468558e';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_s390x_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        amd64|x86_64)          ESUM='78eb54af15fac39eb2d254f51f0302aa213d3ad838f17766a9d081ca783edff4';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.13%2B8_openj9-0.29.0/ibm-semeru-open-jre_x64_linux_11.0.13_8_openj9-0.29.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 28 Oct 2021 00:59:28 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 00:59:28 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 28 Oct 2021 01:00:01 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 28 Oct 2021 01:43:09 GMT
ARG VERBOSE=false
# Thu, 28 Oct 2021 01:43:09 GMT
ARG OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:43:09 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Thu, 28 Oct 2021 01:43:09 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Thu, 28 Oct 2021 01:43:09 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Thu, 28 Oct 2021 01:43:09 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 28 Oct 2021 01:43:10 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Thu, 28 Oct 2021 01:43:10 GMT
ARG LIBERTY_URL
# Thu, 28 Oct 2021 01:43:10 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 28 Oct 2021 01:43:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Oct 2021 01:43:20 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 01:43:20 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Thu, 28 Oct 2021 01:43:20 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 28 Oct 2021 01:43:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 28 Oct 2021 01:43:21 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Thu, 28 Oct 2021 01:43:21 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 28 Oct 2021 01:43:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 28 Oct 2021 01:43:26 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 28 Oct 2021 01:43:27 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 28 Oct 2021 01:43:27 GMT
USER 1001
# Thu, 28 Oct 2021 01:43:27 GMT
EXPOSE 9080 9443
# Thu, 28 Oct 2021 01:43:27 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 28 Oct 2021 01:43:27 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276dbe4459a060d2c186c43e5e92d98fa6f181617c55cce69da393b9d5dd6200`  
		Last Modified: Sat, 16 Oct 2021 01:01:03 GMT  
		Size: 15.7 MB (15742080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bef20936d077045a96f4b0694d1470b79e8825348eb06b3a0ef4207079d17d`  
		Last Modified: Thu, 28 Oct 2021 01:02:07 GMT  
		Size: 43.8 MB (43800069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8547dc44147bfe37bde98eef473a2916985469204db561ebefa3e3d92fee029a`  
		Last Modified: Thu, 28 Oct 2021 01:02:01 GMT  
		Size: 4.3 MB (4284720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8fe7f49f8a6320a829b59b87b8e6d2f5c623b8926fa5cbbd62cb3e14326e58`  
		Last Modified: Thu, 28 Oct 2021 01:58:02 GMT  
		Size: 14.2 MB (14170913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ea4b6d21bf75f5dc6643a5940ef5db23c15356b23f70a0adfcd0e80230ac8a`  
		Last Modified: Thu, 28 Oct 2021 01:57:59 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4198f3548e614a889bcf03b30adebe8652f6a27b339dde077ee4ebb8babfd2e`  
		Last Modified: Thu, 28 Oct 2021 01:57:59 GMT  
		Size: 9.7 KB (9668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633cdc0ee2e63d0df1b1e693ecf3947ca01f9c1843cd1e1f21d9b16958effdf5`  
		Last Modified: Thu, 28 Oct 2021 01:58:00 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57ec9e4f1b5721677f0cd7e5bd77c8d364c04bd78e96a528830486ebe9a74cf`  
		Last Modified: Thu, 28 Oct 2021 01:57:59 GMT  
		Size: 10.7 KB (10652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644a5090ddfa1106a57b25fe1251aa3af652c6bc002ed938c69efa8d13ceec86`  
		Last Modified: Thu, 28 Oct 2021 01:58:00 GMT  
		Size: 2.5 MB (2493018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:latest`

```console
$ docker pull websphere-liberty@sha256:942c68a160909bd10112af6af1a2ee0e17566295dc3030e8ecace60c75f14397
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:latest` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:b1115005499014bf1a10d5355e4d098ba6f4226783f08ea11272c326186fdd7f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.3 MB (403315070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf37216acf115eb9b9aff1a9f65dffc623e75c16a56cb1584bfd62ccf90a8094`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:55:25 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 02:55:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:55:32 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 02:56:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:56:08 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 01 Oct 2021 07:13:40 GMT
ARG VERBOSE=false
# Fri, 01 Oct 2021 07:13:40 GMT
ARG OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:39:24 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Mon, 25 Oct 2021 22:39:24 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Mon, 25 Oct 2021 22:39:24 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Mon, 25 Oct 2021 22:39:24 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 22:39:24 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Mon, 25 Oct 2021 22:39:25 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 22:39:25 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 25 Oct 2021 22:39:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 25 Oct 2021 22:39:42 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Oct 2021 22:39:42 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Mon, 25 Oct 2021 22:39:42 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:39:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 25 Oct 2021 22:39:44 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Mon, 25 Oct 2021 22:39:44 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 25 Oct 2021 22:39:45 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 25 Oct 2021 22:39:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 25 Oct 2021 22:39:58 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Mon, 25 Oct 2021 22:39:58 GMT
USER 1001
# Mon, 25 Oct 2021 22:39:59 GMT
EXPOSE 9080 9443
# Mon, 25 Oct 2021 22:39:59 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 25 Oct 2021 22:39:59 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Mon, 25 Oct 2021 22:40:32 GMT
ARG VERBOSE=false
# Mon, 25 Oct 2021 22:40:32 GMT
ARG REPOSITORIES_PROPERTIES=
# Mon, 25 Oct 2021 22:43:34 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Mon, 25 Oct 2021 22:43:35 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Mon, 25 Oct 2021 22:44:22 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf7ef5b4a4700901695d7489ffa25c9a36a0c54f7003664412a2a582dd362fa`  
		Last Modified: Fri, 01 Oct 2021 02:59:16 GMT  
		Size: 3.0 MB (2959872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58286f2e604db89582fc1898b2d2a229d5920927e7705c94e32f38a70e29902e`  
		Last Modified: Fri, 01 Oct 2021 02:59:26 GMT  
		Size: 128.4 MB (128395032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb130bd160d991d174701aa1d12d4c1f75c81705bd6ae5b036ae6e50a248d88e`  
		Last Modified: Mon, 25 Oct 2021 23:05:29 GMT  
		Size: 14.1 MB (14072794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7beabf2dd59365e93d8abbb027ae0f1b98d39e3ea91de31bded58a8c1f92448`  
		Last Modified: Mon, 25 Oct 2021 23:05:25 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f040313f6379bc9c04a2b94631e0bf2906ed5a99289186e898117021c507384`  
		Last Modified: Mon, 25 Oct 2021 23:05:26 GMT  
		Size: 9.7 KB (9677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fe7348629a8b7a683f0e06d11fd83be6b5349bfcecda69c0e3aac2d45ec8ae`  
		Last Modified: Mon, 25 Oct 2021 23:05:25 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054c2e49311baee037b9f9b7a4c1860cc61c840b03b81c38b83a63dac906a86d`  
		Last Modified: Mon, 25 Oct 2021 23:05:25 GMT  
		Size: 10.7 KB (10667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e464e836a01729d2494c3dc860e6e078d5d69fe1819cc5a4b8c9042c73d6a4`  
		Last Modified: Mon, 25 Oct 2021 23:05:26 GMT  
		Size: 5.9 MB (5869965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c845db47bbb20043cf2fd0baed54e15d4fdcc9659d3028b0d1ac7de9f87084f`  
		Last Modified: Mon, 25 Oct 2021 23:05:58 GMT  
		Size: 209.3 MB (209275727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c30de2c69d7ebc9cdb54e55b3d6a59437590a6fe6567f3bdf252ad06f6cd7d`  
		Last Modified: Mon, 25 Oct 2021 23:05:47 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b9160a1a04cb7a1afff92f9ceee48a39b1138f6751e1b860b52fe4e1c2236b`  
		Last Modified: Mon, 25 Oct 2021 23:05:49 GMT  
		Size: 16.0 MB (16014336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; 386

```console
$ docker pull websphere-liberty@sha256:c847143995aec30ca5d4526544d7c41ca7a42a8baf8195848864d0128e96ecf3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.2 MB (349209019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6d2c9374be56a63d6e35820fec8676f2d4ed2b9bdaf09a49c8545b039479bb7`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 18:38:55 GMT
ADD file:d859d389e38b7ac70fd56f97e38d52a77b58e72b96237a4302d1984cdd912a55 in / 
# Fri, 20 Mar 2020 18:38:56 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:38:57 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:38:58 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:38:58 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:06:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 20 Mar 2020 19:06:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:06:42 GMT
ENV JAVA_VERSION=1.8.0_sr6fp6
# Fri, 20 Mar 2020 19:07:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='87f9d45b7e1fa65ec018479f3ca7da69a03b52b0da10b8d1555142eec8ab0093';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='b5f825047c9bb5d360fb83694f12e17b1a5a15abf94ac82cd0a3aea32c9a361c';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='f3c04cd07ef269c24373840eae6f59c7db7a16d2e206d393ba93efa6dbb8d74f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2bbefda96f7d1a5f1694893961e92ccc59dfa50375ae5450675d7a4213d5812e';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='d5b0508d53d1c7382c06f5bc1daf3d57c19c70d851e86e6b1162bcd93f616f7e';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 20 Mar 2020 19:07:26 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 20 Mar 2020 19:31:53 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.3 org.opencontainers.image.revision=cl200320200305-1433
# Fri, 20 Mar 2020 19:31:53 GMT
ENV LIBERTY_VERSION=20.0.0_03
# Fri, 20 Mar 2020 19:31:53 GMT
ARG LIBERTY_URL
# Fri, 20 Mar 2020 19:31:53 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 20 Mar 2020 19:32:02 GMT
# ARGS: DOWNLOAD_OPTIONS=
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:32:03 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:32:03 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.3 BuildLabel=cl200320200305-1433
# Fri, 20 Mar 2020 19:32:03 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output
# Fri, 20 Mar 2020 19:32:04 GMT
# ARGS: DOWNLOAD_OPTIONS=
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 20 Mar 2020 19:32:04 GMT
COPY dir:0d0cedab2fbb7208b9d81afa78e9f15b12b71232224a2fe9753c00b7b72bd72e in /opt/ibm/helpers/ 
# Fri, 20 Mar 2020 19:32:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 20 Mar 2020 19:32:05 GMT
COPY dir:9277507d983008afcf8df6e0bfe2735bd4e92717515dbb3a7e268c830f213489 in /licenses/ 
# Fri, 20 Mar 2020 19:32:06 GMT
# ARGS: DOWNLOAD_OPTIONS=
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 20 Mar 2020 19:32:06 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 20 Mar 2020 19:32:06 GMT
USER 1001
# Fri, 20 Mar 2020 19:32:06 GMT
EXPOSE 9080 9443
# Fri, 20 Mar 2020 19:32:07 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 20 Mar 2020 19:32:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 20 Mar 2020 19:32:10 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 20 Mar 2020 19:35:01 GMT
# ARGS: REPOSITORIES_PROPERTIES=
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Fri, 20 Mar 2020 19:35:01 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
```

-	Layers:
	-	`sha256:765ce743592771b94ad8ff27e281e66c13f6039962c7dde4dbe47123081e015b`  
		Last Modified: Mon, 16 Mar 2020 15:38:41 GMT  
		Size: 27.1 MB (27122453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dc9c4739090a3d2f7265f1f8184b1cbd8ae133b863f8aa93ec5cf1761ee7a5`  
		Last Modified: Fri, 20 Mar 2020 18:39:35 GMT  
		Size: 34.6 KB (34625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a5b698281c077f48fc598e698f0619e4d00a2fedc1832fc95e9cf281408f63`  
		Last Modified: Fri, 20 Mar 2020 18:39:34 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaebe599891b1e1befc10d752a117cc5615ec2dd3913d399fd66e26e0cace3e5`  
		Last Modified: Fri, 20 Mar 2020 18:39:34 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f829150bc8a53a37ac17eb34838fa33c990881a4031bc650a9dae26b3f7880e`  
		Last Modified: Fri, 20 Mar 2020 19:09:23 GMT  
		Size: 3.0 MB (2992132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17b9ccc4baf3a1ffa517a03c7c3d01900136b128b36a83558c67c42e6c1cbaa`  
		Last Modified: Fri, 20 Mar 2020 19:09:35 GMT  
		Size: 118.8 MB (118756706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5011972f1876d464fb62206211a5b5e162ba2603bf20fc4cd0f2b4ffd311cd9`  
		Last Modified: Fri, 20 Mar 2020 19:39:16 GMT  
		Size: 13.6 MB (13600436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5395b713d5baa0917182ca82077b6fa2a0c51789907f96cbb12455586d9fa9b`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389324a3d9489b2fbcd5946f9d24285c0171c3218470e4a5e2d45c731cefc522`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 3.5 KB (3515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38ea596499e1f23ce426826250984869e92da50aec5845a6233a76d7764bfd1`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea3197b55235384f836e31a605c460f6cb7196f68dc29c65640738d8aa50188`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 57.4 KB (57426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683f76bf565cdb9e59c325f24357eb6b164555ed8629a4b8383448239608966d`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 4.4 KB (4358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cd2560c76831311d13d197b4784e0826f6ffae62e3b9a22d2fa5675b9b71a2`  
		Last Modified: Fri, 20 Mar 2020 19:39:42 GMT  
		Size: 186.6 MB (186634496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9891aa2b3e904f8f514677372187983ac12c98c209c433ab5bf0862e09d6f4ef`  
		Last Modified: Fri, 20 Mar 2020 19:39:20 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:3ebbd27afd1c227833f438d21f9636d883949eb2b952f08fdd6e0ba66b7dd4ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.0 MB (403966097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c78740a0ed156d7ac4d80645081da020f7c953c822c860f315773a5411af4e92`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 17:55:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Oct 2021 17:56:05 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 17:56:16 GMT
ENV JAVA_VERSION=8.0.6.36
# Wed, 06 Oct 2021 17:57:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Oct 2021 17:57:38 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 07 Oct 2021 10:35:31 GMT
ARG VERBOSE=false
# Thu, 07 Oct 2021 10:35:33 GMT
ARG OPENJ9_SCC=true
# Mon, 25 Oct 2021 23:59:34 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Mon, 25 Oct 2021 23:59:39 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Mon, 25 Oct 2021 23:59:43 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Mon, 25 Oct 2021 23:59:46 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 23:59:51 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Mon, 25 Oct 2021 23:59:54 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 23:59:57 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 26 Oct 2021 00:00:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 26 Oct 2021 00:00:59 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 26 Oct 2021 00:01:02 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Tue, 26 Oct 2021 00:01:07 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 26 Oct 2021 00:01:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 26 Oct 2021 00:01:22 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 26 Oct 2021 00:01:23 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 26 Oct 2021 00:01:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 26 Oct 2021 00:01:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 26 Oct 2021 00:01:56 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Tue, 26 Oct 2021 00:01:59 GMT
USER 1001
# Tue, 26 Oct 2021 00:02:02 GMT
EXPOSE 9080 9443
# Tue, 26 Oct 2021 00:02:04 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 26 Oct 2021 00:02:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 26 Oct 2021 00:04:38 GMT
ARG VERBOSE=false
# Tue, 26 Oct 2021 00:04:41 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 26 Oct 2021 00:08:18 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 26 Oct 2021 00:08:26 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 26 Oct 2021 00:09:32 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce6e130fd3d09fd3fe6d741e0fa3f77120aa82717cf6d0a1cb49439939243a6`  
		Last Modified: Wed, 06 Oct 2021 18:04:08 GMT  
		Size: 3.1 MB (3081580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8fc8962750bc0e8c7c6ca6d1498e303c66e1f0b3f9613d204da9abf0200933`  
		Last Modified: Wed, 06 Oct 2021 18:04:22 GMT  
		Size: 127.9 MB (127898987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd371e52f22155313b0f3ae5f5c13597ca17fa0417c214eaf1e16df95bb678a8`  
		Last Modified: Tue, 26 Oct 2021 00:44:12 GMT  
		Size: 14.1 MB (14073366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee227af6d9277d187f05bd7fe3a7148fc127fd5be9bc040db19738760f9c12f`  
		Last Modified: Tue, 26 Oct 2021 00:44:08 GMT  
		Size: 697.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984133fc0355d34799cda371d5d2a8153e614767af49aa3cb7f8c98414e18950`  
		Last Modified: Tue, 26 Oct 2021 00:44:08 GMT  
		Size: 9.7 KB (9677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f9cacb1facc8e3097f176849d860aef3b7ebd23f9c9114047be96ca087ba97`  
		Last Modified: Tue, 26 Oct 2021 00:44:08 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfced5f1e31cfb68f3450e4211967c2c966cecdef7ccb633cb8a52a2c0cc710`  
		Last Modified: Tue, 26 Oct 2021 00:44:08 GMT  
		Size: 10.7 KB (10670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281fb76285f797555b5334b1d7f5596ec01e7137a6d55e8f31365b9fe39c2352`  
		Last Modified: Tue, 26 Oct 2021 00:44:09 GMT  
		Size: 5.3 MB (5339397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4562f8c3c1dade81475edf6207aea4f9c941c6b7c037c67810ebd4ee1c8098a3`  
		Last Modified: Tue, 26 Oct 2021 00:44:52 GMT  
		Size: 209.3 MB (209276516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09802a7cb8ad05d0191cf0a29e24e2e79b4306e2654390c0460db8311b15baa4`  
		Last Modified: Tue, 26 Oct 2021 00:44:33 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfae2d34298fb1bd2f919e6859a8e487b8d641e70379ba24107b763ad45558fe`  
		Last Modified: Tue, 26 Oct 2021 00:44:35 GMT  
		Size: 13.8 MB (13841061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:2456846170fe619056099175052bbc1115ade0e8a159250e76a21941cae6068d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.3 MB (398292262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed3ce5d13fb58bdf360ce6367ee827a0b76c2b099e4a24a7d693097f201d5545`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:17 GMT
ADD file:d248d4b5739ee5d07e920ec481dc4af81b314aa52e64618322197a642394a41d in / 
# Fri, 01 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:23:32 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 01 Oct 2021 02:23:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:23:37 GMT
ENV JAVA_VERSION=8.0.6.36
# Fri, 01 Oct 2021 02:24:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d0198a37b63810174dc972eb06976e3e761efb21524c1fa3f9f1ed1246f3a9e3';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='05dddc6918557b3bf72ba48060e73804dcba692dfddeaaaee5551fcd3ac63915';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='48bbf5a656b06db138d79aeaecc4d63d86f133288d6c3e51084d1c2c5e9321b8';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='087140a55103a896ba134c82ef065fb9486b4de0a72a5f4f42f96f5728c68968';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='471b567c6f42291704020a77e0d1c219dcdefe0e0bfb85a9f0f3c8ecf66a1161';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 01 Oct 2021 02:24:19 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 01 Oct 2021 03:40:55 GMT
ARG VERBOSE=false
# Fri, 01 Oct 2021 03:40:55 GMT
ARG OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:12:45 GMT
ARG EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21
# Mon, 25 Oct 2021 22:12:45 GMT
ARG NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72
# Mon, 25 Oct 2021 22:12:45 GMT
ARG NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2
# Mon, 25 Oct 2021 22:12:45 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.10 org.opencontainers.image.revision=cl211020210920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 25 Oct 2021 22:12:45 GMT
ENV LIBERTY_VERSION=21.0.0_10
# Mon, 25 Oct 2021 22:12:45 GMT
ARG LIBERTY_URL
# Mon, 25 Oct 2021 22:12:45 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 25 Oct 2021 22:12:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 25 Oct 2021 22:12:57 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Oct 2021 22:12:57 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.10 BuildLabel=cl211020210920-1900
# Mon, 25 Oct 2021 22:12:57 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 25 Oct 2021 22:12:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 25 Oct 2021 22:12:58 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Mon, 25 Oct 2021 22:12:58 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 25 Oct 2021 22:12:59 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 25 Oct 2021 22:13:06 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=22d5722d306eaf9b5c658a81e7a9e301f1d956b820ea7497bb71cb61c5715d21 NON_IBM_SHA=163424d07846c44f428786fcaabeca1c9f24fde84e61e2a28f90858b968f3a72 NOTICES_SHA=da6cdfe101e6dd1d60c10df4fe74b85ac4e4c0a920cc5f12c27bba2be81912b2 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 25 Oct 2021 22:13:07 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Mon, 25 Oct 2021 22:13:07 GMT
USER 1001
# Mon, 25 Oct 2021 22:13:07 GMT
EXPOSE 9080 9443
# Mon, 25 Oct 2021 22:13:07 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 25 Oct 2021 22:13:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Mon, 25 Oct 2021 22:13:39 GMT
ARG VERBOSE=false
# Mon, 25 Oct 2021 22:13:40 GMT
ARG REPOSITORIES_PROPERTIES=
# Mon, 25 Oct 2021 22:17:03 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Mon, 25 Oct 2021 22:17:07 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Mon, 25 Oct 2021 22:17:31 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:97372e5b313b6b8bab9913de546bc50f73818d8275c94fc6491993c97b9d8bad`  
		Last Modified: Fri, 01 Oct 2021 01:43:49 GMT  
		Size: 25.4 MB (25362918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf425722012c2264c66ba97a53ff25a2f196330fbcc0872474e5e4562fa95f0`  
		Last Modified: Fri, 01 Oct 2021 02:27:43 GMT  
		Size: 2.7 MB (2676365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d432d8be662b9a55c0dfed6d79d328a62b58be822a9888d1b7d0d16dc6c248`  
		Last Modified: Fri, 01 Oct 2021 02:27:51 GMT  
		Size: 125.4 MB (125395531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969119abed0aabe761027277ec6fb7718eba553a1b072f7b1c13fbc7ad2643ce`  
		Last Modified: Mon, 25 Oct 2021 22:40:41 GMT  
		Size: 14.1 MB (14072637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6345425373ca667c20a30007a8292172e2b4eab13044ca41d184e4af52ff61e6`  
		Last Modified: Mon, 25 Oct 2021 22:40:39 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371f939cc39d32f824f40420cc6c72cee355cfa91155275e712b4632b2f7bc05`  
		Last Modified: Mon, 25 Oct 2021 22:40:39 GMT  
		Size: 9.7 KB (9674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f290e6c52139c0593dbbcd890fbc67f5b59bb711b97ea14886a2833a5a49ff93`  
		Last Modified: Mon, 25 Oct 2021 22:40:39 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4389715a5776e4d60e9b0bd807528101d253d83f6a4f2e5f9da17258ad41422c`  
		Last Modified: Mon, 25 Oct 2021 22:40:39 GMT  
		Size: 10.7 KB (10660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d732cb763586ba0cd58e22ae8ca4d3c4051b7370e0a5b974869d092a0d3a6b`  
		Last Modified: Mon, 25 Oct 2021 22:40:40 GMT  
		Size: 5.9 MB (5868523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3471c7e056a5f605febd60fea600313267b0f15c9c8449d042119817212638bb`  
		Last Modified: Mon, 25 Oct 2021 22:41:02 GMT  
		Size: 209.3 MB (209276442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb25227e9262c819dd066fb48ebfc7b4e86cfe76a0939caf9895ac2836c0531d`  
		Last Modified: Mon, 25 Oct 2021 22:40:53 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc404276fd2ceb3aac5a837f879edd92a65c6cdda45b95937e3ca3d7f1bd01c`  
		Last Modified: Mon, 25 Oct 2021 22:40:56 GMT  
		Size: 15.6 MB (15617590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
