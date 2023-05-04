## `websphere-liberty:full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:f23f3e8fdcdc5cde37568ee9ac6645c5c83513012ec694e7b92b171170a34711
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:e77e0c66a51ca1c08c3ba9caeb87c555bea369bcd2a5fcb3d7917d62b87d34e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.6 MB (487641262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71ea9b060938768a7cf591efa3135cc2e50f015fd42266cc17051627ad5f42f6`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Tue, 18 Apr 2023 01:48:06 GMT
ENV JAVA_VERSION=jdk-11.0.18+10_openj9-0.36.0
# Tue, 18 Apr 2023 01:49:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b7dae99808061eb1774e3af436453c48c30c01213a1613ca53df698276844f65';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.18%2B10_openj9-0.36.1/ibm-semeru-open-jre_aarch64_linux_11.0.18_10_openj9-0.36.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='f4eb9f501596a722a4be708361c1bfaa6b760cc7c885519d176cabba7a84d6e8';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.18%2B10_openj9-0.36.1/ibm-semeru-open-jre_ppc64le_linux_11.0.18_10_openj9-0.36.1.tar.gz';          ;;        amd64|x86_64)          ESUM='509a8c1e533c41896fddab187a8f6712ce1121d19eff71f4f023b58969147c9f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.18%2B10_openj9-0.36.1/ibm-semeru-open-jre_x64_linux_11.0.18_10_openj9-0.36.1.tar.gz';          ;;        s390x)          ESUM='ed6bbd482d9db361beb27510c5e88d882ba7232fc80409e35e33c08a5af7c7c0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.18%2B10_openj9-0.36.1/ibm-semeru-open-jre_s390x_linux_11.0.18_10_openj9-0.36.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 18 Apr 2023 01:49:02 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:49:02 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 18 Apr 2023 01:49:37 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 18 Apr 2023 06:55:52 GMT
ARG VERBOSE=false
# Tue, 18 Apr 2023 06:55:52 GMT
ARG OPENJ9_SCC=true
# Tue, 18 Apr 2023 06:55:52 GMT
ARG EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f
# Tue, 18 Apr 2023 06:55:52 GMT
ARG NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f
# Tue, 18 Apr 2023 06:55:52 GMT
ARG NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee
# Tue, 18 Apr 2023 06:55:52 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=23.0.0.3 org.opencontainers.image.revision=cl230320230319-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 18 Apr 2023 06:55:52 GMT
ENV LIBERTY_VERSION=23.0.0_03
# Tue, 18 Apr 2023 06:55:52 GMT
ARG LIBERTY_URL
# Tue, 18 Apr 2023 06:55:52 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 18 Apr 2023 06:56:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 06:56:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ibm/wlp/bin:/opt/ibm/helpers/build
# Tue, 18 Apr 2023 06:56:09 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=23.0.0.3 BuildLabel=cl230320230319-1900
# Tue, 18 Apr 2023 06:56:09 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 18 Apr 2023 06:56:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 18 Apr 2023 06:56:10 GMT
COPY dir:0f3e336b1e5adb84a625050153035561e1c9802a57b7b90b5a17ebb82adba489 in /opt/ibm/helpers/ 
# Tue, 18 Apr 2023 06:56:10 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 18 Apr 2023 06:56:11 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 18 Apr 2023 06:56:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 18 Apr 2023 06:56:16 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 18 Apr 2023 06:56:16 GMT
USER 1001
# Tue, 18 Apr 2023 06:56:17 GMT
EXPOSE 9080 9443
# Tue, 18 Apr 2023 06:56:17 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 18 Apr 2023 06:56:17 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 18 Apr 2023 06:56:50 GMT
ARG VERBOSE=false
# Tue, 18 Apr 2023 06:56:51 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 18 Apr 2023 07:06:43 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 18 Apr 2023 07:06:45 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 18 Apr 2023 07:07:13 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:30def0b8c478f7d3f489d3b3cdb9e9db73566671bc38544c711cdffd59440f71`  
		Last Modified: Tue, 18 Apr 2023 01:55:11 GMT  
		Size: 48.3 MB (48304695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048a8ba33e640597d4f1d4bd7cdd26ec92a5f86178cd1875c28ae8ebc411f0f4`  
		Last Modified: Tue, 18 Apr 2023 01:55:05 GMT  
		Size: 4.1 MB (4145788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621d231d670bcfc648bc6a5e825d44ab3183cab8f42f5a74f65cc54c5cbd2a49`  
		Last Modified: Tue, 18 Apr 2023 07:38:19 GMT  
		Size: 14.5 MB (14452468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a3220cd70e33c1e9e2817cee091e52a89d33fd5728255752ec20d4bdb6d3af`  
		Last Modified: Tue, 18 Apr 2023 07:38:16 GMT  
		Size: 674.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f001c06473f8a7d9d4c92a3a5e5ec464d11d75f87d6a1bb440adbf31573f43`  
		Last Modified: Tue, 18 Apr 2023 07:38:16 GMT  
		Size: 9.8 KB (9806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b349fe0fc0636da846344ee0a3af2b9e5705f951f0a54e921cb9db2c0bdeeec`  
		Last Modified: Tue, 18 Apr 2023 07:38:16 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77c30ae52945640a8d7ea5d82c3a7c62d80b7445d706195b35679673d029731`  
		Last Modified: Tue, 18 Apr 2023 07:38:16 GMT  
		Size: 10.8 KB (10781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6eedc3c367d1c791cf1aa6dd419b735c1fd923aae9911c311253fd4978c25cf`  
		Last Modified: Tue, 18 Apr 2023 07:38:16 GMT  
		Size: 2.6 MB (2642509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129614b321aaf17b2ba5b61043c90aba1a9bf11e1cbd6e970176f9386018b448`  
		Last Modified: Tue, 18 Apr 2023 07:38:51 GMT  
		Size: 359.0 MB (359033951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f218a505125a727137f8de9e42c845766f3ef03674e75f4b47a80b9cb7207f6f`  
		Last Modified: Tue, 18 Apr 2023 07:38:34 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec5272e9240ae7e1daea17bfc82360f4ab49134f0eebd6cecca5b6d4855ca7f`  
		Last Modified: Tue, 18 Apr 2023 07:38:36 GMT  
		Size: 14.5 MB (14458019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java11-openj9` - linux; arm64 variant v8

```console
$ docker pull websphere-liberty@sha256:7e3c8379ac6fddb72e387ded177dfcefcccd75142e89ecaf439826486d83e7ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **483.8 MB (483839629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5748b3396ee2b4b34ed93baf734c81a1200127e532547be22a3284e46c8ab474`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Tue, 18 Apr 2023 01:47:22 GMT
ENV JAVA_VERSION=jdk-11.0.18+10_openj9-0.36.0
# Tue, 18 Apr 2023 01:48:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b7dae99808061eb1774e3af436453c48c30c01213a1613ca53df698276844f65';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.18%2B10_openj9-0.36.1/ibm-semeru-open-jre_aarch64_linux_11.0.18_10_openj9-0.36.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='f4eb9f501596a722a4be708361c1bfaa6b760cc7c885519d176cabba7a84d6e8';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.18%2B10_openj9-0.36.1/ibm-semeru-open-jre_ppc64le_linux_11.0.18_10_openj9-0.36.1.tar.gz';          ;;        amd64|x86_64)          ESUM='509a8c1e533c41896fddab187a8f6712ce1121d19eff71f4f023b58969147c9f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.18%2B10_openj9-0.36.1/ibm-semeru-open-jre_x64_linux_11.0.18_10_openj9-0.36.1.tar.gz';          ;;        s390x)          ESUM='ed6bbd482d9db361beb27510c5e88d882ba7232fc80409e35e33c08a5af7c7c0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.18%2B10_openj9-0.36.1/ibm-semeru-open-jre_s390x_linux_11.0.18_10_openj9-0.36.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 18 Apr 2023 01:48:15 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:48:15 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 18 Apr 2023 01:48:50 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 04 May 2023 09:00:43 GMT
ARG VERBOSE=false
# Thu, 04 May 2023 09:00:43 GMT
ARG OPENJ9_SCC=true
# Thu, 04 May 2023 09:00:43 GMT
ARG EN_SHA=d7580938d35387110e39c3c8b3bb5c1f8dc9f0418a2f77799dbcf69a2ab63093
# Thu, 04 May 2023 09:00:43 GMT
ARG NON_IBM_SHA=0d97a3e5cf5403a9b3be514509977f4e9be4a2ac4258e692ef8e64761910f4c0
# Thu, 04 May 2023 09:00:43 GMT
ARG NOTICES_SHA=71f58dc38b4c9b60beaec4459b97b0d08228ad8e5fe5e3a0f4fd7e7c66285925
# Thu, 04 May 2023 09:00:44 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=23.0.0.4 org.opencontainers.image.revision=cl230420230418-0035 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 04 May 2023 09:00:44 GMT
ENV LIBERTY_VERSION=23.0.0_04
# Thu, 04 May 2023 09:00:44 GMT
ARG LIBERTY_URL
# Thu, 04 May 2023 09:00:44 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 04 May 2023 09:00:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=d7580938d35387110e39c3c8b3bb5c1f8dc9f0418a2f77799dbcf69a2ab63093 NON_IBM_SHA=0d97a3e5cf5403a9b3be514509977f4e9be4a2ac4258e692ef8e64761910f4c0 NOTICES_SHA=71f58dc38b4c9b60beaec4459b97b0d08228ad8e5fe5e3a0f4fd7e7c66285925 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 09:00:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ibm/wlp/bin:/opt/ibm/helpers/build
# Thu, 04 May 2023 09:00:59 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=23.0.0.4 BuildLabel=cl230420230418-0035
# Thu, 04 May 2023 09:00:59 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 04 May 2023 09:00:59 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=d7580938d35387110e39c3c8b3bb5c1f8dc9f0418a2f77799dbcf69a2ab63093 NON_IBM_SHA=0d97a3e5cf5403a9b3be514509977f4e9be4a2ac4258e692ef8e64761910f4c0 NOTICES_SHA=71f58dc38b4c9b60beaec4459b97b0d08228ad8e5fe5e3a0f4fd7e7c66285925 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 04 May 2023 09:00:59 GMT
COPY dir:0f3e336b1e5adb84a625050153035561e1c9802a57b7b90b5a17ebb82adba489 in /opt/ibm/helpers/ 
# Thu, 04 May 2023 09:00:59 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 04 May 2023 09:01:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=d7580938d35387110e39c3c8b3bb5c1f8dc9f0418a2f77799dbcf69a2ab63093 NON_IBM_SHA=0d97a3e5cf5403a9b3be514509977f4e9be4a2ac4258e692ef8e64761910f4c0 NOTICES_SHA=71f58dc38b4c9b60beaec4459b97b0d08228ad8e5fe5e3a0f4fd7e7c66285925 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 04 May 2023 09:01:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=d7580938d35387110e39c3c8b3bb5c1f8dc9f0418a2f77799dbcf69a2ab63093 NON_IBM_SHA=0d97a3e5cf5403a9b3be514509977f4e9be4a2ac4258e692ef8e64761910f4c0 NOTICES_SHA=71f58dc38b4c9b60beaec4459b97b0d08228ad8e5fe5e3a0f4fd7e7c66285925 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 04 May 2023 09:01:04 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 04 May 2023 09:01:04 GMT
USER 1001
# Thu, 04 May 2023 09:01:04 GMT
EXPOSE 9080 9443
# Thu, 04 May 2023 09:01:04 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 04 May 2023 09:01:05 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 04 May 2023 09:01:29 GMT
ARG VERBOSE=false
# Thu, 04 May 2023 09:01:29 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 04 May 2023 09:10:49 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Thu, 04 May 2023 09:10:52 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 04 May 2023 09:11:16 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:5449cdf62715285254f11ec0c25765e512ad9845213ad36c98569cba1994cf6b`  
		Last Modified: Tue, 18 Apr 2023 01:54:09 GMT  
		Size: 46.5 MB (46473382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e998d9cf0ff4f1b62b93f84bcfcea5a8337b5e417cc26d85818be82b95ad7d7b`  
		Last Modified: Tue, 18 Apr 2023 01:54:05 GMT  
		Size: 4.0 MB (3985359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fef513d476c6b3a002e6376adfc3fd71ad372b3e31fc089efb7f8e62cbe1ba4`  
		Last Modified: Thu, 04 May 2023 09:59:40 GMT  
		Size: 14.7 MB (14749568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64590c1ae2bfc750f272270aa7cdda582e1bc67ffe9c8da8e8a64ad393a13e2`  
		Last Modified: Thu, 04 May 2023 09:59:37 GMT  
		Size: 676.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c779928c880c3501b457ff598cd3be8370e4208e1fbae3c20a25fab4a95d46c`  
		Last Modified: Thu, 04 May 2023 09:59:37 GMT  
		Size: 9.8 KB (9810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af12c7f1bb55c97030d892a31724c252faa18535acac2ba98533eb8a7b761a42`  
		Last Modified: Thu, 04 May 2023 09:59:37 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a84369e7156b303d2ce82f418efc61cfd7112fad76074144fa9eb41ff9161c`  
		Last Modified: Thu, 04 May 2023 09:59:37 GMT  
		Size: 10.8 KB (10790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53bbdb11e71ed7dc31222f00e5ff0fe04f4c1bf52afefadd949c99a08057664`  
		Last Modified: Thu, 04 May 2023 09:59:37 GMT  
		Size: 2.6 MB (2626857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51f261dd70c3e933e6f2ab7d3fd483eb68f552d498187e2793a9382c179a92c`  
		Last Modified: Thu, 04 May 2023 10:00:08 GMT  
		Size: 359.1 MB (359070216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6cdc3aab258d17de43cb0f51d797bcb2f11397ec1b7abbf96a9ac4cd312a82`  
		Last Modified: Thu, 04 May 2023 09:59:54 GMT  
		Size: 939.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b446b0c4869bfafafb3100e62f316877141bdeb266c8a7f92e09210929d634`  
		Last Modified: Thu, 04 May 2023 09:59:55 GMT  
		Size: 13.8 MB (13849523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:760e8d979b9e4fb0388092e3d42f0141dd23db28dad947a417ec424ca37ec6fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **491.8 MB (491781106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65f4c43dfb823633c979908b71654ff583ab9f89fe8863eb8f72715815d11228`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Tue, 18 Apr 2023 01:27:22 GMT
ENV JAVA_VERSION=jdk-11.0.18+10_openj9-0.36.0
# Tue, 18 Apr 2023 01:28:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b7dae99808061eb1774e3af436453c48c30c01213a1613ca53df698276844f65';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.18%2B10_openj9-0.36.1/ibm-semeru-open-jre_aarch64_linux_11.0.18_10_openj9-0.36.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='f4eb9f501596a722a4be708361c1bfaa6b760cc7c885519d176cabba7a84d6e8';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.18%2B10_openj9-0.36.1/ibm-semeru-open-jre_ppc64le_linux_11.0.18_10_openj9-0.36.1.tar.gz';          ;;        amd64|x86_64)          ESUM='509a8c1e533c41896fddab187a8f6712ce1121d19eff71f4f023b58969147c9f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.18%2B10_openj9-0.36.1/ibm-semeru-open-jre_x64_linux_11.0.18_10_openj9-0.36.1.tar.gz';          ;;        s390x)          ESUM='ed6bbd482d9db361beb27510c5e88d882ba7232fc80409e35e33c08a5af7c7c0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.18%2B10_openj9-0.36.1/ibm-semeru-open-jre_s390x_linux_11.0.18_10_openj9-0.36.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 18 Apr 2023 01:28:44 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:28:44 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 18 Apr 2023 01:29:21 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 18 Apr 2023 03:22:01 GMT
ARG VERBOSE=false
# Tue, 18 Apr 2023 03:22:02 GMT
ARG OPENJ9_SCC=true
# Tue, 18 Apr 2023 03:22:02 GMT
ARG EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f
# Tue, 18 Apr 2023 03:22:02 GMT
ARG NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f
# Tue, 18 Apr 2023 03:22:02 GMT
ARG NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee
# Tue, 18 Apr 2023 03:22:03 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=23.0.0.3 org.opencontainers.image.revision=cl230320230319-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 18 Apr 2023 03:22:03 GMT
ENV LIBERTY_VERSION=23.0.0_03
# Tue, 18 Apr 2023 03:22:04 GMT
ARG LIBERTY_URL
# Tue, 18 Apr 2023 03:22:04 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 18 Apr 2023 03:22:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:22:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ibm/wlp/bin:/opt/ibm/helpers/build
# Tue, 18 Apr 2023 03:22:38 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=23.0.0.3 BuildLabel=cl230320230319-1900
# Tue, 18 Apr 2023 03:22:38 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 18 Apr 2023 03:22:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 18 Apr 2023 03:22:40 GMT
COPY dir:0f3e336b1e5adb84a625050153035561e1c9802a57b7b90b5a17ebb82adba489 in /opt/ibm/helpers/ 
# Tue, 18 Apr 2023 03:22:40 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 18 Apr 2023 03:22:42 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 18 Apr 2023 03:22:52 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 18 Apr 2023 03:22:52 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 18 Apr 2023 03:22:53 GMT
USER 1001
# Tue, 18 Apr 2023 03:22:53 GMT
EXPOSE 9080 9443
# Tue, 18 Apr 2023 03:22:53 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 18 Apr 2023 03:22:53 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 18 Apr 2023 03:24:12 GMT
ARG VERBOSE=false
# Tue, 18 Apr 2023 03:24:12 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 18 Apr 2023 03:42:36 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 18 Apr 2023 03:42:38 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 18 Apr 2023 03:43:32 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:85794083caa683460a3966622f58bd441fe30c836d2fac8e9c91e49e001d3643`  
		Last Modified: Tue, 18 Apr 2023 01:36:06 GMT  
		Size: 49.1 MB (49064121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106a33d97ef631121995c9a925c9775496289c5600d5e45253b017827ef017dc`  
		Last Modified: Tue, 18 Apr 2023 01:35:55 GMT  
		Size: 3.4 MB (3440865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18455e84e772570f2b4237e8e68a8f1d8826a2624ca52ff96bf174903ca6fe23`  
		Last Modified: Tue, 18 Apr 2023 04:42:19 GMT  
		Size: 14.5 MB (14453008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7635538bea4ccb1dda2924b7cfbaa0a907ce982a3c0caec42c33739a10134c7c`  
		Last Modified: Tue, 18 Apr 2023 04:42:14 GMT  
		Size: 684.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54392431d9ae322ac26e0f7b705d6ec4c4844504841ed42f400c3d334bb812ea`  
		Last Modified: Tue, 18 Apr 2023 04:42:14 GMT  
		Size: 9.8 KB (9813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814ed08c43a28cb1ac36baf2d66aa70a7805b53e1f2b71372f5fd8c28f194a45`  
		Last Modified: Tue, 18 Apr 2023 04:42:14 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5068d17fe7a9a7490355036914ab7b558029af4b4eb75328fec1731d064aeb`  
		Last Modified: Tue, 18 Apr 2023 04:42:14 GMT  
		Size: 10.8 KB (10800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64cdeab0e47f7b2da109d1b6373fab1d8a175f5a32bcb0b804e73ef9efef1185`  
		Last Modified: Tue, 18 Apr 2023 04:42:15 GMT  
		Size: 2.6 MB (2567820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43adf0ecd62787354bf4411d8c7a615f19ee7378fe37411e3c289c41043a850b`  
		Last Modified: Tue, 18 Apr 2023 04:43:10 GMT  
		Size: 359.0 MB (359034262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879a080240d3868afd61514aa86bc12099b18722cb60d7df56c0f83d367f4c9a`  
		Last Modified: Tue, 18 Apr 2023 04:42:36 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f6e55abb9856ab22a8026f02fac8b3fb9bb82239f7e9f93be9b8f34ce4f4d`  
		Last Modified: Tue, 18 Apr 2023 04:42:39 GMT  
		Size: 12.7 MB (12720640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:1275adf8005cd1086954da1dc9f7b3c37a1e7dbbd8e6535d07e679d5d74e4cad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.3 MB (486289021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f779491ab652577bd7e8af0ae25edda668931e498a3a8c2d312d457a82e8b513`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

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
# Tue, 18 Apr 2023 01:22:27 GMT
ENV JAVA_VERSION=jdk-11.0.18+10_openj9-0.36.0
# Tue, 18 Apr 2023 01:23:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b7dae99808061eb1774e3af436453c48c30c01213a1613ca53df698276844f65';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.18%2B10_openj9-0.36.1/ibm-semeru-open-jre_aarch64_linux_11.0.18_10_openj9-0.36.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='f4eb9f501596a722a4be708361c1bfaa6b760cc7c885519d176cabba7a84d6e8';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.18%2B10_openj9-0.36.1/ibm-semeru-open-jre_ppc64le_linux_11.0.18_10_openj9-0.36.1.tar.gz';          ;;        amd64|x86_64)          ESUM='509a8c1e533c41896fddab187a8f6712ce1121d19eff71f4f023b58969147c9f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.18%2B10_openj9-0.36.1/ibm-semeru-open-jre_x64_linux_11.0.18_10_openj9-0.36.1.tar.gz';          ;;        s390x)          ESUM='ed6bbd482d9db361beb27510c5e88d882ba7232fc80409e35e33c08a5af7c7c0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.18%2B10_openj9-0.36.1/ibm-semeru-open-jre_s390x_linux_11.0.18_10_openj9-0.36.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 18 Apr 2023 01:23:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:23:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 18 Apr 2023 01:24:30 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 18 Apr 2023 17:32:33 GMT
ARG VERBOSE=false
# Tue, 18 Apr 2023 17:32:33 GMT
ARG OPENJ9_SCC=true
# Tue, 18 Apr 2023 17:32:33 GMT
ARG EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f
# Tue, 18 Apr 2023 17:32:33 GMT
ARG NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f
# Tue, 18 Apr 2023 17:32:33 GMT
ARG NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee
# Tue, 18 Apr 2023 17:32:33 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=23.0.0.3 org.opencontainers.image.revision=cl230320230319-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 18 Apr 2023 17:32:33 GMT
ENV LIBERTY_VERSION=23.0.0_03
# Tue, 18 Apr 2023 17:32:33 GMT
ARG LIBERTY_URL
# Tue, 18 Apr 2023 17:32:33 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 18 Apr 2023 17:32:47 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 17:32:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ibm/wlp/bin:/opt/ibm/helpers/build
# Tue, 18 Apr 2023 17:32:47 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=23.0.0.3 BuildLabel=cl230320230319-1900
# Tue, 18 Apr 2023 17:32:47 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 18 Apr 2023 17:32:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 18 Apr 2023 17:32:48 GMT
COPY dir:0f3e336b1e5adb84a625050153035561e1c9802a57b7b90b5a17ebb82adba489 in /opt/ibm/helpers/ 
# Tue, 18 Apr 2023 17:32:48 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 18 Apr 2023 17:32:49 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 18 Apr 2023 17:32:52 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 18 Apr 2023 17:32:52 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 18 Apr 2023 17:32:52 GMT
USER 1001
# Tue, 18 Apr 2023 17:32:52 GMT
EXPOSE 9080 9443
# Tue, 18 Apr 2023 17:32:53 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 18 Apr 2023 17:32:53 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 18 Apr 2023 17:33:27 GMT
ARG VERBOSE=false
# Tue, 18 Apr 2023 17:33:27 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 18 Apr 2023 17:49:37 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 18 Apr 2023 17:49:43 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 18 Apr 2023 17:50:06 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:1476332455ffd401ffb7f5d61a786e7932494806470556e7cc64dcd5567c9d20`  
		Last Modified: Tue, 18 Apr 2023 01:30:13 GMT  
		Size: 47.7 MB (47746532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dfae40855592acf37b42000eddcb06a38a1466dd4bf1cf63c1fcc13eaa75a0`  
		Last Modified: Tue, 18 Apr 2023 01:30:07 GMT  
		Size: 4.3 MB (4337281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb4320a620534dbc4cac9618c98c0b4eb97d9eb5322e382a5d69563a48fa555`  
		Last Modified: Tue, 18 Apr 2023 18:34:48 GMT  
		Size: 14.5 MB (14452668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb39bcf44c402d3ec2c7b8c3576de50dbc2a69177873cc348bab3774178effda`  
		Last Modified: Tue, 18 Apr 2023 18:34:46 GMT  
		Size: 674.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d066056a5be90391993fa4de5913ff8757ae930ee6d08fe9e150fb2ef847a785`  
		Last Modified: Tue, 18 Apr 2023 18:34:46 GMT  
		Size: 9.8 KB (9813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d1494981ee30c918f55078f84114c778f310b93707d04bd2f6d1a22adf0a1f`  
		Last Modified: Tue, 18 Apr 2023 18:34:46 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2054750caefc0224225f9aa6ca54db8aee28a0d013dc45b6528b1c3a6c1a20`  
		Last Modified: Tue, 18 Apr 2023 18:34:46 GMT  
		Size: 10.8 KB (10785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5315df4944b59dd2f6caa09711accffa58cf11d3eff89f3163094247f890122d`  
		Last Modified: Tue, 18 Apr 2023 18:34:46 GMT  
		Size: 2.6 MB (2599646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a017c2ac7b10ed0a8b71f33edd1cdd97e6d83ebde7bc93cf0250a0bb763075`  
		Last Modified: Tue, 18 Apr 2023 18:35:17 GMT  
		Size: 359.0 MB (359034772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba93d8d3cb6abd10455db055698f7b780f2405a795204e211f52773d56cfd60`  
		Last Modified: Tue, 18 Apr 2023 18:35:00 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc006c698e1935e7aaa729f3df6686b9a8818e75d4712e08be37425ec90be78`  
		Last Modified: Tue, 18 Apr 2023 18:35:02 GMT  
		Size: 15.4 MB (15385887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
