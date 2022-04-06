## `websphere-liberty:kernel-java17-openj9`

```console
$ docker pull websphere-liberty@sha256:2483ee1237a1c69fe21a4f023ead2402d4a46baff9423e496360abeb8cc6d540
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:kernel-java17-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:d964d96f4e7a7bd52f19d9aa90d148fe206f4325873a0f1e85d61cb046f36c7c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (114008085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e12e85221f809f0f0268916da087e867ab7d6f8bb30ea9135a185fb1933b6d72`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:50 GMT
ADD file:b83df51ab7caf8a4dc35f730f5a18a59403300c59eecae4cf5779cba0f6fda6e in / 
# Tue, 05 Apr 2022 22:20:51 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:05:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 05 Apr 2022 23:06:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:36:31 GMT
ENV JAVA_VERSION=jdk-17.0.2+8_openj9-0.30.0
# Tue, 05 Apr 2022 23:36:35 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3bf1e63c4868f0f2bc7bd87ff46c2b24d3df4a4a0de63f142c7f83c8411950fc';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.2%2B8_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_17.0.2_8_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='f3ead398d99946af791006b4b5edde066ab277f372c402d76987b85522aff1dc';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.2%2B8_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_17.0.2_8_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='36757dcfc4891d41626fd75c0ebf16ae253eb40b7ac2afee39890cb9a5f0188b';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.2%2B8_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_17.0.2_8_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='bdb674f475cbeea9d528f179d2f4028bae6dee1a9f9551be6e39bb578fac9639';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.2%2B8_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_17.0.2_8_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 05 Apr 2022 23:36:36 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 23:36:36 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 05 Apr 2022 23:37:11 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 06 Apr 2022 06:05:41 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:05:41 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:05:41 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 06:05:41 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 06:05:41 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 06:05:41 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 06:05:42 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 06:05:42 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 06:05:42 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 06:05:49 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 06:05:49 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 06:05:50 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 06:05:50 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:05:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 06:05:51 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 06:05:51 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 06:05:52 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 06:06:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 06:06:00 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 06:06:00 GMT
USER 1001
# Wed, 06 Apr 2022 06:06:00 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 06:06:00 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 06:06:01 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e0b25ef516347a097d75f8aea6bc0f42a4e8e70b057e84d85098d51f96d458f9`  
		Last Modified: Tue, 05 Apr 2022 13:14:03 GMT  
		Size: 28.6 MB (28566292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bd2bc15eb1778663f55f9d16d0759ddc862631f9cf765680eb4f9dcd5894ea`  
		Last Modified: Tue, 05 Apr 2022 23:09:42 GMT  
		Size: 16.0 MB (16030073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057941e11059e7d1dab1775403a45ee6721a43a9606dd8d5776d0a88d00bd8f3`  
		Last Modified: Tue, 05 Apr 2022 23:40:41 GMT  
		Size: 47.7 MB (47727591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3e1b4584fbbe1a08e3a2b270305d5df3b28675a176a7a7fea2864ee2579579`  
		Last Modified: Tue, 05 Apr 2022 23:40:35 GMT  
		Size: 4.9 MB (4905243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebbe51cb69ce0ead934eb476611aa611f95f28626c9f6a72a38398f40a3a6094`  
		Last Modified: Wed, 06 Apr 2022 06:35:02 GMT  
		Size: 14.2 MB (14176967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00efbef07f3d8d817e5094a32441ccafb9059581bcbcba1305c9732ccd55263`  
		Last Modified: Wed, 06 Apr 2022 06:34:59 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc89ebd359561ed2487084a6f27406ab86cce6282ad85d5a512dd0d8ad0ac7fd`  
		Last Modified: Wed, 06 Apr 2022 06:34:59 GMT  
		Size: 9.7 KB (9672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d6a7336162c34c4c8cb74512f8edfff3bb318a4756a8b88d184b7431b1a4b2`  
		Last Modified: Wed, 06 Apr 2022 06:34:59 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a78f382c7cd5e7c672f4cf7f1128f9f3078b0ea27dc37a144b55c8aced14c16`  
		Last Modified: Wed, 06 Apr 2022 06:34:59 GMT  
		Size: 10.7 KB (10656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ddaebf34b65bad1176b7c4f2d2dec23ed383ae3cef2a7804db3ed7339606bfe`  
		Last Modified: Wed, 06 Apr 2022 06:34:59 GMT  
		Size: 2.6 MB (2580625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java17-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:dda3a7cbc778dbef67a99a2a7c48ff6127790133cd1f57ae24d278dffa267281
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118986603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf10fece5207c6232583d879f552d5f4b72e41e204985e7dd7502d6dea4d3063`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 06 Apr 2022 03:35:37 GMT
ADD file:c1af9c0e405f7eecbc87225c13709becfd46d66f87a4c5b8e30a1b82de7337e5 in / 
# Wed, 06 Apr 2022 03:35:41 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 04:53:37 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 06 Apr 2022 04:55:12 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 05:36:20 GMT
ENV JAVA_VERSION=jdk-17.0.2+8_openj9-0.30.0
# Wed, 06 Apr 2022 05:36:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3bf1e63c4868f0f2bc7bd87ff46c2b24d3df4a4a0de63f142c7f83c8411950fc';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.2%2B8_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_17.0.2_8_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='f3ead398d99946af791006b4b5edde066ab277f372c402d76987b85522aff1dc';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.2%2B8_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_17.0.2_8_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='36757dcfc4891d41626fd75c0ebf16ae253eb40b7ac2afee39890cb9a5f0188b';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.2%2B8_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_17.0.2_8_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='bdb674f475cbeea9d528f179d2f4028bae6dee1a9f9551be6e39bb578fac9639';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.2%2B8_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_17.0.2_8_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 06 Apr 2022 05:36:54 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 05:37:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 06 Apr 2022 05:38:12 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 06 Apr 2022 11:06:55 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:07:03 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:07:12 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 11:07:20 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 11:07:35 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 11:07:59 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 11:08:16 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 11:08:28 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 11:08:32 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 11:09:18 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 11:09:28 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 11:09:38 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 11:09:57 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:10:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 11:10:27 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 11:10:30 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 11:10:55 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 11:11:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 11:11:28 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 11:11:34 GMT
USER 1001
# Wed, 06 Apr 2022 11:11:41 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 11:11:46 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 11:11:53 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:83a2da48a82b52067676278a5eb4359bd7a79e7b57cabd370d77e11a9204121c`  
		Last Modified: Tue, 05 Apr 2022 13:16:22 GMT  
		Size: 33.3 MB (33291809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51134a7a9e0d0b603ce41f6ef7aa0f9d1a77696cb80e63a1e73b539ff51023b0`  
		Last Modified: Wed, 06 Apr 2022 05:08:30 GMT  
		Size: 17.2 MB (17204248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12c9f837337c5d1968bd291421f38dfa36c761769927b1273c5305cbfb818e9`  
		Last Modified: Wed, 06 Apr 2022 05:44:03 GMT  
		Size: 48.1 MB (48100204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4daaf56ed511bf82b1d3761b91ef30051cfb8471515a00950144f22c004545`  
		Last Modified: Wed, 06 Apr 2022 05:43:56 GMT  
		Size: 3.7 MB (3696393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d6d08d887f34ed7a33fb64e608bafcf82b397b5c7cc59be7f8c4a1a24b3b04`  
		Last Modified: Wed, 06 Apr 2022 12:00:47 GMT  
		Size: 14.2 MB (14177026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5b8f03f2574aa0e6c16d8bfc40f6349839afdb9b44c9446f60f286cb94b72a`  
		Last Modified: Wed, 06 Apr 2022 12:00:42 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf2aa38ecf6aba8e8a241c3bf4995d8e545d87627b33a15cd4ae3b283b10989`  
		Last Modified: Wed, 06 Apr 2022 12:00:42 GMT  
		Size: 9.7 KB (9678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc2e3c4b44b7bcd45a77ffee5685849219276ebe77b04ed867e473e9362fde2c`  
		Last Modified: Wed, 06 Apr 2022 12:00:41 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e148b89274b95dcb03031a9381eb2fe84c8de3191c4d88595a6cb95362bf3d3`  
		Last Modified: Wed, 06 Apr 2022 12:00:42 GMT  
		Size: 10.7 KB (10661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6309d4143cd81c07ec9432fdbec512aa5de99f8d828257cf049a31b69d00da`  
		Last Modified: Wed, 06 Apr 2022 12:00:42 GMT  
		Size: 2.5 MB (2495622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java17-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:9187849efd310b17495c5d713e75a7d1662b59ea935cdc4b0a0f642e3ab1d4ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110821652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46791a1da7d27cbb05cec81a56a13749d8137b276013f1612d846036bfcf8df0`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Apr 2022 22:42:05 GMT
ADD file:44b5cfe67740a0d7e33d6aa2c83d9918fdb30a0649aa3471e2f668dec1ba7f3a in / 
# Tue, 05 Apr 2022 22:42:07 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 22:59:29 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 05 Apr 2022 22:59:42 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:41:55 GMT
ENV JAVA_VERSION=jdk-17.0.2+8_openj9-0.30.0
# Tue, 05 Apr 2022 23:42:00 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3bf1e63c4868f0f2bc7bd87ff46c2b24d3df4a4a0de63f142c7f83c8411950fc';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.2%2B8_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_17.0.2_8_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='f3ead398d99946af791006b4b5edde066ab277f372c402d76987b85522aff1dc';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.2%2B8_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_17.0.2_8_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='36757dcfc4891d41626fd75c0ebf16ae253eb40b7ac2afee39890cb9a5f0188b';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.2%2B8_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_17.0.2_8_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='bdb674f475cbeea9d528f179d2f4028bae6dee1a9f9551be6e39bb578fac9639';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.2%2B8_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_17.0.2_8_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 05 Apr 2022 23:42:03 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 23:42:03 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 05 Apr 2022 23:42:36 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 06 Apr 2022 00:22:54 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:22:54 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:22:54 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 00:22:54 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 00:22:54 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 00:22:55 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 00:22:55 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 00:22:55 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 00:22:55 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 00:23:06 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:23:07 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 00:23:07 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 00:23:07 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:23:08 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 00:23:08 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 00:23:08 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 00:23:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 00:23:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 00:23:16 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 00:23:17 GMT
USER 1001
# Wed, 06 Apr 2022 00:23:17 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 00:23:17 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 00:23:17 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:502c7975d4ed549ab7d6e63b9ea10b0d24c1c3c12a33540d91d6739a0218faec`  
		Last Modified: Tue, 05 Apr 2022 13:17:47 GMT  
		Size: 27.1 MB (27084913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51699acdfda16fb15da1b4991b6dfd17e93efc6061b51d2928578f56536bea0`  
		Last Modified: Tue, 05 Apr 2022 23:02:31 GMT  
		Size: 15.7 MB (15738318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc7669e3948a392bbf20bfeee0d144e51dad8b914a2d175045c1a785c0372a1`  
		Last Modified: Tue, 05 Apr 2022 23:45:51 GMT  
		Size: 46.2 MB (46217068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b066bdfdd7f1da3cbafe1a9514b9ddcaff35ffdc9aa83effe2d3845659878fc7`  
		Last Modified: Tue, 05 Apr 2022 23:45:45 GMT  
		Size: 5.0 MB (4952439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d998d1aa890244cb4f940e67b76c9b2aae748e5bc9c6527e12ad16f14f62a4`  
		Last Modified: Wed, 06 Apr 2022 00:59:50 GMT  
		Size: 14.2 MB (14176988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395754c5fe8a49ba508841c7bbe305579644ca03a091e8cf9e311df0e06852fd`  
		Last Modified: Wed, 06 Apr 2022 00:59:47 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a371bfc65d563137aff9f027931dca7a8f200630afdfcaf1e2896dd0a481ef1`  
		Last Modified: Wed, 06 Apr 2022 00:59:47 GMT  
		Size: 9.7 KB (9673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43d67f7d34c7dcb304095bf87a0cb0995b4477afb2cecc951eee067cfd34541`  
		Last Modified: Wed, 06 Apr 2022 00:59:47 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7948c599425e713627c904fcf269dd03080d5b1f5c243a31831d13463727f29a`  
		Last Modified: Wed, 06 Apr 2022 00:59:47 GMT  
		Size: 10.7 KB (10665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bb78b472a0026bb56a3c275e9d5a031189a580e8f22b3bca09791a797e3352`  
		Last Modified: Wed, 06 Apr 2022 00:59:48 GMT  
		Size: 2.6 MB (2630623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
