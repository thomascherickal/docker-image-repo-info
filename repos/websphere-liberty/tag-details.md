<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `websphere-liberty`

-	[`websphere-liberty:22.0.0.3-full-java11-openj9`](#websphere-liberty22003-full-java11-openj9)
-	[`websphere-liberty:22.0.0.3-full-java17-openj9`](#websphere-liberty22003-full-java17-openj9)
-	[`websphere-liberty:22.0.0.3-full-java8-ibmjava`](#websphere-liberty22003-full-java8-ibmjava)
-	[`websphere-liberty:22.0.0.3-kernel-java11-openj9`](#websphere-liberty22003-kernel-java11-openj9)
-	[`websphere-liberty:22.0.0.3-kernel-java17-openj9`](#websphere-liberty22003-kernel-java17-openj9)
-	[`websphere-liberty:22.0.0.3-kernel-java8-ibmjava`](#websphere-liberty22003-kernel-java8-ibmjava)
-	[`websphere-liberty:22.0.0.6-full-java11-openj9`](#websphere-liberty22006-full-java11-openj9)
-	[`websphere-liberty:22.0.0.6-full-java17-openj9`](#websphere-liberty22006-full-java17-openj9)
-	[`websphere-liberty:22.0.0.6-full-java8-ibmjava`](#websphere-liberty22006-full-java8-ibmjava)
-	[`websphere-liberty:22.0.0.6-kernel-java11-openj9`](#websphere-liberty22006-kernel-java11-openj9)
-	[`websphere-liberty:22.0.0.6-kernel-java17-openj9`](#websphere-liberty22006-kernel-java17-openj9)
-	[`websphere-liberty:22.0.0.6-kernel-java8-ibmjava`](#websphere-liberty22006-kernel-java8-ibmjava)
-	[`websphere-liberty:full`](#websphere-libertyfull)
-	[`websphere-liberty:full-java11-openj9`](#websphere-libertyfull-java11-openj9)
-	[`websphere-liberty:full-java17-openj9`](#websphere-libertyfull-java17-openj9)
-	[`websphere-liberty:kernel`](#websphere-libertykernel)
-	[`websphere-liberty:kernel-java11-openj9`](#websphere-libertykernel-java11-openj9)
-	[`websphere-liberty:kernel-java17-openj9`](#websphere-libertykernel-java17-openj9)
-	[`websphere-liberty:latest`](#websphere-libertylatest)

## `websphere-liberty:22.0.0.3-full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:a4f95535dbae5af1988de261ab04a9f7e54d66fe5585b2eff6684d2d2325f801
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:22.0.0.3-full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:7863eef60812e806e2b3681ca81e811d21345b292509fe932ffa739cf8a723c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.7 MB (391681980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b922faad26dd31cfe125687ee0b32440434583af142260b9ac049f5b58bb7b84`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 19:04:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 19:05:01 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 19:56:56 GMT
ENV JAVA_VERSION=jdk-11.0.15+10_openj9-0.32.0
# Tue, 02 Aug 2022 19:58:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69e4a0b383c7b4187478ddb196de3cdc91560e2be40b8ef66354591e87c36e85';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5e82f7df54786c557d2d9e9ac22df655fd94b9702c73261390903ac87532d545';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='25d4d5e2bbe3eb19bcb9a76aec4b43d4eef5ad66200df3122118f69da5325cf6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='def85f1b00e9c65a8c3b5dcf4da0f1b04c17675b4ff9cd6f5dad61d8dcbd03d0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 19:58:02 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 19:58:02 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 19:58:37 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 13:23:06 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:23:06 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:49:36 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 03 Aug 2022 13:49:36 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 03 Aug 2022 13:49:36 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 03 Aug 2022 13:49:37 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 13:49:37 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 03 Aug 2022 13:49:37 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 13:49:37 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 13:49:49 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 13:49:49 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 13:49:49 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 03 Aug 2022 13:49:50 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:49:50 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 13:49:50 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 13:49:51 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 13:49:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 13:49:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 13:49:58 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 13:49:58 GMT
USER 1001
# Wed, 03 Aug 2022 13:49:58 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 13:49:59 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 13:49:59 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 03 Aug 2022 13:58:56 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:58:56 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 03 Aug 2022 14:06:29 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 03 Aug 2022 14:06:31 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 03 Aug 2022 14:07:00 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:a84b3718e4bf43f94609ec6fedf833567945fd97d9b8c324995df295d627fbb7`  
		Last Modified: Tue, 02 Aug 2022 20:06:46 GMT  
		Size: 47.7 MB (47691482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c02c82f8c35f778ae48a325cbccf65292ecbdea6e70272147ca65f72cda4dd`  
		Last Modified: Tue, 02 Aug 2022 20:06:39 GMT  
		Size: 4.2 MB (4183653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3749c336c8e53404196a4ef7487ba2d86efef38cf8411bbc2a3cda067d2dc6`  
		Last Modified: Wed, 03 Aug 2022 14:17:58 GMT  
		Size: 14.2 MB (14177312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286a0815b0f15d6ba25f9ef7336d04476b95f78ff0d913094ab8d59162ac4eb4`  
		Last Modified: Wed, 03 Aug 2022 14:17:55 GMT  
		Size: 688.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dbb0edbfa1622940b94507358149801014c356fd85354b507a664e8b33c3208`  
		Last Modified: Wed, 03 Aug 2022 14:17:55 GMT  
		Size: 9.8 KB (9752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e015528a7ee9944d3fc453eb424ea31c814aedb903a0d59922b0d7bcef43ec19`  
		Last Modified: Wed, 03 Aug 2022 14:17:55 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e30c2eb15f3ccf1c6976ad47be54051f14201c562f926735dd100dd62a7746`  
		Last Modified: Wed, 03 Aug 2022 14:17:55 GMT  
		Size: 10.7 KB (10728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0096aa4d96fecd1ef8fdaa46cc689973a803fe1f88d3c433b990597d945a4d`  
		Last Modified: Wed, 03 Aug 2022 14:17:55 GMT  
		Size: 2.6 MB (2557238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9eaf2aed7473e8d3d704c079a0a91e4205e1fcb15170bca4549f4bc7f11774`  
		Last Modified: Wed, 03 Aug 2022 14:18:51 GMT  
		Size: 264.0 MB (263983280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921ed5a24650baa105fbc75b1babb635281f64f90c446bc3afcef72cbf9414a5`  
		Last Modified: Wed, 03 Aug 2022 14:18:37 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa966a9d5eec9e9e5888a7c1dd7a9232a1a8cc59aff5f7e08d9ffbd8548067c`  
		Last Modified: Wed, 03 Aug 2022 14:18:39 GMT  
		Size: 14.5 MB (14464094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.3-full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:b387b46ac2aede0403b6c7a532b2fc124e80624ae3f57d202a10bfa352cd381a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.2 MB (396198824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b83fbd33d0d5691201c9534bddaef31938da3c25f23eeb9549550c335ac3dc4`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 07:16:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 07:18:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:46:26 GMT
ENV JAVA_VERSION=jdk-11.0.15+10_openj9-0.32.0
# Tue, 07 Jun 2022 09:48:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69e4a0b383c7b4187478ddb196de3cdc91560e2be40b8ef66354591e87c36e85';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5e82f7df54786c557d2d9e9ac22df655fd94b9702c73261390903ac87532d545';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='25d4d5e2bbe3eb19bcb9a76aec4b43d4eef5ad66200df3122118f69da5325cf6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='def85f1b00e9c65a8c3b5dcf4da0f1b04c17675b4ff9cd6f5dad61d8dcbd03d0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 09:48:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 09:48:28 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 07 Jun 2022 09:49:12 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 07 Jun 2022 11:28:13 GMT
ARG VERBOSE=false
# Tue, 07 Jun 2022 11:28:23 GMT
ARG OPENJ9_SCC=true
# Tue, 07 Jun 2022 11:45:50 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Tue, 07 Jun 2022 11:45:56 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Tue, 07 Jun 2022 11:46:01 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Tue, 07 Jun 2022 11:46:08 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 07 Jun 2022 11:46:12 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Tue, 07 Jun 2022 11:46:18 GMT
ARG LIBERTY_URL
# Tue, 07 Jun 2022 11:46:30 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 07 Jun 2022 11:47:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 11:47:37 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 11:47:42 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Tue, 07 Jun 2022 11:47:47 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 07 Jun 2022 11:48:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 27 Jun 2022 19:44:48 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Mon, 27 Jun 2022 19:44:50 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 27 Jun 2022 19:45:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 27 Jun 2022 19:45:33 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 27 Jun 2022 19:45:39 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Mon, 27 Jun 2022 19:45:45 GMT
USER 1001
# Mon, 27 Jun 2022 19:45:48 GMT
EXPOSE 9080 9443
# Mon, 27 Jun 2022 19:45:51 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 27 Jun 2022 19:45:52 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Mon, 27 Jun 2022 19:58:08 GMT
ARG VERBOSE=false
# Mon, 27 Jun 2022 19:58:15 GMT
ARG REPOSITORIES_PROPERTIES=
# Mon, 27 Jun 2022 20:07:57 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Mon, 27 Jun 2022 20:08:02 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Mon, 27 Jun 2022 20:09:00 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6c621e52fdf1e59e073b1c51c52e2e5a829be92510ef56949c609a03af2492`  
		Last Modified: Tue, 07 Jun 2022 07:30:19 GMT  
		Size: 17.2 MB (17203633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06eb9350ab17a87b8e47ac6a3389da7e21786ee038077cf7b627f90b125f1acf`  
		Last Modified: Tue, 07 Jun 2022 10:01:58 GMT  
		Size: 48.4 MB (48378487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc0d65d22cb0b40edcecacc4b8c684bc4bf1ddc89b24fd16e7abefba2b0c7df`  
		Last Modified: Tue, 07 Jun 2022 10:01:49 GMT  
		Size: 3.3 MB (3334009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef76e6542ec91cafb582fb1c5bb0b69febf2049a96ad5f1621c88fb7f9562c16`  
		Last Modified: Tue, 07 Jun 2022 12:59:50 GMT  
		Size: 14.2 MB (14177201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c885bba9a10ca381c3326209506ab8f13ac8d400ff75dfc7a339805126a665`  
		Last Modified: Tue, 07 Jun 2022 12:59:45 GMT  
		Size: 697.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5de8137fe948781fb75f2ad158d64ef8ab468b55acd0334bbb0952b9f8bf15e`  
		Last Modified: Mon, 27 Jun 2022 20:25:08 GMT  
		Size: 9.8 KB (9756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf9a1dd35843a103978be09996b8328854e8b6618384eb1c7a6a76403e378d5`  
		Last Modified: Mon, 27 Jun 2022 20:25:08 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350e88faaf3117044d4939dd3330f7b924058d964783d42a0ce2dc2c09803282`  
		Last Modified: Mon, 27 Jun 2022 20:25:08 GMT  
		Size: 10.7 KB (10749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3965897ce4df8879728ffb32e01ac3e07100c51948d00a876b37f329acbf979a`  
		Last Modified: Mon, 27 Jun 2022 20:25:08 GMT  
		Size: 2.5 MB (2502574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7049c641321b5e9d46ba65a57c1629aa123eb526e8dc25fedcd414d50f12021`  
		Last Modified: Mon, 27 Jun 2022 20:26:23 GMT  
		Size: 264.0 MB (263982251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3752ae785950d64a9b738c4bf6d349227fd08940832c2596371abe3309041acb`  
		Last Modified: Mon, 27 Jun 2022 20:26:00 GMT  
		Size: 951.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a710ab2d456a103e63b9bdef11ed81c307d9127b7a24118d45be8cd8de1f08`  
		Last Modified: Mon, 27 Jun 2022 20:26:03 GMT  
		Size: 13.3 MB (13303895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.3-full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:a51a60281eeabb4cbfd835a66d97fc98f37795e92619aa759f5a8b24bafce886
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **388.9 MB (388912059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47e26570d2865963cfc9eb48d9de5b4da1def367dce197d424e86cf1f1ab1f69`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:41:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 12:41:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:43:42 GMT
ENV JAVA_VERSION=jdk-11.0.15+10_openj9-0.32.0
# Tue, 02 Aug 2022 12:44:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69e4a0b383c7b4187478ddb196de3cdc91560e2be40b8ef66354591e87c36e85';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5e82f7df54786c557d2d9e9ac22df655fd94b9702c73261390903ac87532d545';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='25d4d5e2bbe3eb19bcb9a76aec4b43d4eef5ad66200df3122118f69da5325cf6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='def85f1b00e9c65a8c3b5dcf4da0f1b04c17675b4ff9cd6f5dad61d8dcbd03d0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 12:44:51 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 12:44:51 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 12:45:24 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 00:31:25 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:31:25 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:58:01 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 03 Aug 2022 00:58:01 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 03 Aug 2022 00:58:01 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 03 Aug 2022 00:58:01 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 00:58:01 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 03 Aug 2022 00:58:01 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 00:58:02 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 00:58:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 00:58:13 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 00:58:13 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 03 Aug 2022 00:58:13 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:58:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 00:58:14 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 00:58:14 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 00:58:14 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 00:58:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 00:58:20 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 00:58:20 GMT
USER 1001
# Wed, 03 Aug 2022 00:58:20 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 00:58:20 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 00:58:20 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 03 Aug 2022 01:06:04 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 01:06:04 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 03 Aug 2022 01:12:34 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 03 Aug 2022 01:12:39 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 03 Aug 2022 01:13:03 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:3f28b38375577480d13a8d78bab4c30073086c8a51a4ff217f32365aa0847411`  
		Last Modified: Tue, 02 Aug 2022 12:53:12 GMT  
		Size: 46.7 MB (46721680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3142744ed0637685528da62bbcb28da17d0b48fdc151bd52e7b22274eeb2c5da`  
		Last Modified: Tue, 02 Aug 2022 12:53:07 GMT  
		Size: 4.3 MB (4313565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30492df40f17354bae4842e7cb65ff16f7be8ba7841fdd50909013914aa1d432`  
		Last Modified: Wed, 03 Aug 2022 01:22:48 GMT  
		Size: 14.2 MB (14177343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a7b5d47544eb6069dca94107bb56c4011eb04fabf5b87d31bbf231b41543e7`  
		Last Modified: Wed, 03 Aug 2022 01:22:45 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19af7ac683e0c9f977a5fe78effccb9d3d7c84ff745b16b3d62344eb4c05e705`  
		Last Modified: Wed, 03 Aug 2022 01:22:46 GMT  
		Size: 9.8 KB (9753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4235d4d690d2954fdbd796bb63814a4937e66e29d3a51455983ff0216f5e17`  
		Last Modified: Wed, 03 Aug 2022 01:22:45 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308bfea86026b4b2dcdc9f45c7eccec55e5ef8d63c662d63238492a58be4485f`  
		Last Modified: Wed, 03 Aug 2022 01:22:45 GMT  
		Size: 10.7 KB (10733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd15fca7a7309d281421d7a5a80cbba7fe01dc65dbd0a1de2a459bbc240002d`  
		Last Modified: Wed, 03 Aug 2022 01:22:45 GMT  
		Size: 2.6 MB (2558728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679b9fa514e4f1e3799bc56f8d4f45eecf08d3aa5ba9bf568a5ead401d89e459`  
		Last Modified: Wed, 03 Aug 2022 01:23:30 GMT  
		Size: 264.0 MB (263981022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf8735b1be6119ecf1a33021efeda4d4452c80fe2df7ee78c611b7328dc52ef`  
		Last Modified: Wed, 03 Aug 2022 01:23:18 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a12e80695c64087666883b4e11528faabb74c814417bc022c7e88d042dbe26`  
		Last Modified: Wed, 03 Aug 2022 01:23:20 GMT  
		Size: 14.4 MB (14361837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.3-full-java17-openj9`

```console
$ docker pull websphere-liberty@sha256:21b3acd9ae51b0b8346a4f41217704719bffce2d09000c49603371ec392d747f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:22.0.0.3-full-java17-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:39d28dd4cf9c401a6b5caea766f055bf9315bdb879b98b0886920c2a0a277c98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.6 MB (392586304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e6b1aad381c6cc48fbf900e11ec776349597bf20ce76b9f52583aee76ae8057`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 19:04:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 19:05:01 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:00:47 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Tue, 02 Aug 2022 20:02:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f899948ea0c5dc80a66f801db585939a25a4ae7e1f21a9a8f3bf3749c3baa87f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9c54166490ac55a6bd26249b57eae5df4531635f4871e6642e7979affc894875';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='dad35fec82047e3a82c6e2dda8b53ee763b55aaedaed13b7b130856f4a3ffd35';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='4e2f631ad18c288e419db5c35295829dd7e83f4cd1be95252db06eb622b23090';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 20:02:05 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 20:02:05 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 20:02:40 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 13:23:34 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:23:34 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:50:04 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 03 Aug 2022 13:50:04 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 03 Aug 2022 13:50:05 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 03 Aug 2022 13:50:05 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 13:50:05 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 03 Aug 2022 13:50:05 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 13:50:05 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 13:50:17 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 13:50:17 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 13:50:18 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 03 Aug 2022 13:50:18 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:50:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 13:50:19 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 13:50:19 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 13:50:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 13:50:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 13:50:27 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 13:50:27 GMT
USER 1001
# Wed, 03 Aug 2022 13:50:27 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 13:50:27 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 13:50:27 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 03 Aug 2022 14:07:04 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 14:07:04 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 03 Aug 2022 14:14:43 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 03 Aug 2022 14:14:45 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 03 Aug 2022 14:15:15 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:7b6279e9931cb0efc3b60659be8fd46c95156f958f00818850fba3ac0ecd0616`  
		Last Modified: Tue, 02 Aug 2022 20:08:11 GMT  
		Size: 47.8 MB (47754438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e834be70bdf636e5c875d9e2badbf281d32ff675b9eb7db8768a2da9dbdf5e`  
		Last Modified: Tue, 02 Aug 2022 20:08:05 GMT  
		Size: 4.7 MB (4744099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f90721c8214905e9144d1f98a7d960e786e58f44e95a9cbb5d21154ccb780c9`  
		Last Modified: Wed, 03 Aug 2022 14:18:09 GMT  
		Size: 14.2 MB (14177316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c08027647eb22ecf679815d802601139122ee22138b8e591d5b0ab8fec068de`  
		Last Modified: Wed, 03 Aug 2022 14:18:06 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29afdd13e4761f268c20ff7f4d913391c7256a56e689c366acbcdf1e95ccbc6b`  
		Last Modified: Wed, 03 Aug 2022 14:18:06 GMT  
		Size: 9.8 KB (9751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b6c91acf376235b95d0f445059c7a276d5b645f302737235f7a4342484ff89`  
		Last Modified: Wed, 03 Aug 2022 14:18:06 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0c0bee7d0049340fd26007ddb7a644686e5b43cdda20e2b1a11d0f50ac2d3e`  
		Last Modified: Wed, 03 Aug 2022 14:18:06 GMT  
		Size: 10.7 KB (10727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d033366c675ea1b9f002473fa56ee48c022460ac9ee87cbac592db23ecf82a`  
		Last Modified: Wed, 03 Aug 2022 14:18:06 GMT  
		Size: 2.6 MB (2590466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ded20eaccadd0d3783dffb2e9dccac528566f0a929ee35c3993897e77b66f2b`  
		Last Modified: Wed, 03 Aug 2022 14:19:12 GMT  
		Size: 264.0 MB (263982825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e596f7985df21903e52f5bb84343d82dc8901802cc92566bd924e5973c88e8`  
		Last Modified: Wed, 03 Aug 2022 14:18:58 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4352c9e1a38a0d5524a35cf2af1401b41cca2c0ca4c16e693368d967c775425`  
		Last Modified: Wed, 03 Aug 2022 14:19:01 GMT  
		Size: 14.7 MB (14712238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.3-full-java17-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:22f72d2d5903fab8e73d8991ebcb4597a58791d43d244fa142ed565163f2dd82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.3 MB (396348546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67e6c22821babb35311b130ee136b627749ba9ff6630f86253e7e7e6bb34d693`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 07:16:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 07:18:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:52:39 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Tue, 07 Jun 2022 09:54:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f899948ea0c5dc80a66f801db585939a25a4ae7e1f21a9a8f3bf3749c3baa87f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9c54166490ac55a6bd26249b57eae5df4531635f4871e6642e7979affc894875';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='dad35fec82047e3a82c6e2dda8b53ee763b55aaedaed13b7b130856f4a3ffd35';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='4e2f631ad18c288e419db5c35295829dd7e83f4cd1be95252db06eb622b23090';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 09:54:20 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 09:54:22 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 07 Jun 2022 09:55:03 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 07 Jun 2022 11:31:51 GMT
ARG VERBOSE=false
# Tue, 07 Jun 2022 11:31:54 GMT
ARG OPENJ9_SCC=true
# Tue, 07 Jun 2022 11:50:14 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Tue, 07 Jun 2022 11:50:21 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Tue, 07 Jun 2022 11:50:25 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Tue, 07 Jun 2022 11:50:30 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 07 Jun 2022 11:50:35 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Tue, 07 Jun 2022 11:50:40 GMT
ARG LIBERTY_URL
# Tue, 07 Jun 2022 11:50:44 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 07 Jun 2022 11:51:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 11:51:53 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 11:51:57 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Tue, 07 Jun 2022 11:52:03 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 07 Jun 2022 11:52:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 27 Jun 2022 19:45:56 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Mon, 27 Jun 2022 19:45:58 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 27 Jun 2022 19:46:03 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 27 Jun 2022 19:46:28 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 27 Jun 2022 19:46:33 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Mon, 27 Jun 2022 19:46:37 GMT
USER 1001
# Mon, 27 Jun 2022 19:46:45 GMT
EXPOSE 9080 9443
# Mon, 27 Jun 2022 19:46:49 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 27 Jun 2022 19:46:53 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Mon, 27 Jun 2022 20:09:19 GMT
ARG VERBOSE=false
# Mon, 27 Jun 2022 20:09:22 GMT
ARG REPOSITORIES_PROPERTIES=
# Mon, 27 Jun 2022 20:18:45 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Mon, 27 Jun 2022 20:18:58 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Mon, 27 Jun 2022 20:20:11 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6c621e52fdf1e59e073b1c51c52e2e5a829be92510ef56949c609a03af2492`  
		Last Modified: Tue, 07 Jun 2022 07:30:19 GMT  
		Size: 17.2 MB (17203633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643e82d1f37eb2778986afcd7aa289e4f42b3c21d19b6dc2b50320f2836d580e`  
		Last Modified: Tue, 07 Jun 2022 10:03:59 GMT  
		Size: 48.1 MB (48115319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe972a29b91980b448bef8b1d66c53f248a582f57eb8476283dad120863f562`  
		Last Modified: Tue, 07 Jun 2022 10:03:52 GMT  
		Size: 3.7 MB (3691417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e5e59f0479d2819daf6bbf7e0092c0fd2870392053bbb1fa626cb335110747`  
		Last Modified: Tue, 07 Jun 2022 13:00:04 GMT  
		Size: 14.2 MB (14177183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf149583f4b3ca4aa8660caf345b205efea81d3fbbe1f4a26eb93122e7266bb`  
		Last Modified: Tue, 07 Jun 2022 12:59:59 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaf4913e1f3802720cdae39cead964ff5e53c908cffb78399ad317ca2ad4668`  
		Last Modified: Mon, 27 Jun 2022 20:25:18 GMT  
		Size: 9.8 KB (9758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb13ac17557dd68458fc2d34c1adfcab23e98b530637ef976a5adbd48f02896b`  
		Last Modified: Mon, 27 Jun 2022 20:25:17 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126f2b45ae77f5dd8e99944b9762f07fdbece5e587c9bc2d67978cea68de0a30`  
		Last Modified: Mon, 27 Jun 2022 20:25:18 GMT  
		Size: 10.7 KB (10745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9839bb93112137f7723692dbf85f749560347702eca16f7a6031270b3f8969b`  
		Last Modified: Mon, 27 Jun 2022 20:25:18 GMT  
		Size: 2.5 MB (2494859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eac4a34568a1f66dcb61955273f68fd37bf439e39634b03e3959d41f440e1b3`  
		Last Modified: Mon, 27 Jun 2022 20:26:57 GMT  
		Size: 264.0 MB (263983530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4605012ee68030f36f741887e0d2ec2d36b1a9309b14647f9b1933162008fb`  
		Last Modified: Mon, 27 Jun 2022 20:26:34 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55ff0653cbe3a1abce6891a879aeba15d93050f10bcd4779b3b8e8df577b0d5`  
		Last Modified: Mon, 27 Jun 2022 20:26:37 GMT  
		Size: 13.4 MB (13365839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.3-full-java17-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:5a9939a50544835441fca5bccd535bc9681d1defccd33ee9f2ac2f6567049b75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.2 MB (390194550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bedfa734a7638c1874f01b01c36ecb063b9e373349ad1673fbe159f6976cb9`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:41:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 12:41:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:47:17 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Tue, 02 Aug 2022 12:48:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f899948ea0c5dc80a66f801db585939a25a4ae7e1f21a9a8f3bf3749c3baa87f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9c54166490ac55a6bd26249b57eae5df4531635f4871e6642e7979affc894875';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='dad35fec82047e3a82c6e2dda8b53ee763b55aaedaed13b7b130856f4a3ffd35';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='4e2f631ad18c288e419db5c35295829dd7e83f4cd1be95252db06eb622b23090';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 12:48:20 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 12:48:20 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 12:48:53 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 00:31:56 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:31:56 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:58:28 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 03 Aug 2022 00:58:28 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 03 Aug 2022 00:58:29 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 03 Aug 2022 00:58:29 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 00:58:29 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 03 Aug 2022 00:58:29 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 00:58:29 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 00:58:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 00:58:39 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 00:58:39 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 03 Aug 2022 00:58:40 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:58:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 00:58:40 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 00:58:40 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 00:58:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 00:58:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 00:58:47 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 00:58:47 GMT
USER 1001
# Wed, 03 Aug 2022 00:58:47 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 00:58:47 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 00:58:47 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 03 Aug 2022 01:13:14 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 01:13:14 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 03 Aug 2022 01:19:45 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 03 Aug 2022 01:19:51 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 03 Aug 2022 01:20:15 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:8366f0be07eee724257935ccff074ac6069837c38e228be50a0b6f2e058ab16c`  
		Last Modified: Tue, 02 Aug 2022 12:54:24 GMT  
		Size: 46.2 MB (46241889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc471632f4e136d4fa45d0a7216573974cc332f3e9fa969846cb74f259e5e9cc`  
		Last Modified: Tue, 02 Aug 2022 12:54:19 GMT  
		Size: 4.9 MB (4939140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de9a36d5fbf5d611bab2200f4f80e76f6c340b3e718fc4833421954bd75e18c`  
		Last Modified: Wed, 03 Aug 2022 01:22:56 GMT  
		Size: 14.2 MB (14177336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d10e4a10caa655f57c14e23a3dc8b9f8cb97e1122630b7d5c1d5ae2350ef70`  
		Last Modified: Wed, 03 Aug 2022 01:22:54 GMT  
		Size: 690.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd0d83f98fb0b32d0d0090042a444c124da512520447d43c6bc9fda6f444cd8`  
		Last Modified: Wed, 03 Aug 2022 01:22:54 GMT  
		Size: 9.8 KB (9755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a16c5a35f7fea6399e22685da0bffd79be7dff2d4903f7a2e10cac53ecf1ce`  
		Last Modified: Wed, 03 Aug 2022 01:22:54 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5d404e1c64ec9327501ac0db62a38586f0184219713589552c3958fd3ef29a`  
		Last Modified: Wed, 03 Aug 2022 01:22:54 GMT  
		Size: 10.7 KB (10733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b82e7c16e18adecba092f08fb55ba338d14c4ee8c6212d03895751bf0e245af`  
		Last Modified: Wed, 03 Aug 2022 01:22:54 GMT  
		Size: 2.5 MB (2548608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ad9e21893ba7f87c2fda2a0de8622a175c2523060981915ed33c104220d099`  
		Last Modified: Wed, 03 Aug 2022 01:23:49 GMT  
		Size: 264.0 MB (263981632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da50604a0e472606eee6464fa88fa42a52d72561f086e3c423ee0cbe5f0e342`  
		Last Modified: Wed, 03 Aug 2022 01:23:37 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2029445e38fb6c370d3304f99f506d340a140a407f7ac30fde3efbe0b7a6b97f`  
		Last Modified: Wed, 03 Aug 2022 01:23:39 GMT  
		Size: 15.5 MB (15508061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.3-full-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:bfd6366e92d611358af31e9ef488408b6f4b3b3687dff39bb7f3b4a88f563146
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:22.0.0.3-full-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:6e9bc4ea32640a4e5705aa1835b5829986beed9a7e48a688276868e6a2ee1853
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **458.8 MB (458751119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef01948e139658dea4372158fc3eef2003b049b9e6abddedb32de04e4b6bc2e`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:09:52 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 02 Aug 2022 20:10:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:10:01 GMT
ENV JAVA_VERSION=8.0.7.11
# Tue, 02 Aug 2022 20:10:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 02 Aug 2022 20:10:53 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 03 Aug 2022 13:22:32 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:22:32 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:49:08 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 03 Aug 2022 13:49:08 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 03 Aug 2022 13:49:08 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 03 Aug 2022 13:49:08 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 13:49:09 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 03 Aug 2022 13:49:09 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 13:49:09 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 13:49:22 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 13:49:22 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 13:49:22 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 03 Aug 2022 13:49:22 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:49:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 13:49:23 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 13:49:23 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 13:49:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 13:49:33 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 13:49:33 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 03 Aug 2022 13:49:33 GMT
USER 1001
# Wed, 03 Aug 2022 13:49:33 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 13:49:34 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 13:49:34 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 03 Aug 2022 13:50:32 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:50:33 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 03 Aug 2022 13:58:08 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 03 Aug 2022 13:58:09 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 03 Aug 2022 13:58:39 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6715a1bb89fcf5e91403be2bc6130f23e6b3cfd0da73e6b09e937d028409d3`  
		Last Modified: Tue, 02 Aug 2022 20:13:24 GMT  
		Size: 3.0 MB (2957815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1607240ca884b25e20b8db8c53c4aea519b76a50e23c19a40aaadd508939589`  
		Last Modified: Tue, 02 Aug 2022 20:13:35 GMT  
		Size: 129.1 MB (129092301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd376116f0255a5936ba040aa80c0f3b34cd853737517b6e1e219336ea6bd67a`  
		Last Modified: Wed, 03 Aug 2022 14:17:48 GMT  
		Size: 14.1 MB (14079596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b756764ec4146955c479f2b9eb2556b60129720dd763fa8b57f5d99952db1ca`  
		Last Modified: Wed, 03 Aug 2022 14:17:45 GMT  
		Size: 686.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122022c189e35d2c9d2ed2b46ef65b13a2555e4ca6af1d5d942d079635f237bd`  
		Last Modified: Wed, 03 Aug 2022 14:17:45 GMT  
		Size: 9.8 KB (9755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2718333544b606e7d11939378d0696fdd34aa77cabf27be95942171c7b3d35c0`  
		Last Modified: Wed, 03 Aug 2022 14:17:45 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a63c196c6194314faa0a14e2ac5d111d8395522b2c03056656c53c7a1a11ff5`  
		Last Modified: Wed, 03 Aug 2022 14:17:45 GMT  
		Size: 10.7 KB (10734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd896b840d88bcfa57c5076c131df6acecf3b451f11be38e30594c6a81e7c0d2`  
		Last Modified: Wed, 03 Aug 2022 14:17:46 GMT  
		Size: 5.8 MB (5757989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1420c470f43f1fa7cfabea195e322513c036dd7cd57de75741937e2ad8afdee5`  
		Last Modified: Wed, 03 Aug 2022 14:18:30 GMT  
		Size: 264.0 MB (263982873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad148dc2482664d79684b899b22df0e8e0014418f83256e790f9cfc0109ecc23`  
		Last Modified: Wed, 03 Aug 2022 14:18:17 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67a2d2b3517b18ad88c5a076e6dd339e323a87e30bd49876f013a2620085e16`  
		Last Modified: Wed, 03 Aug 2022 14:18:18 GMT  
		Size: 16.1 MB (16147881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.3-full-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:eda2c6068cbe04b53156d4958d6862df4f404a1d2e1ca9cd9f8aba99cad93303
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **459.7 MB (459697426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d1073a06195957b527cb03fed2babe7779835961c350e7f165cc4e80afcb55e`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:49:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 07 Jun 2022 08:50:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 18:31:53 GMT
ENV JAVA_VERSION=8.0.7.11
# Wed, 29 Jun 2022 18:33:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 29 Jun 2022 18:33:35 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 29 Jun 2022 19:03:57 GMT
ARG VERBOSE=false
# Wed, 29 Jun 2022 19:04:05 GMT
ARG OPENJ9_SCC=true
# Wed, 29 Jun 2022 19:20:58 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 29 Jun 2022 19:21:07 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 29 Jun 2022 19:21:10 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 29 Jun 2022 19:21:14 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 29 Jun 2022 19:21:18 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 29 Jun 2022 19:21:22 GMT
ARG LIBERTY_URL
# Wed, 29 Jun 2022 19:21:31 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 29 Jun 2022 19:22:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 19:22:37 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Jun 2022 19:22:40 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 29 Jun 2022 19:22:44 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 29 Jun 2022 19:22:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 29 Jun 2022 19:22:58 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 29 Jun 2022 19:23:01 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 29 Jun 2022 19:23:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 29 Jun 2022 19:23:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 29 Jun 2022 19:23:42 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 29 Jun 2022 19:23:49 GMT
USER 1001
# Wed, 29 Jun 2022 19:23:55 GMT
EXPOSE 9080 9443
# Wed, 29 Jun 2022 19:23:59 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 29 Jun 2022 19:24:04 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 29 Jun 2022 19:24:32 GMT
ARG VERBOSE=false
# Wed, 29 Jun 2022 19:24:38 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 29 Jun 2022 19:33:58 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 29 Jun 2022 19:34:03 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 29 Jun 2022 19:35:13 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4a22aedc3b9f2593635b0a3f6fe64e6dd424850b9782f66e88c8c162926d6a`  
		Last Modified: Tue, 07 Jun 2022 08:54:16 GMT  
		Size: 3.1 MB (3082521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448aed354e59dc01b7da997655c86778001067ef107a5c1fb36a7c38fcf5fdda`  
		Last Modified: Wed, 29 Jun 2022 18:38:02 GMT  
		Size: 128.6 MB (128629743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315aa69ea9848470ad9633185d0c939f3350f1bbc367bd888dcec33016e3d36e`  
		Last Modified: Wed, 29 Jun 2022 19:37:23 GMT  
		Size: 14.4 MB (14407322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9b364212ac3c9cd51f4b4ac71547955228a430e65573ebb26408a3ade7aaf4`  
		Last Modified: Wed, 29 Jun 2022 19:37:18 GMT  
		Size: 680.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe9a429664a923f6fd2cac536b42514ada9fbe2965585093f4ccd98193bbd27`  
		Last Modified: Wed, 29 Jun 2022 19:37:18 GMT  
		Size: 9.8 KB (9758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aded815fcdabc6d10f987c0f48c20e81c39776ab6f05bf562f44e8dcb306551`  
		Last Modified: Wed, 29 Jun 2022 19:37:18 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca4dbddc845e7d48a289b08f7fbd411cf5d2e3f7d335aa3f1238cf6d9cf6b2a`  
		Last Modified: Wed, 29 Jun 2022 19:37:18 GMT  
		Size: 10.7 KB (10740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419732f323d71a8ab58836655c727f3c088fae1bda27617a74fb6b247d0917c2`  
		Last Modified: Wed, 29 Jun 2022 19:37:19 GMT  
		Size: 5.3 MB (5328315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c005090f8d74a5aaddefe0b8048dba5c6dce706d5d0eb99514fa242952a116a5`  
		Last Modified: Wed, 29 Jun 2022 19:37:57 GMT  
		Size: 264.0 MB (263983723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbcfaa24bd58fc44da3c7d9df46a3b6c50fa08bb2a8c009e87c7a11377690bf`  
		Last Modified: Wed, 29 Jun 2022 19:37:33 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92271c0b6e06d0b77465d4d3ff4658210c4793b4e8b7277579ecc151424c2ad`  
		Last Modified: Wed, 29 Jun 2022 19:37:35 GMT  
		Size: 13.8 MB (13800544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.3-full-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:d92c52eb0aa0b2f7c46b7605aa6e7f0b41f0217f0969ba6ca5499f8c3250d99c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **454.1 MB (454149122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd17c5d48248eea5a6e7beaa112312db598bc0f4ed2c4a6916f6ff324f9caca2`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:01:57 GMT
ADD file:3d2e9b401524527b395347bc3847be7c9cb465b9a214a1a1d31e74330e293c45 in / 
# Tue, 02 Aug 2022 01:01:58 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 13:19:12 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 02 Aug 2022 13:19:25 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:19:25 GMT
ENV JAVA_VERSION=8.0.7.11
# Tue, 02 Aug 2022 13:20:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 02 Aug 2022 13:20:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 03 Aug 2022 00:30:47 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:30:48 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:57:34 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 03 Aug 2022 00:57:34 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 03 Aug 2022 00:57:34 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 03 Aug 2022 00:57:34 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 00:57:34 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 03 Aug 2022 00:57:34 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 00:57:34 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 00:57:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 00:57:45 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 00:57:45 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 03 Aug 2022 00:57:45 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:57:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 00:57:46 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 00:57:46 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 00:57:47 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 00:57:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 00:57:54 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 03 Aug 2022 00:57:54 GMT
USER 1001
# Wed, 03 Aug 2022 00:57:55 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 00:57:55 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 00:57:55 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 03 Aug 2022 00:58:53 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:58:53 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 03 Aug 2022 01:05:22 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 03 Aug 2022 01:05:26 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 03 Aug 2022 01:05:51 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:be3ed498266c519f84268ff1f02085fa249c0e32fb60a59466e24c862b5f094b`  
		Last Modified: Tue, 02 Aug 2022 01:03:25 GMT  
		Size: 25.4 MB (25369584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2ed0adcefe11b30e3dff027bcb1cb9fe759f39f50b008bafb3644d3d2fcba8`  
		Last Modified: Tue, 02 Aug 2022 13:22:41 GMT  
		Size: 2.7 MB (2671706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745854ef92308f8e24873e2cf64eb998c725371b7d10ba8318989b37bba26f33`  
		Last Modified: Tue, 02 Aug 2022 13:22:49 GMT  
		Size: 126.1 MB (126143967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974fefeaf21f90e751b044175d4bf9e9d40d602855e046cd5b7275a3c5ec3fb8`  
		Last Modified: Wed, 03 Aug 2022 01:22:40 GMT  
		Size: 14.1 MB (14079782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c9b03efe4042d882baf28dd6693403668d048e2770c3cba94663f44fb58a54`  
		Last Modified: Wed, 03 Aug 2022 01:22:38 GMT  
		Size: 683.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e47b30dd51ef2a8cf86e72c1e2df4374bc8d6c38542199d5c9cc25c983bd630`  
		Last Modified: Wed, 03 Aug 2022 01:22:38 GMT  
		Size: 9.8 KB (9753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3104abd5350f6fb1869fa4a2199bdefa3c7d5b5497212915bbaf38a8ca13a60c`  
		Last Modified: Wed, 03 Aug 2022 01:22:38 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6789e2f9b06fdc267ba249d75c22d4c5cbcd003479b990405cab04d9a97252c1`  
		Last Modified: Wed, 03 Aug 2022 01:22:38 GMT  
		Size: 10.7 KB (10737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b90efb0815342eda22636b96bf2af4b46d9a66cef700fce14817216fbcad375`  
		Last Modified: Wed, 03 Aug 2022 01:22:38 GMT  
		Size: 5.9 MB (5883006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f5dcf09d93ec54f1001e95f730460705aa4f9ed90711635d90e3b9360b16aa`  
		Last Modified: Wed, 03 Aug 2022 01:23:13 GMT  
		Size: 264.0 MB (263981040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18792580c011b53a8a352ae13556b8a31bc7b90c63b28740122c29adb42351fd`  
		Last Modified: Wed, 03 Aug 2022 01:23:01 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42cc886369bd4a3b79fe91e347b5a1275778228efae2343f0e6cf38b092d2fd`  
		Last Modified: Wed, 03 Aug 2022 01:23:03 GMT  
		Size: 16.0 MB (15997643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.3-kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:f98a0ecd76cfb143a15415b168dd98120aaf63a3f1434ce4d1a458351c2a8d60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:22.0.0.3-kernel-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:687fcdc506dfde48f13c1172f850454e812962c4d909eeae8054a9a1bb3ae39e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113233662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38b7cec731b0c7607343ca0be986589bfa248921cc2bc49fc025d3597859e0cf`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 19:04:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 19:05:01 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 19:56:56 GMT
ENV JAVA_VERSION=jdk-11.0.15+10_openj9-0.32.0
# Tue, 02 Aug 2022 19:58:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69e4a0b383c7b4187478ddb196de3cdc91560e2be40b8ef66354591e87c36e85';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5e82f7df54786c557d2d9e9ac22df655fd94b9702c73261390903ac87532d545';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='25d4d5e2bbe3eb19bcb9a76aec4b43d4eef5ad66200df3122118f69da5325cf6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='def85f1b00e9c65a8c3b5dcf4da0f1b04c17675b4ff9cd6f5dad61d8dcbd03d0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 19:58:02 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 19:58:02 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 19:58:37 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 13:23:06 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:23:06 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:49:36 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 03 Aug 2022 13:49:36 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 03 Aug 2022 13:49:36 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 03 Aug 2022 13:49:37 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 13:49:37 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 03 Aug 2022 13:49:37 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 13:49:37 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 13:49:49 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 13:49:49 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 13:49:49 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 03 Aug 2022 13:49:50 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:49:50 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 13:49:50 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 13:49:51 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 13:49:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 13:49:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 13:49:58 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 13:49:58 GMT
USER 1001
# Wed, 03 Aug 2022 13:49:58 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 13:49:59 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 13:49:59 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:a84b3718e4bf43f94609ec6fedf833567945fd97d9b8c324995df295d627fbb7`  
		Last Modified: Tue, 02 Aug 2022 20:06:46 GMT  
		Size: 47.7 MB (47691482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c02c82f8c35f778ae48a325cbccf65292ecbdea6e70272147ca65f72cda4dd`  
		Last Modified: Tue, 02 Aug 2022 20:06:39 GMT  
		Size: 4.2 MB (4183653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3749c336c8e53404196a4ef7487ba2d86efef38cf8411bbc2a3cda067d2dc6`  
		Last Modified: Wed, 03 Aug 2022 14:17:58 GMT  
		Size: 14.2 MB (14177312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286a0815b0f15d6ba25f9ef7336d04476b95f78ff0d913094ab8d59162ac4eb4`  
		Last Modified: Wed, 03 Aug 2022 14:17:55 GMT  
		Size: 688.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dbb0edbfa1622940b94507358149801014c356fd85354b507a664e8b33c3208`  
		Last Modified: Wed, 03 Aug 2022 14:17:55 GMT  
		Size: 9.8 KB (9752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e015528a7ee9944d3fc453eb424ea31c814aedb903a0d59922b0d7bcef43ec19`  
		Last Modified: Wed, 03 Aug 2022 14:17:55 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e30c2eb15f3ccf1c6976ad47be54051f14201c562f926735dd100dd62a7746`  
		Last Modified: Wed, 03 Aug 2022 14:17:55 GMT  
		Size: 10.7 KB (10728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0096aa4d96fecd1ef8fdaa46cc689973a803fe1f88d3c433b990597d945a4d`  
		Last Modified: Wed, 03 Aug 2022 14:17:55 GMT  
		Size: 2.6 MB (2557238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.3-kernel-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:64b8fe5a8431e263370d4c682bfe279fdea6186edd9abdbb96b4885af0714322
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118911727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb0f7baa3aafb00b231def11b2b7e7b376c826966ad642c9b73bee9229efd8d0`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 07:16:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 07:18:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:46:26 GMT
ENV JAVA_VERSION=jdk-11.0.15+10_openj9-0.32.0
# Tue, 07 Jun 2022 09:48:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69e4a0b383c7b4187478ddb196de3cdc91560e2be40b8ef66354591e87c36e85';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5e82f7df54786c557d2d9e9ac22df655fd94b9702c73261390903ac87532d545';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='25d4d5e2bbe3eb19bcb9a76aec4b43d4eef5ad66200df3122118f69da5325cf6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='def85f1b00e9c65a8c3b5dcf4da0f1b04c17675b4ff9cd6f5dad61d8dcbd03d0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 09:48:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 09:48:28 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 07 Jun 2022 09:49:12 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 07 Jun 2022 11:28:13 GMT
ARG VERBOSE=false
# Tue, 07 Jun 2022 11:28:23 GMT
ARG OPENJ9_SCC=true
# Tue, 07 Jun 2022 11:45:50 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Tue, 07 Jun 2022 11:45:56 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Tue, 07 Jun 2022 11:46:01 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Tue, 07 Jun 2022 11:46:08 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 07 Jun 2022 11:46:12 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Tue, 07 Jun 2022 11:46:18 GMT
ARG LIBERTY_URL
# Tue, 07 Jun 2022 11:46:30 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 07 Jun 2022 11:47:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 11:47:37 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 11:47:42 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Tue, 07 Jun 2022 11:47:47 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 07 Jun 2022 11:48:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 27 Jun 2022 19:44:48 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Mon, 27 Jun 2022 19:44:50 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 27 Jun 2022 19:45:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 27 Jun 2022 19:45:33 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 27 Jun 2022 19:45:39 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Mon, 27 Jun 2022 19:45:45 GMT
USER 1001
# Mon, 27 Jun 2022 19:45:48 GMT
EXPOSE 9080 9443
# Mon, 27 Jun 2022 19:45:51 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 27 Jun 2022 19:45:52 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6c621e52fdf1e59e073b1c51c52e2e5a829be92510ef56949c609a03af2492`  
		Last Modified: Tue, 07 Jun 2022 07:30:19 GMT  
		Size: 17.2 MB (17203633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06eb9350ab17a87b8e47ac6a3389da7e21786ee038077cf7b627f90b125f1acf`  
		Last Modified: Tue, 07 Jun 2022 10:01:58 GMT  
		Size: 48.4 MB (48378487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc0d65d22cb0b40edcecacc4b8c684bc4bf1ddc89b24fd16e7abefba2b0c7df`  
		Last Modified: Tue, 07 Jun 2022 10:01:49 GMT  
		Size: 3.3 MB (3334009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef76e6542ec91cafb582fb1c5bb0b69febf2049a96ad5f1621c88fb7f9562c16`  
		Last Modified: Tue, 07 Jun 2022 12:59:50 GMT  
		Size: 14.2 MB (14177201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c885bba9a10ca381c3326209506ab8f13ac8d400ff75dfc7a339805126a665`  
		Last Modified: Tue, 07 Jun 2022 12:59:45 GMT  
		Size: 697.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5de8137fe948781fb75f2ad158d64ef8ab468b55acd0334bbb0952b9f8bf15e`  
		Last Modified: Mon, 27 Jun 2022 20:25:08 GMT  
		Size: 9.8 KB (9756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf9a1dd35843a103978be09996b8328854e8b6618384eb1c7a6a76403e378d5`  
		Last Modified: Mon, 27 Jun 2022 20:25:08 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350e88faaf3117044d4939dd3330f7b924058d964783d42a0ce2dc2c09803282`  
		Last Modified: Mon, 27 Jun 2022 20:25:08 GMT  
		Size: 10.7 KB (10749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3965897ce4df8879728ffb32e01ac3e07100c51948d00a876b37f329acbf979a`  
		Last Modified: Mon, 27 Jun 2022 20:25:08 GMT  
		Size: 2.5 MB (2502574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.3-kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:2f2d3792c26e704cd985b3e2bbc7f4460db0905c312b4126287c50cf5d945ba1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110568254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57f6a373fa1c3c91023d8227a8d78e69a3db018533c0c6d6edbcd57fdc262630`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:41:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 12:41:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:43:42 GMT
ENV JAVA_VERSION=jdk-11.0.15+10_openj9-0.32.0
# Tue, 02 Aug 2022 12:44:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69e4a0b383c7b4187478ddb196de3cdc91560e2be40b8ef66354591e87c36e85';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5e82f7df54786c557d2d9e9ac22df655fd94b9702c73261390903ac87532d545';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='25d4d5e2bbe3eb19bcb9a76aec4b43d4eef5ad66200df3122118f69da5325cf6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='def85f1b00e9c65a8c3b5dcf4da0f1b04c17675b4ff9cd6f5dad61d8dcbd03d0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 12:44:51 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 12:44:51 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 12:45:24 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 00:31:25 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:31:25 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:58:01 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 03 Aug 2022 00:58:01 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 03 Aug 2022 00:58:01 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 03 Aug 2022 00:58:01 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 00:58:01 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 03 Aug 2022 00:58:01 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 00:58:02 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 00:58:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 00:58:13 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 00:58:13 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 03 Aug 2022 00:58:13 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:58:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 00:58:14 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 00:58:14 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 00:58:14 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 00:58:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 00:58:20 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 00:58:20 GMT
USER 1001
# Wed, 03 Aug 2022 00:58:20 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 00:58:20 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 00:58:20 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:3f28b38375577480d13a8d78bab4c30073086c8a51a4ff217f32365aa0847411`  
		Last Modified: Tue, 02 Aug 2022 12:53:12 GMT  
		Size: 46.7 MB (46721680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3142744ed0637685528da62bbcb28da17d0b48fdc151bd52e7b22274eeb2c5da`  
		Last Modified: Tue, 02 Aug 2022 12:53:07 GMT  
		Size: 4.3 MB (4313565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30492df40f17354bae4842e7cb65ff16f7be8ba7841fdd50909013914aa1d432`  
		Last Modified: Wed, 03 Aug 2022 01:22:48 GMT  
		Size: 14.2 MB (14177343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a7b5d47544eb6069dca94107bb56c4011eb04fabf5b87d31bbf231b41543e7`  
		Last Modified: Wed, 03 Aug 2022 01:22:45 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19af7ac683e0c9f977a5fe78effccb9d3d7c84ff745b16b3d62344eb4c05e705`  
		Last Modified: Wed, 03 Aug 2022 01:22:46 GMT  
		Size: 9.8 KB (9753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4235d4d690d2954fdbd796bb63814a4937e66e29d3a51455983ff0216f5e17`  
		Last Modified: Wed, 03 Aug 2022 01:22:45 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308bfea86026b4b2dcdc9f45c7eccec55e5ef8d63c662d63238492a58be4485f`  
		Last Modified: Wed, 03 Aug 2022 01:22:45 GMT  
		Size: 10.7 KB (10733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd15fca7a7309d281421d7a5a80cbba7fe01dc65dbd0a1de2a459bbc240002d`  
		Last Modified: Wed, 03 Aug 2022 01:22:45 GMT  
		Size: 2.6 MB (2558728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.3-kernel-java17-openj9`

```console
$ docker pull websphere-liberty@sha256:7f3956575fbb2abeca2fa274e92f7d42e684d05c98266ae6a5ad7bf64597d3d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:22.0.0.3-kernel-java17-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:59f425b44acfc13f3ed75cf25382523c30bb8039fc4e39275c55685408f0f753
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113890293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82494836ad52168560a18d1a937ed40c2222a26a51c0222020822f87d53fe5af`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 19:04:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 19:05:01 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:00:47 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Tue, 02 Aug 2022 20:02:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f899948ea0c5dc80a66f801db585939a25a4ae7e1f21a9a8f3bf3749c3baa87f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9c54166490ac55a6bd26249b57eae5df4531635f4871e6642e7979affc894875';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='dad35fec82047e3a82c6e2dda8b53ee763b55aaedaed13b7b130856f4a3ffd35';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='4e2f631ad18c288e419db5c35295829dd7e83f4cd1be95252db06eb622b23090';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 20:02:05 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 20:02:05 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 20:02:40 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 13:23:34 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:23:34 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:50:04 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 03 Aug 2022 13:50:04 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 03 Aug 2022 13:50:05 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 03 Aug 2022 13:50:05 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 13:50:05 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 03 Aug 2022 13:50:05 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 13:50:05 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 13:50:17 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 13:50:17 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 13:50:18 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 03 Aug 2022 13:50:18 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:50:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 13:50:19 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 13:50:19 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 13:50:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 13:50:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 13:50:27 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 13:50:27 GMT
USER 1001
# Wed, 03 Aug 2022 13:50:27 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 13:50:27 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 13:50:27 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:7b6279e9931cb0efc3b60659be8fd46c95156f958f00818850fba3ac0ecd0616`  
		Last Modified: Tue, 02 Aug 2022 20:08:11 GMT  
		Size: 47.8 MB (47754438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e834be70bdf636e5c875d9e2badbf281d32ff675b9eb7db8768a2da9dbdf5e`  
		Last Modified: Tue, 02 Aug 2022 20:08:05 GMT  
		Size: 4.7 MB (4744099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f90721c8214905e9144d1f98a7d960e786e58f44e95a9cbb5d21154ccb780c9`  
		Last Modified: Wed, 03 Aug 2022 14:18:09 GMT  
		Size: 14.2 MB (14177316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c08027647eb22ecf679815d802601139122ee22138b8e591d5b0ab8fec068de`  
		Last Modified: Wed, 03 Aug 2022 14:18:06 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29afdd13e4761f268c20ff7f4d913391c7256a56e689c366acbcdf1e95ccbc6b`  
		Last Modified: Wed, 03 Aug 2022 14:18:06 GMT  
		Size: 9.8 KB (9751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b6c91acf376235b95d0f445059c7a276d5b645f302737235f7a4342484ff89`  
		Last Modified: Wed, 03 Aug 2022 14:18:06 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0c0bee7d0049340fd26007ddb7a644686e5b43cdda20e2b1a11d0f50ac2d3e`  
		Last Modified: Wed, 03 Aug 2022 14:18:06 GMT  
		Size: 10.7 KB (10727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d033366c675ea1b9f002473fa56ee48c022460ac9ee87cbac592db23ecf82a`  
		Last Modified: Wed, 03 Aug 2022 14:18:06 GMT  
		Size: 2.6 MB (2590466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.3-kernel-java17-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:a0fc89584311c15d01da70315e449b9ec7c434e1b822834298473a534d6b4492
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118998222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd1e6933f514a2ad93c66c4fe7d401196e68e1e2c2f83aa55a574e1961433f21`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 07:16:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 07:18:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:52:39 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Tue, 07 Jun 2022 09:54:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f899948ea0c5dc80a66f801db585939a25a4ae7e1f21a9a8f3bf3749c3baa87f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9c54166490ac55a6bd26249b57eae5df4531635f4871e6642e7979affc894875';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='dad35fec82047e3a82c6e2dda8b53ee763b55aaedaed13b7b130856f4a3ffd35';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='4e2f631ad18c288e419db5c35295829dd7e83f4cd1be95252db06eb622b23090';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 09:54:20 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 09:54:22 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 07 Jun 2022 09:55:03 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 07 Jun 2022 11:31:51 GMT
ARG VERBOSE=false
# Tue, 07 Jun 2022 11:31:54 GMT
ARG OPENJ9_SCC=true
# Tue, 07 Jun 2022 11:50:14 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Tue, 07 Jun 2022 11:50:21 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Tue, 07 Jun 2022 11:50:25 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Tue, 07 Jun 2022 11:50:30 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 07 Jun 2022 11:50:35 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Tue, 07 Jun 2022 11:50:40 GMT
ARG LIBERTY_URL
# Tue, 07 Jun 2022 11:50:44 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 07 Jun 2022 11:51:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 11:51:53 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 11:51:57 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Tue, 07 Jun 2022 11:52:03 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 07 Jun 2022 11:52:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 27 Jun 2022 19:45:56 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Mon, 27 Jun 2022 19:45:58 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 27 Jun 2022 19:46:03 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 27 Jun 2022 19:46:28 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 27 Jun 2022 19:46:33 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Mon, 27 Jun 2022 19:46:37 GMT
USER 1001
# Mon, 27 Jun 2022 19:46:45 GMT
EXPOSE 9080 9443
# Mon, 27 Jun 2022 19:46:49 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 27 Jun 2022 19:46:53 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6c621e52fdf1e59e073b1c51c52e2e5a829be92510ef56949c609a03af2492`  
		Last Modified: Tue, 07 Jun 2022 07:30:19 GMT  
		Size: 17.2 MB (17203633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643e82d1f37eb2778986afcd7aa289e4f42b3c21d19b6dc2b50320f2836d580e`  
		Last Modified: Tue, 07 Jun 2022 10:03:59 GMT  
		Size: 48.1 MB (48115319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe972a29b91980b448bef8b1d66c53f248a582f57eb8476283dad120863f562`  
		Last Modified: Tue, 07 Jun 2022 10:03:52 GMT  
		Size: 3.7 MB (3691417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e5e59f0479d2819daf6bbf7e0092c0fd2870392053bbb1fa626cb335110747`  
		Last Modified: Tue, 07 Jun 2022 13:00:04 GMT  
		Size: 14.2 MB (14177183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf149583f4b3ca4aa8660caf345b205efea81d3fbbe1f4a26eb93122e7266bb`  
		Last Modified: Tue, 07 Jun 2022 12:59:59 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaf4913e1f3802720cdae39cead964ff5e53c908cffb78399ad317ca2ad4668`  
		Last Modified: Mon, 27 Jun 2022 20:25:18 GMT  
		Size: 9.8 KB (9758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb13ac17557dd68458fc2d34c1adfcab23e98b530637ef976a5adbd48f02896b`  
		Last Modified: Mon, 27 Jun 2022 20:25:17 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126f2b45ae77f5dd8e99944b9762f07fdbece5e587c9bc2d67978cea68de0a30`  
		Last Modified: Mon, 27 Jun 2022 20:25:18 GMT  
		Size: 10.7 KB (10745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9839bb93112137f7723692dbf85f749560347702eca16f7a6031270b3f8969b`  
		Last Modified: Mon, 27 Jun 2022 20:25:18 GMT  
		Size: 2.5 MB (2494859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.3-kernel-java17-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:af07f31c93f0eb19792699145364d4f13a91297c5181665177d08f8cb306c004
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110703913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aac5512b088bea2a699f9f716facaad7101b3f8725b948019ee03b0426ed1106`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:41:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 12:41:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:47:17 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Tue, 02 Aug 2022 12:48:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f899948ea0c5dc80a66f801db585939a25a4ae7e1f21a9a8f3bf3749c3baa87f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9c54166490ac55a6bd26249b57eae5df4531635f4871e6642e7979affc894875';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='dad35fec82047e3a82c6e2dda8b53ee763b55aaedaed13b7b130856f4a3ffd35';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='4e2f631ad18c288e419db5c35295829dd7e83f4cd1be95252db06eb622b23090';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 12:48:20 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 12:48:20 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 12:48:53 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 00:31:56 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:31:56 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:58:28 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 03 Aug 2022 00:58:28 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 03 Aug 2022 00:58:29 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 03 Aug 2022 00:58:29 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 00:58:29 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 03 Aug 2022 00:58:29 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 00:58:29 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 00:58:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 00:58:39 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 00:58:39 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 03 Aug 2022 00:58:40 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:58:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 00:58:40 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 00:58:40 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 00:58:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 00:58:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 00:58:47 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 00:58:47 GMT
USER 1001
# Wed, 03 Aug 2022 00:58:47 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 00:58:47 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 00:58:47 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:8366f0be07eee724257935ccff074ac6069837c38e228be50a0b6f2e058ab16c`  
		Last Modified: Tue, 02 Aug 2022 12:54:24 GMT  
		Size: 46.2 MB (46241889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc471632f4e136d4fa45d0a7216573974cc332f3e9fa969846cb74f259e5e9cc`  
		Last Modified: Tue, 02 Aug 2022 12:54:19 GMT  
		Size: 4.9 MB (4939140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de9a36d5fbf5d611bab2200f4f80e76f6c340b3e718fc4833421954bd75e18c`  
		Last Modified: Wed, 03 Aug 2022 01:22:56 GMT  
		Size: 14.2 MB (14177336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d10e4a10caa655f57c14e23a3dc8b9f8cb97e1122630b7d5c1d5ae2350ef70`  
		Last Modified: Wed, 03 Aug 2022 01:22:54 GMT  
		Size: 690.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd0d83f98fb0b32d0d0090042a444c124da512520447d43c6bc9fda6f444cd8`  
		Last Modified: Wed, 03 Aug 2022 01:22:54 GMT  
		Size: 9.8 KB (9755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a16c5a35f7fea6399e22685da0bffd79be7dff2d4903f7a2e10cac53ecf1ce`  
		Last Modified: Wed, 03 Aug 2022 01:22:54 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5d404e1c64ec9327501ac0db62a38586f0184219713589552c3958fd3ef29a`  
		Last Modified: Wed, 03 Aug 2022 01:22:54 GMT  
		Size: 10.7 KB (10733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b82e7c16e18adecba092f08fb55ba338d14c4ee8c6212d03895751bf0e245af`  
		Last Modified: Wed, 03 Aug 2022 01:22:54 GMT  
		Size: 2.5 MB (2548608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.3-kernel-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:7de04727d4f7a26d69b2b551f586b5d9c2aa2194e5b76d6de3c20b77bebaa49d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:22.0.0.3-kernel-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:e11a87d3a4f79183dbb6da6ec7ce7b605f742c665fd71d2382b1f9f05990ce15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.6 MB (178619418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dceed9a173b1d344fac2c79b722f72c94b4f4d6d22ca71fb63b7459c65d083b`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:09:52 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 02 Aug 2022 20:10:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:10:01 GMT
ENV JAVA_VERSION=8.0.7.11
# Tue, 02 Aug 2022 20:10:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 02 Aug 2022 20:10:53 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 03 Aug 2022 13:22:32 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:22:32 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:49:08 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 03 Aug 2022 13:49:08 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 03 Aug 2022 13:49:08 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 03 Aug 2022 13:49:08 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 13:49:09 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 03 Aug 2022 13:49:09 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 13:49:09 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 13:49:22 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 13:49:22 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 13:49:22 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 03 Aug 2022 13:49:22 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:49:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 13:49:23 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 13:49:23 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 13:49:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 13:49:33 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 13:49:33 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 03 Aug 2022 13:49:33 GMT
USER 1001
# Wed, 03 Aug 2022 13:49:33 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 13:49:34 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 13:49:34 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6715a1bb89fcf5e91403be2bc6130f23e6b3cfd0da73e6b09e937d028409d3`  
		Last Modified: Tue, 02 Aug 2022 20:13:24 GMT  
		Size: 3.0 MB (2957815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1607240ca884b25e20b8db8c53c4aea519b76a50e23c19a40aaadd508939589`  
		Last Modified: Tue, 02 Aug 2022 20:13:35 GMT  
		Size: 129.1 MB (129092301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd376116f0255a5936ba040aa80c0f3b34cd853737517b6e1e219336ea6bd67a`  
		Last Modified: Wed, 03 Aug 2022 14:17:48 GMT  
		Size: 14.1 MB (14079596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b756764ec4146955c479f2b9eb2556b60129720dd763fa8b57f5d99952db1ca`  
		Last Modified: Wed, 03 Aug 2022 14:17:45 GMT  
		Size: 686.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122022c189e35d2c9d2ed2b46ef65b13a2555e4ca6af1d5d942d079635f237bd`  
		Last Modified: Wed, 03 Aug 2022 14:17:45 GMT  
		Size: 9.8 KB (9755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2718333544b606e7d11939378d0696fdd34aa77cabf27be95942171c7b3d35c0`  
		Last Modified: Wed, 03 Aug 2022 14:17:45 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a63c196c6194314faa0a14e2ac5d111d8395522b2c03056656c53c7a1a11ff5`  
		Last Modified: Wed, 03 Aug 2022 14:17:45 GMT  
		Size: 10.7 KB (10734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd896b840d88bcfa57c5076c131df6acecf3b451f11be38e30594c6a81e7c0d2`  
		Last Modified: Wed, 03 Aug 2022 14:17:46 GMT  
		Size: 5.8 MB (5757989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.3-kernel-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:1b1d3e5d82168f615c12a295068aed7be7be9d52b143d20824cbfa487720fe73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.9 MB (181912211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007b7cd9472d712013fc0d81e12987280b3970fd263c026db991119ecd81794e`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:49:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 07 Jun 2022 08:50:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 18:31:53 GMT
ENV JAVA_VERSION=8.0.7.11
# Wed, 29 Jun 2022 18:33:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 29 Jun 2022 18:33:35 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 29 Jun 2022 19:03:57 GMT
ARG VERBOSE=false
# Wed, 29 Jun 2022 19:04:05 GMT
ARG OPENJ9_SCC=true
# Wed, 29 Jun 2022 19:20:58 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 29 Jun 2022 19:21:07 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 29 Jun 2022 19:21:10 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 29 Jun 2022 19:21:14 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 29 Jun 2022 19:21:18 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 29 Jun 2022 19:21:22 GMT
ARG LIBERTY_URL
# Wed, 29 Jun 2022 19:21:31 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 29 Jun 2022 19:22:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 19:22:37 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Jun 2022 19:22:40 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 29 Jun 2022 19:22:44 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 29 Jun 2022 19:22:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 29 Jun 2022 19:22:58 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 29 Jun 2022 19:23:01 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 29 Jun 2022 19:23:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 29 Jun 2022 19:23:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 29 Jun 2022 19:23:42 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 29 Jun 2022 19:23:49 GMT
USER 1001
# Wed, 29 Jun 2022 19:23:55 GMT
EXPOSE 9080 9443
# Wed, 29 Jun 2022 19:23:59 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 29 Jun 2022 19:24:04 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4a22aedc3b9f2593635b0a3f6fe64e6dd424850b9782f66e88c8c162926d6a`  
		Last Modified: Tue, 07 Jun 2022 08:54:16 GMT  
		Size: 3.1 MB (3082521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448aed354e59dc01b7da997655c86778001067ef107a5c1fb36a7c38fcf5fdda`  
		Last Modified: Wed, 29 Jun 2022 18:38:02 GMT  
		Size: 128.6 MB (128629743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315aa69ea9848470ad9633185d0c939f3350f1bbc367bd888dcec33016e3d36e`  
		Last Modified: Wed, 29 Jun 2022 19:37:23 GMT  
		Size: 14.4 MB (14407322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9b364212ac3c9cd51f4b4ac71547955228a430e65573ebb26408a3ade7aaf4`  
		Last Modified: Wed, 29 Jun 2022 19:37:18 GMT  
		Size: 680.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe9a429664a923f6fd2cac536b42514ada9fbe2965585093f4ccd98193bbd27`  
		Last Modified: Wed, 29 Jun 2022 19:37:18 GMT  
		Size: 9.8 KB (9758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aded815fcdabc6d10f987c0f48c20e81c39776ab6f05bf562f44e8dcb306551`  
		Last Modified: Wed, 29 Jun 2022 19:37:18 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca4dbddc845e7d48a289b08f7fbd411cf5d2e3f7d335aa3f1238cf6d9cf6b2a`  
		Last Modified: Wed, 29 Jun 2022 19:37:18 GMT  
		Size: 10.7 KB (10740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419732f323d71a8ab58836655c727f3c088fae1bda27617a74fb6b247d0917c2`  
		Last Modified: Wed, 29 Jun 2022 19:37:19 GMT  
		Size: 5.3 MB (5328315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.3-kernel-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:7fb819915e356fbbeb7adad4ae23c91ece3e7b8586d01e4604801871adf04573
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.2 MB (174169493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea5a8defa1d5c4c1ad214f7a403de023fdb2fd5ca2bf7ffba7c4e067ace5696`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:01:57 GMT
ADD file:3d2e9b401524527b395347bc3847be7c9cb465b9a214a1a1d31e74330e293c45 in / 
# Tue, 02 Aug 2022 01:01:58 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 13:19:12 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 02 Aug 2022 13:19:25 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:19:25 GMT
ENV JAVA_VERSION=8.0.7.11
# Tue, 02 Aug 2022 13:20:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 02 Aug 2022 13:20:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 03 Aug 2022 00:30:47 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:30:48 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:57:34 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 03 Aug 2022 00:57:34 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 03 Aug 2022 00:57:34 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 03 Aug 2022 00:57:34 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 00:57:34 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 03 Aug 2022 00:57:34 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 00:57:34 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 00:57:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 00:57:45 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 00:57:45 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 03 Aug 2022 00:57:45 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:57:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 00:57:46 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 00:57:46 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 00:57:47 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 00:57:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 00:57:54 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 03 Aug 2022 00:57:54 GMT
USER 1001
# Wed, 03 Aug 2022 00:57:55 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 00:57:55 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 00:57:55 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:be3ed498266c519f84268ff1f02085fa249c0e32fb60a59466e24c862b5f094b`  
		Last Modified: Tue, 02 Aug 2022 01:03:25 GMT  
		Size: 25.4 MB (25369584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2ed0adcefe11b30e3dff027bcb1cb9fe759f39f50b008bafb3644d3d2fcba8`  
		Last Modified: Tue, 02 Aug 2022 13:22:41 GMT  
		Size: 2.7 MB (2671706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745854ef92308f8e24873e2cf64eb998c725371b7d10ba8318989b37bba26f33`  
		Last Modified: Tue, 02 Aug 2022 13:22:49 GMT  
		Size: 126.1 MB (126143967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974fefeaf21f90e751b044175d4bf9e9d40d602855e046cd5b7275a3c5ec3fb8`  
		Last Modified: Wed, 03 Aug 2022 01:22:40 GMT  
		Size: 14.1 MB (14079782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c9b03efe4042d882baf28dd6693403668d048e2770c3cba94663f44fb58a54`  
		Last Modified: Wed, 03 Aug 2022 01:22:38 GMT  
		Size: 683.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e47b30dd51ef2a8cf86e72c1e2df4374bc8d6c38542199d5c9cc25c983bd630`  
		Last Modified: Wed, 03 Aug 2022 01:22:38 GMT  
		Size: 9.8 KB (9753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3104abd5350f6fb1869fa4a2199bdefa3c7d5b5497212915bbaf38a8ca13a60c`  
		Last Modified: Wed, 03 Aug 2022 01:22:38 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6789e2f9b06fdc267ba249d75c22d4c5cbcd003479b990405cab04d9a97252c1`  
		Last Modified: Wed, 03 Aug 2022 01:22:38 GMT  
		Size: 10.7 KB (10737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b90efb0815342eda22636b96bf2af4b46d9a66cef700fce14817216fbcad375`  
		Last Modified: Wed, 03 Aug 2022 01:22:38 GMT  
		Size: 5.9 MB (5883006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.6-full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:326189db7af92893f0e3b341351f8a334fb5cf93f5735d768529122da6b858e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:22.0.0.6-full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:9b3977be801ee7d384fb934fd6c8c24640b0de518141ee7efa557b280e6f4b40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **394.9 MB (394928920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cdb74cfa2ffeffb22e4d0b330871c4e06e42acb96eb1fb693d45fb5222577d6`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 19:04:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 19:05:01 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 19:56:56 GMT
ENV JAVA_VERSION=jdk-11.0.15+10_openj9-0.32.0
# Tue, 02 Aug 2022 19:58:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69e4a0b383c7b4187478ddb196de3cdc91560e2be40b8ef66354591e87c36e85';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5e82f7df54786c557d2d9e9ac22df655fd94b9702c73261390903ac87532d545';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='25d4d5e2bbe3eb19bcb9a76aec4b43d4eef5ad66200df3122118f69da5325cf6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='def85f1b00e9c65a8c3b5dcf4da0f1b04c17675b4ff9cd6f5dad61d8dcbd03d0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 19:58:02 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 19:58:02 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 19:58:37 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 13:23:06 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:23:06 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:23:06 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 13:23:06 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 13:23:06 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 13:23:06 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 13:23:07 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 13:23:07 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 13:23:07 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 13:23:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 13:23:20 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 13:23:20 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 13:23:20 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:23:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 13:23:21 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 13:23:21 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 13:23:22 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 13:23:29 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 13:23:29 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 13:23:29 GMT
USER 1001
# Wed, 03 Aug 2022 13:23:29 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 13:23:29 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 13:23:29 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 03 Aug 2022 13:32:10 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:32:11 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 03 Aug 2022 13:39:49 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 03 Aug 2022 13:39:51 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 03 Aug 2022 13:40:20 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:a84b3718e4bf43f94609ec6fedf833567945fd97d9b8c324995df295d627fbb7`  
		Last Modified: Tue, 02 Aug 2022 20:06:46 GMT  
		Size: 47.7 MB (47691482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c02c82f8c35f778ae48a325cbccf65292ecbdea6e70272147ca65f72cda4dd`  
		Last Modified: Tue, 02 Aug 2022 20:06:39 GMT  
		Size: 4.2 MB (4183653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f41d289bc930a3a92caf3a90f84db2362a42680dd7ce48a2e1befa89078e3d`  
		Last Modified: Wed, 03 Aug 2022 14:16:04 GMT  
		Size: 14.2 MB (14183927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe3d80467e0f8bbeb61b656c7c4ed7ce644a4d1c7eab501f1b6a0e7fe8375b4`  
		Last Modified: Wed, 03 Aug 2022 14:16:00 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b9afcc7c926f3a529e2ea516fde829c98dbefe91c9d6f6ad3da2566ac205aff`  
		Last Modified: Wed, 03 Aug 2022 14:16:00 GMT  
		Size: 9.8 KB (9754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1691ca21cc220ab5c388a3736a7d146f33ae925532fb1608e128ef9b5d0bae8`  
		Last Modified: Wed, 03 Aug 2022 14:16:00 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a698c8b450bdc7160dc4aec60aec1b5bf12d3eba41cacac8016a21efc396f6`  
		Last Modified: Wed, 03 Aug 2022 14:16:00 GMT  
		Size: 10.7 KB (10731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d3164f01d38ac4bfa365542bbba93799c6f0fdd8ac6a8ae099ff4b510397a5`  
		Last Modified: Wed, 03 Aug 2022 14:16:01 GMT  
		Size: 2.5 MB (2534099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1ab2301875a334deb371209e9dca924755437756da96780092a995e0a1f0c6`  
		Last Modified: Wed, 03 Aug 2022 14:16:59 GMT  
		Size: 267.1 MB (267144880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14816fa7889d9e1162dce8c26791c4f7fdd3205871ffd806993820d0dcf26e59`  
		Last Modified: Wed, 03 Aug 2022 14:16:46 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ff575ec50297731f1e101a1281569273f275b1b37d235d1ef010528a460cdc`  
		Last Modified: Wed, 03 Aug 2022 14:16:48 GMT  
		Size: 14.6 MB (14565953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.6-full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:568ef80bcca1347cbe226376d843073d6a27ba7c43cc818dc85e6d15bf59e28f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.9 MB (399864626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:270f4646bfd8b7ae7175d55df724300751667413afa34555b6d898b0fd2ab212`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 07:16:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 07:18:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:46:26 GMT
ENV JAVA_VERSION=jdk-11.0.15+10_openj9-0.32.0
# Tue, 07 Jun 2022 09:48:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69e4a0b383c7b4187478ddb196de3cdc91560e2be40b8ef66354591e87c36e85';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5e82f7df54786c557d2d9e9ac22df655fd94b9702c73261390903ac87532d545';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='25d4d5e2bbe3eb19bcb9a76aec4b43d4eef5ad66200df3122118f69da5325cf6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='def85f1b00e9c65a8c3b5dcf4da0f1b04c17675b4ff9cd6f5dad61d8dcbd03d0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 09:48:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 09:48:28 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 07 Jun 2022 09:49:12 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 07 Jun 2022 11:28:13 GMT
ARG VERBOSE=false
# Tue, 07 Jun 2022 11:28:23 GMT
ARG OPENJ9_SCC=true
# Mon, 27 Jun 2022 19:05:58 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Mon, 27 Jun 2022 19:06:02 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Mon, 27 Jun 2022 19:06:05 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Mon, 27 Jun 2022 19:06:10 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 27 Jun 2022 19:06:13 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Mon, 27 Jun 2022 19:06:17 GMT
ARG LIBERTY_URL
# Mon, 27 Jun 2022 19:06:22 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 27 Jun 2022 19:07:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 27 Jun 2022 19:07:15 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Jun 2022 19:07:20 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Mon, 27 Jun 2022 19:07:23 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 27 Jun 2022 19:07:30 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 27 Jun 2022 19:07:32 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Mon, 27 Jun 2022 19:07:33 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 27 Jun 2022 19:07:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 27 Jun 2022 19:07:55 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 27 Jun 2022 19:07:57 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Mon, 27 Jun 2022 19:08:01 GMT
USER 1001
# Mon, 27 Jun 2022 19:08:05 GMT
EXPOSE 9080 9443
# Mon, 27 Jun 2022 19:08:08 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 27 Jun 2022 19:08:10 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Mon, 27 Jun 2022 19:20:56 GMT
ARG VERBOSE=false
# Mon, 27 Jun 2022 19:20:59 GMT
ARG REPOSITORIES_PROPERTIES=
# Mon, 27 Jun 2022 19:30:13 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Mon, 27 Jun 2022 19:30:26 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Mon, 27 Jun 2022 19:31:35 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6c621e52fdf1e59e073b1c51c52e2e5a829be92510ef56949c609a03af2492`  
		Last Modified: Tue, 07 Jun 2022 07:30:19 GMT  
		Size: 17.2 MB (17203633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06eb9350ab17a87b8e47ac6a3389da7e21786ee038077cf7b627f90b125f1acf`  
		Last Modified: Tue, 07 Jun 2022 10:01:58 GMT  
		Size: 48.4 MB (48378487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc0d65d22cb0b40edcecacc4b8c684bc4bf1ddc89b24fd16e7abefba2b0c7df`  
		Last Modified: Tue, 07 Jun 2022 10:01:49 GMT  
		Size: 3.3 MB (3334009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5ff26c4cf89eaa05313a18d91d7309df617938eb84d02061347a609a33a7b8`  
		Last Modified: Mon, 27 Jun 2022 20:21:41 GMT  
		Size: 14.5 MB (14515853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ccfddb3da6a003c78fba8f80fd75c65f4fc295e3cc5bdf38bacf9e33c4844f`  
		Last Modified: Mon, 27 Jun 2022 20:21:32 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e827be780b6a43a9e9798fec11910f661a036eb43e9b207bd5a09dc0931e9b`  
		Last Modified: Mon, 27 Jun 2022 20:21:32 GMT  
		Size: 9.8 KB (9751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79a0d64d22b6a5861752d66f9cef744682bef6f31b78ac467d9065fadc0587c`  
		Last Modified: Mon, 27 Jun 2022 20:21:32 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93afd12b58a928c66cb4067a1a977a97bc0dacfe201dc9ad79c4800176e8cca`  
		Last Modified: Mon, 27 Jun 2022 20:21:32 GMT  
		Size: 10.7 KB (10734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210f9edeb69d5d47378b5b0de8220cb51a99548682efd824bb4fc5dce63089c3`  
		Last Modified: Mon, 27 Jun 2022 20:21:33 GMT  
		Size: 2.5 MB (2522136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610e5d1cf0778b270585e8c568433ebe0d1721c289aef87a4e33139fbfc8be22`  
		Last Modified: Mon, 27 Jun 2022 20:23:50 GMT  
		Size: 267.1 MB (267145041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823da95363ffd3cef0df423c707c5741e0e46d33a1211239731e7020f132c98b`  
		Last Modified: Mon, 27 Jun 2022 20:23:27 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a806cb8e7c52d02a647b832925c7dd227d390e06af95aa5ca784a9e3e796a7`  
		Last Modified: Mon, 27 Jun 2022 20:23:30 GMT  
		Size: 13.4 MB (13448725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.6-full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:30360124bffc5d586450ed00757b3da2b07527fdd14f607522e7113a68c4d6c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.3 MB (392311995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6380aa33c3d2bf9aa3cda4cb99b404ff94433d361c0026bcd2d70911bf9fc2fa`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:41:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 12:41:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:43:42 GMT
ENV JAVA_VERSION=jdk-11.0.15+10_openj9-0.32.0
# Tue, 02 Aug 2022 12:44:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69e4a0b383c7b4187478ddb196de3cdc91560e2be40b8ef66354591e87c36e85';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5e82f7df54786c557d2d9e9ac22df655fd94b9702c73261390903ac87532d545';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='25d4d5e2bbe3eb19bcb9a76aec4b43d4eef5ad66200df3122118f69da5325cf6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='def85f1b00e9c65a8c3b5dcf4da0f1b04c17675b4ff9cd6f5dad61d8dcbd03d0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 12:44:51 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 12:44:51 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 12:45:24 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 00:31:25 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:31:25 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:31:25 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 00:31:25 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 00:31:25 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 00:31:26 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 00:31:26 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 00:31:26 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 00:31:26 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 00:31:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 00:31:38 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 00:31:38 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 00:31:38 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:31:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 00:31:39 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 00:31:39 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 00:31:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 00:31:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 00:31:46 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 00:31:46 GMT
USER 1001
# Wed, 03 Aug 2022 00:31:47 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 00:31:47 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 00:31:47 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 03 Aug 2022 00:40:52 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:40:53 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 03 Aug 2022 00:48:29 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 03 Aug 2022 00:48:41 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 03 Aug 2022 00:49:06 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:3f28b38375577480d13a8d78bab4c30073086c8a51a4ff217f32365aa0847411`  
		Last Modified: Tue, 02 Aug 2022 12:53:12 GMT  
		Size: 46.7 MB (46721680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3142744ed0637685528da62bbcb28da17d0b48fdc151bd52e7b22274eeb2c5da`  
		Last Modified: Tue, 02 Aug 2022 12:53:07 GMT  
		Size: 4.3 MB (4313565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9e7b387efd480990d6c64a866fba64fb104280672f530db487652f6a8b2420`  
		Last Modified: Wed, 03 Aug 2022 01:21:19 GMT  
		Size: 14.2 MB (14184080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d846195251009f85f9e3322ee32d4f6714c2208a979e2878e07e74634075b2`  
		Last Modified: Wed, 03 Aug 2022 01:21:17 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a4da3cc546eda0832bbac5eea20e393ef5335b890a0401290b55655e909ae4`  
		Last Modified: Wed, 03 Aug 2022 01:21:17 GMT  
		Size: 9.8 KB (9753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc9ec89f07bd2ea2472397191fdaf70131a284380baa496449e81346c8f9e97`  
		Last Modified: Wed, 03 Aug 2022 01:21:17 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6edb8309c1fef9cc240f64d15d2875b926152ce9f44aa1e3a2fa26b7eacecb`  
		Last Modified: Wed, 03 Aug 2022 01:21:16 GMT  
		Size: 10.7 KB (10726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c61c79763634b9154ab44813cd5f16fac38e3a947bc0e0a208f3468ae4c3910`  
		Last Modified: Wed, 03 Aug 2022 01:21:18 GMT  
		Size: 2.5 MB (2549406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc0bd9df0380ed2d04e74a81ae642853add021ebef188564b042d142d7b5faa`  
		Last Modified: Wed, 03 Aug 2022 01:22:02 GMT  
		Size: 267.1 MB (267143265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e189831428d2706995b316dcfcdb2f9dbde838fbd1a188ac5d869aaf028d1f4a`  
		Last Modified: Wed, 03 Aug 2022 01:21:51 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557ad0e62e6ef6a383af9d2f91a0b9d5fc0ebefdbd530332b73d31367e3ac446`  
		Last Modified: Wed, 03 Aug 2022 01:21:52 GMT  
		Size: 14.6 MB (14602122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.6-full-java17-openj9`

```console
$ docker pull websphere-liberty@sha256:34362463fcb358b55f026fefe7cc6e114bcfe9508795a4d11d4487d090c2a389
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:22.0.0.6-full-java17-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:8337943a15d51cb83b3b793640a07bd4e5fcba7e5416ce631c2ff0aefee030c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (396008706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0c46e520aae2f1050803a9fb2df6a5a9a897d207ae26a4449a0faea6499711e`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 19:04:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 19:05:01 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:00:47 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Tue, 02 Aug 2022 20:02:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f899948ea0c5dc80a66f801db585939a25a4ae7e1f21a9a8f3bf3749c3baa87f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9c54166490ac55a6bd26249b57eae5df4531635f4871e6642e7979affc894875';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='dad35fec82047e3a82c6e2dda8b53ee763b55aaedaed13b7b130856f4a3ffd35';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='4e2f631ad18c288e419db5c35295829dd7e83f4cd1be95252db06eb622b23090';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 20:02:05 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 20:02:05 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 20:02:40 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 13:23:34 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:23:34 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:23:34 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 13:23:34 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 13:23:35 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 13:23:35 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 13:23:35 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 13:23:35 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 13:23:35 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 13:23:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 13:23:48 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 13:23:48 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 13:23:48 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:23:49 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 13:23:49 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 13:23:49 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 13:23:50 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 13:23:57 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 13:23:57 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 13:23:57 GMT
USER 1001
# Wed, 03 Aug 2022 13:23:57 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 13:23:58 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 13:23:58 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 03 Aug 2022 13:40:34 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:40:34 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 03 Aug 2022 13:48:12 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 03 Aug 2022 13:48:14 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 03 Aug 2022 13:48:44 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:7b6279e9931cb0efc3b60659be8fd46c95156f958f00818850fba3ac0ecd0616`  
		Last Modified: Tue, 02 Aug 2022 20:08:11 GMT  
		Size: 47.8 MB (47754438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e834be70bdf636e5c875d9e2badbf281d32ff675b9eb7db8768a2da9dbdf5e`  
		Last Modified: Tue, 02 Aug 2022 20:08:05 GMT  
		Size: 4.7 MB (4744099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b29111272e76b623f6a1c705052b79e4aed2ed08bb404f433fd8a20cd7c752`  
		Last Modified: Wed, 03 Aug 2022 14:16:14 GMT  
		Size: 14.2 MB (14183924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6606826ea4776a63f20adb28aca4a26e64d000ea040af34471de8c2366784452`  
		Last Modified: Wed, 03 Aug 2022 14:16:11 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa6ada95f6df02ffacedde72e53786a3bc150cc4bf94f7861f91a2cb9e026b0`  
		Last Modified: Wed, 03 Aug 2022 14:16:11 GMT  
		Size: 9.7 KB (9749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9521245474cad0537df9cfe305a8f740cb08a15941eea9bbd4b6d48ca6f91cd7`  
		Last Modified: Wed, 03 Aug 2022 14:16:11 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3f9ef840580663cf3012d2a8a7d7b03dab23484c4e62f2eba0004d6f4adaa`  
		Last Modified: Wed, 03 Aug 2022 14:16:11 GMT  
		Size: 10.7 KB (10725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f946b913fac313fce2c6d202c5ea9c9da8039c23dda2c638d1035e62305bc81`  
		Last Modified: Wed, 03 Aug 2022 14:16:11 GMT  
		Size: 2.5 MB (2549516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d00dd2ab51ffc9eeabfa9eca2f588e9cb53c5fc4ba3ef2021fb3f12e357f19`  
		Last Modified: Wed, 03 Aug 2022 14:17:20 GMT  
		Size: 267.1 MB (267144532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b633affe3bbc937124f9773be4f737c55d2f47a37f2308dbfb0a7199110753`  
		Last Modified: Wed, 03 Aug 2022 14:17:06 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a02c200927d909642073247ea75742a772e35a2e308cb01aa2ab9a5f81f82d`  
		Last Modified: Wed, 03 Aug 2022 14:17:08 GMT  
		Size: 15.0 MB (15007284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.6-full-java17-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:d2b38cf5aeaf7df489e9b960daf12f80ff3351af7cb88d0f598dfe388b1cc414
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.3 MB (399269706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce1658e884c9121f94bdddfa7883b8ca0797266dc1a09218a559585fe3960aef`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 07:16:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 07:18:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:52:39 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Tue, 07 Jun 2022 09:54:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f899948ea0c5dc80a66f801db585939a25a4ae7e1f21a9a8f3bf3749c3baa87f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9c54166490ac55a6bd26249b57eae5df4531635f4871e6642e7979affc894875';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='dad35fec82047e3a82c6e2dda8b53ee763b55aaedaed13b7b130856f4a3ffd35';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='4e2f631ad18c288e419db5c35295829dd7e83f4cd1be95252db06eb622b23090';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 09:54:20 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 09:54:22 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 07 Jun 2022 09:55:03 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 07 Jun 2022 11:31:51 GMT
ARG VERBOSE=false
# Tue, 07 Jun 2022 11:31:54 GMT
ARG OPENJ9_SCC=true
# Mon, 27 Jun 2022 19:08:20 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Mon, 27 Jun 2022 19:08:23 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Mon, 27 Jun 2022 19:08:26 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Mon, 27 Jun 2022 19:08:29 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 27 Jun 2022 19:08:32 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Mon, 27 Jun 2022 19:08:33 GMT
ARG LIBERTY_URL
# Mon, 27 Jun 2022 19:08:37 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 27 Jun 2022 19:09:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 27 Jun 2022 19:09:29 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Jun 2022 19:09:31 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Mon, 27 Jun 2022 19:09:32 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 27 Jun 2022 19:09:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 27 Jun 2022 19:09:42 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Mon, 27 Jun 2022 19:09:43 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 27 Jun 2022 19:09:52 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 27 Jun 2022 19:10:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 27 Jun 2022 19:10:11 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Mon, 27 Jun 2022 19:10:14 GMT
USER 1001
# Mon, 27 Jun 2022 19:10:17 GMT
EXPOSE 9080 9443
# Mon, 27 Jun 2022 19:10:18 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 27 Jun 2022 19:10:23 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Mon, 27 Jun 2022 19:31:54 GMT
ARG VERBOSE=false
# Mon, 27 Jun 2022 19:31:58 GMT
ARG REPOSITORIES_PROPERTIES=
# Mon, 27 Jun 2022 19:41:31 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Mon, 27 Jun 2022 19:41:38 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Mon, 27 Jun 2022 19:42:34 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6c621e52fdf1e59e073b1c51c52e2e5a829be92510ef56949c609a03af2492`  
		Last Modified: Tue, 07 Jun 2022 07:30:19 GMT  
		Size: 17.2 MB (17203633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643e82d1f37eb2778986afcd7aa289e4f42b3c21d19b6dc2b50320f2836d580e`  
		Last Modified: Tue, 07 Jun 2022 10:03:59 GMT  
		Size: 48.1 MB (48115319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe972a29b91980b448bef8b1d66c53f248a582f57eb8476283dad120863f562`  
		Last Modified: Tue, 07 Jun 2022 10:03:52 GMT  
		Size: 3.7 MB (3691417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c056cb98358395a411cf5384fbbdbec5ccfd5f81859801ac0c85148bbb98a4`  
		Last Modified: Mon, 27 Jun 2022 20:22:00 GMT  
		Size: 14.5 MB (14515851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd06b09fbbdc503b03e823a42d86309633c6d84767fa73330825bc907e14df3`  
		Last Modified: Mon, 27 Jun 2022 20:21:51 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbb19c1ede5ad19ca10791cc60a2f22dd80c54475f408a0e73abdccbca16792`  
		Last Modified: Mon, 27 Jun 2022 20:21:51 GMT  
		Size: 9.8 KB (9753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948cca84307d534dd3b66a3ccd42411c24283967d6c73d87983819647f564e0c`  
		Last Modified: Mon, 27 Jun 2022 20:21:51 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39dcdc56c341ef84605200c2bc492ee7ebd2d7d6c088f9188b4b724f2316504`  
		Last Modified: Mon, 27 Jun 2022 20:21:51 GMT  
		Size: 10.7 KB (10740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdde75f3ce0ceab51ecdf4a88f513912d5744afccff705acaa98d4d96a9399d1`  
		Last Modified: Mon, 27 Jun 2022 20:21:52 GMT  
		Size: 2.5 MB (2524189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70d3a471d83cfe5ea6fb0e3494c7237e036a1b239cdd198d683ced84e37b6b8`  
		Last Modified: Mon, 27 Jun 2022 20:24:24 GMT  
		Size: 267.1 MB (267144514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cd749118a548d29d9d565402d900fd0e6cf95d4f72a07133d3adf7cd3c4b29`  
		Last Modified: Mon, 27 Jun 2022 20:24:00 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca0169250169b2ddc110e2a4d47306077c03fc3040d77c4d134e177924a5193`  
		Last Modified: Mon, 27 Jun 2022 20:24:03 GMT  
		Size: 12.8 MB (12758043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.6-full-java17-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:f69a28b7536236c0a60225c9f8f051862dc9a5e3f7cddcc3765ad686052fc9a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.7 MB (392657062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9618452d33ff355bf5b087737ad9ac477c3db4bc630c4a75304cbb38ca5142da`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:41:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 12:41:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:47:17 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Tue, 02 Aug 2022 12:48:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f899948ea0c5dc80a66f801db585939a25a4ae7e1f21a9a8f3bf3749c3baa87f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9c54166490ac55a6bd26249b57eae5df4531635f4871e6642e7979affc894875';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='dad35fec82047e3a82c6e2dda8b53ee763b55aaedaed13b7b130856f4a3ffd35';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='4e2f631ad18c288e419db5c35295829dd7e83f4cd1be95252db06eb622b23090';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 12:48:20 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 12:48:20 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 12:48:53 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 00:31:56 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:31:56 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:31:56 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 00:31:57 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 00:31:57 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 00:31:57 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 00:31:57 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 00:31:57 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 00:31:57 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 00:32:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 00:32:08 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 00:32:08 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 00:32:08 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:32:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 00:32:09 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 00:32:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 00:32:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 00:32:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 00:32:16 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 00:32:16 GMT
USER 1001
# Wed, 03 Aug 2022 00:32:16 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 00:32:17 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 00:32:17 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 03 Aug 2022 00:49:19 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:49:19 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 03 Aug 2022 00:56:16 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 03 Aug 2022 00:56:21 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 03 Aug 2022 00:56:46 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:8366f0be07eee724257935ccff074ac6069837c38e228be50a0b6f2e058ab16c`  
		Last Modified: Tue, 02 Aug 2022 12:54:24 GMT  
		Size: 46.2 MB (46241889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc471632f4e136d4fa45d0a7216573974cc332f3e9fa969846cb74f259e5e9cc`  
		Last Modified: Tue, 02 Aug 2022 12:54:19 GMT  
		Size: 4.9 MB (4939140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88edf1255c796274783dd2b408dda42ea663cad4b64810259c6acc1259419aa0`  
		Last Modified: Wed, 03 Aug 2022 01:21:26 GMT  
		Size: 14.2 MB (14184036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353a76e46cfbb610eda04921de105adf89120c8930d1974118798f627627b68b`  
		Last Modified: Wed, 03 Aug 2022 01:21:24 GMT  
		Size: 688.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfabfad0e607d1360481e4e76a8538189f1d761829c85652481cc8110f7abd2`  
		Last Modified: Wed, 03 Aug 2022 01:21:24 GMT  
		Size: 9.8 KB (9755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1851082a958effaac3cac4eddcea238e723fb008a9460dc32982226790cf22`  
		Last Modified: Wed, 03 Aug 2022 01:21:24 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3260426547d5393a73a84720e7ff09a76a39680394581d9c50107cb7f6f2489f`  
		Last Modified: Wed, 03 Aug 2022 01:21:24 GMT  
		Size: 10.7 KB (10734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fef24753132b515d30c6966531a9a4e35f7b4cc2441ecbe77dcaf61055f2ce0`  
		Last Modified: Wed, 03 Aug 2022 01:21:25 GMT  
		Size: 2.6 MB (2582268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8976d85227f2d0aba5790a1cea3c5acf86bbae43c589ad3f20b2a7c21dd101b`  
		Last Modified: Wed, 03 Aug 2022 01:22:19 GMT  
		Size: 267.1 MB (267143376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5168ad06a92f4ca58fcdb0144b2c1921376af9657fcaf25b6a85d25b2af1732c`  
		Last Modified: Wed, 03 Aug 2022 01:22:07 GMT  
		Size: 941.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afc1985dd70a701d3ee6a9b6ffcbc88686fe3d09ccc6811624d5c32a95d69e7`  
		Last Modified: Wed, 03 Aug 2022 01:22:09 GMT  
		Size: 14.8 MB (14768472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.6-full-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:3a27bdeb56129c14e7bd4a664be6774a78b910e3d5203d585e55a23137c7c009
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:22.0.0.6-full-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:886abf89eb3316d1fa1e344b1c566b12c8c56dbdfe67ef1ab450f516026e19ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **461.9 MB (461889376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90501b5e0a18925bbd8d499cd561137878b9b24d6b69dcb7f15f4ad327d68c64`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:09:52 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 02 Aug 2022 20:10:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:10:01 GMT
ENV JAVA_VERSION=8.0.7.11
# Tue, 02 Aug 2022 20:10:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 02 Aug 2022 20:10:53 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 03 Aug 2022 13:22:32 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:22:32 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:22:32 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 13:22:33 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 13:22:33 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 13:22:33 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 13:22:33 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 13:22:33 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 13:22:33 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 13:22:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 13:22:51 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 13:22:51 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 13:22:51 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:22:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 13:22:53 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 13:22:53 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 13:22:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 13:23:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 13:23:02 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 03 Aug 2022 13:23:03 GMT
USER 1001
# Wed, 03 Aug 2022 13:23:03 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 13:23:03 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 13:23:03 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 03 Aug 2022 13:24:02 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:24:02 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 03 Aug 2022 13:31:35 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 03 Aug 2022 13:31:36 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 03 Aug 2022 13:32:07 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6715a1bb89fcf5e91403be2bc6130f23e6b3cfd0da73e6b09e937d028409d3`  
		Last Modified: Tue, 02 Aug 2022 20:13:24 GMT  
		Size: 3.0 MB (2957815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1607240ca884b25e20b8db8c53c4aea519b76a50e23c19a40aaadd508939589`  
		Last Modified: Tue, 02 Aug 2022 20:13:35 GMT  
		Size: 129.1 MB (129092301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb38c444df15407ab436886281e04c48950509ec0de9d9bc5203e14640165ddb`  
		Last Modified: Wed, 03 Aug 2022 14:15:54 GMT  
		Size: 14.1 MB (14085453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05aa53415f32b814deebc075a7bb595df58d79cf67a5fe218c1cd111e5b6ee0a`  
		Last Modified: Wed, 03 Aug 2022 14:15:50 GMT  
		Size: 679.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ddbf21b719f1a92ad3ee2ffed35afb7f2c0836d372a03e8ef6c86bc5546c4a`  
		Last Modified: Wed, 03 Aug 2022 14:15:50 GMT  
		Size: 9.8 KB (9757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5492e88c0d013bf0d79353e5c81b4167fe2b1aa74465b5c05edbf3b14658858a`  
		Last Modified: Wed, 03 Aug 2022 14:15:50 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f086c2ef5ce4893aeade47c11c788a8992b4e43bfa5e8316e9a13a422acb4b06`  
		Last Modified: Wed, 03 Aug 2022 14:15:50 GMT  
		Size: 10.7 KB (10735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3191d937acd525f20b08c085e17bb91eb22cf727d6199fd8049c53e3332a232`  
		Last Modified: Wed, 03 Aug 2022 14:15:51 GMT  
		Size: 5.7 MB (5702881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17cdf033149a3de277684874263c1eb2bedf5f30eb0a4012432b12def4c7822`  
		Last Modified: Wed, 03 Aug 2022 14:16:36 GMT  
		Size: 267.1 MB (267144319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10376ddb37d6232ae5252c9bdf6f04422f9557849cd611df7d58c8bf1185eede`  
		Last Modified: Wed, 03 Aug 2022 14:16:21 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5c901d7e4747e67d324ddb82affbf24e080a953b3ce5ed31ad1504258d171a`  
		Last Modified: Wed, 03 Aug 2022 14:16:24 GMT  
		Size: 16.2 MB (16173947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.6-full-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:20b8c8568ac1ace5302e32de4580705070ad867b1267fc10eddecc0342efb233
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.1 MB (463103256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24bec26d5b6e33bfa1465f31c5486fb46d341b64a8a89ebecee746a78fd2086b`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:49:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 07 Jun 2022 08:50:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 18:31:53 GMT
ENV JAVA_VERSION=8.0.7.11
# Wed, 29 Jun 2022 18:33:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 29 Jun 2022 18:33:35 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 29 Jun 2022 19:03:57 GMT
ARG VERBOSE=false
# Wed, 29 Jun 2022 19:04:05 GMT
ARG OPENJ9_SCC=true
# Wed, 29 Jun 2022 19:04:16 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 29 Jun 2022 19:04:32 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 29 Jun 2022 19:04:39 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 29 Jun 2022 19:04:46 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 29 Jun 2022 19:04:53 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 29 Jun 2022 19:04:57 GMT
ARG LIBERTY_URL
# Wed, 29 Jun 2022 19:05:02 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 29 Jun 2022 19:06:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 19:06:54 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Jun 2022 19:06:59 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 29 Jun 2022 19:07:04 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 29 Jun 2022 19:07:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 29 Jun 2022 19:07:22 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 29 Jun 2022 19:07:27 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 29 Jun 2022 19:07:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 29 Jun 2022 19:08:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 29 Jun 2022 19:08:16 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 29 Jun 2022 19:08:20 GMT
USER 1001
# Wed, 29 Jun 2022 19:08:28 GMT
EXPOSE 9080 9443
# Wed, 29 Jun 2022 19:08:35 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 29 Jun 2022 19:08:44 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 29 Jun 2022 19:09:19 GMT
ARG VERBOSE=false
# Wed, 29 Jun 2022 19:09:27 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 29 Jun 2022 19:18:40 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 29 Jun 2022 19:18:47 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 29 Jun 2022 19:19:57 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4a22aedc3b9f2593635b0a3f6fe64e6dd424850b9782f66e88c8c162926d6a`  
		Last Modified: Tue, 07 Jun 2022 08:54:16 GMT  
		Size: 3.1 MB (3082521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448aed354e59dc01b7da997655c86778001067ef107a5c1fb36a7c38fcf5fdda`  
		Last Modified: Wed, 29 Jun 2022 18:38:02 GMT  
		Size: 128.6 MB (128629743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ee64dfa956bec7a3911c4fbcec85677da5eb3557fdd1fad0cd05371b418ed3`  
		Last Modified: Wed, 29 Jun 2022 19:36:18 GMT  
		Size: 14.4 MB (14414087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f44198605bccf1a3fd327e2929165c362826698ef117c8ed5e5f61cf8471cce`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 685.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8008efd74eeabae4093e325cb3ee9f17c49e27f7dbb19564636c92acb9051471`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 9.8 KB (9757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df8e4e4d330f9771962db9ea9c4da8f370e92f1745f117e9db5baae643dfff3`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa888647a678f768a7a68d44ee29bc98b5834e1d4b43481f1d79fb22ae798d8`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 10.7 KB (10748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24233765490b95aea52162ad51e9982a4c6bd67895d93467ca629ea8bfb5a68`  
		Last Modified: Wed, 29 Jun 2022 19:36:15 GMT  
		Size: 5.3 MB (5337804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a597fe1c695442d024092e9ba428ea88ffa886c912a199fbe492b776a53a7595`  
		Last Modified: Wed, 29 Jun 2022 19:36:52 GMT  
		Size: 267.1 MB (267144840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165a7c33a3339f487205b064950b8fb81222d47d74c6fdfef158d7464150dbbb`  
		Last Modified: Wed, 29 Jun 2022 19:36:29 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ede9c741b2ef54fc67a38aab455cdc0ef8bea790cfdf300b7e1d01aa4486ec`  
		Last Modified: Wed, 29 Jun 2022 19:36:35 GMT  
		Size: 14.0 MB (14028991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.6-full-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:f6b028efccb8a1d3a8e7633ab097afc5ef7ea9eb145ecff4d148ebf489240309
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **457.5 MB (457473936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52b2b35b4ae3c6168a008c1dd5dccb115e7bc94a70e161ac19b8340a87a722b7`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:01:57 GMT
ADD file:3d2e9b401524527b395347bc3847be7c9cb465b9a214a1a1d31e74330e293c45 in / 
# Tue, 02 Aug 2022 01:01:58 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 13:19:12 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 02 Aug 2022 13:19:25 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:19:25 GMT
ENV JAVA_VERSION=8.0.7.11
# Tue, 02 Aug 2022 13:20:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 02 Aug 2022 13:20:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 03 Aug 2022 00:30:47 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:30:48 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:30:48 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 00:30:48 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 00:30:48 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 00:30:49 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 00:30:49 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 00:30:49 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 00:30:49 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 00:31:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 00:31:03 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 00:31:03 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 00:31:03 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:31:06 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 00:31:07 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 00:31:07 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 00:31:08 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 00:31:17 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 00:31:18 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 03 Aug 2022 00:31:18 GMT
USER 1001
# Wed, 03 Aug 2022 00:31:18 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 00:31:18 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 00:31:19 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 03 Aug 2022 00:32:24 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:32:24 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 03 Aug 2022 00:39:41 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 03 Aug 2022 00:40:02 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 03 Aug 2022 00:40:42 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:be3ed498266c519f84268ff1f02085fa249c0e32fb60a59466e24c862b5f094b`  
		Last Modified: Tue, 02 Aug 2022 01:03:25 GMT  
		Size: 25.4 MB (25369584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2ed0adcefe11b30e3dff027bcb1cb9fe759f39f50b008bafb3644d3d2fcba8`  
		Last Modified: Tue, 02 Aug 2022 13:22:41 GMT  
		Size: 2.7 MB (2671706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745854ef92308f8e24873e2cf64eb998c725371b7d10ba8318989b37bba26f33`  
		Last Modified: Tue, 02 Aug 2022 13:22:49 GMT  
		Size: 126.1 MB (126143967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a59a661cbbb2b8555a22d1f6e2943fbf1eaa8381c6a30030ac4c3276c7cf1e8`  
		Last Modified: Wed, 03 Aug 2022 01:21:11 GMT  
		Size: 14.1 MB (14085532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19a28dc7880331492105ef80fe1628f9d15c71bc959cd9765cdcd64a139c472`  
		Last Modified: Wed, 03 Aug 2022 01:21:09 GMT  
		Size: 679.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc961a105d81f315d8af16fb228d90842f45dd9ff3a0ce06580d31bf5ae346c3`  
		Last Modified: Wed, 03 Aug 2022 01:21:09 GMT  
		Size: 9.8 KB (9763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07467c7f0c1b48d655b4ff47a1a5101cb4f28e77adce3d47f9c5bfaaaa1968a7`  
		Last Modified: Wed, 03 Aug 2022 01:21:08 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55abb9ff522a8f086c734b47a7b69b3d2770c58ec832b8d992f7e67766700ca8`  
		Last Modified: Wed, 03 Aug 2022 01:21:09 GMT  
		Size: 10.7 KB (10735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4009dc9f786bc5ce10ba8ebf96892fd74d20c3548ff8acc69160e27dcb3a615`  
		Last Modified: Wed, 03 Aug 2022 01:21:09 GMT  
		Size: 5.9 MB (5889501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e27310727e03cbd34d78cf4d4b95a8e316a4b322be112db401ab8c19e495739`  
		Last Modified: Wed, 03 Aug 2022 01:21:43 GMT  
		Size: 267.1 MB (267143557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7fa949e35b734374f99454dc3a7a9f7dba0a28dd865c7ca9514f169950d991`  
		Last Modified: Wed, 03 Aug 2022 01:21:31 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3f51986dc9d010c1551d1d44b8efb475ea65824d2ae8e3fba9476278e13ff0`  
		Last Modified: Wed, 03 Aug 2022 01:21:33 GMT  
		Size: 16.1 MB (16147687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.6-kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:be2eae562c627321465756db2cb0fdaa4730028432e4a05f0c8c46ca32edfd8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:22.0.0.6-kernel-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:236bd357c37f0f21b7adff989a4dab6e6aadd5af1780f2e5b9f5ef684d159d28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113217145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:519b9356f1ab3952e988d47b506fd3a838137be4c4b0a6c9539a7f7c969c91e9`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 19:04:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 19:05:01 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 19:56:56 GMT
ENV JAVA_VERSION=jdk-11.0.15+10_openj9-0.32.0
# Tue, 02 Aug 2022 19:58:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69e4a0b383c7b4187478ddb196de3cdc91560e2be40b8ef66354591e87c36e85';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5e82f7df54786c557d2d9e9ac22df655fd94b9702c73261390903ac87532d545';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='25d4d5e2bbe3eb19bcb9a76aec4b43d4eef5ad66200df3122118f69da5325cf6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='def85f1b00e9c65a8c3b5dcf4da0f1b04c17675b4ff9cd6f5dad61d8dcbd03d0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 19:58:02 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 19:58:02 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 19:58:37 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 13:23:06 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:23:06 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:23:06 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 13:23:06 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 13:23:06 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 13:23:06 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 13:23:07 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 13:23:07 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 13:23:07 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 13:23:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 13:23:20 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 13:23:20 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 13:23:20 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:23:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 13:23:21 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 13:23:21 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 13:23:22 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 13:23:29 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 13:23:29 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 13:23:29 GMT
USER 1001
# Wed, 03 Aug 2022 13:23:29 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 13:23:29 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 13:23:29 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:a84b3718e4bf43f94609ec6fedf833567945fd97d9b8c324995df295d627fbb7`  
		Last Modified: Tue, 02 Aug 2022 20:06:46 GMT  
		Size: 47.7 MB (47691482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c02c82f8c35f778ae48a325cbccf65292ecbdea6e70272147ca65f72cda4dd`  
		Last Modified: Tue, 02 Aug 2022 20:06:39 GMT  
		Size: 4.2 MB (4183653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f41d289bc930a3a92caf3a90f84db2362a42680dd7ce48a2e1befa89078e3d`  
		Last Modified: Wed, 03 Aug 2022 14:16:04 GMT  
		Size: 14.2 MB (14183927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe3d80467e0f8bbeb61b656c7c4ed7ce644a4d1c7eab501f1b6a0e7fe8375b4`  
		Last Modified: Wed, 03 Aug 2022 14:16:00 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b9afcc7c926f3a529e2ea516fde829c98dbefe91c9d6f6ad3da2566ac205aff`  
		Last Modified: Wed, 03 Aug 2022 14:16:00 GMT  
		Size: 9.8 KB (9754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1691ca21cc220ab5c388a3736a7d146f33ae925532fb1608e128ef9b5d0bae8`  
		Last Modified: Wed, 03 Aug 2022 14:16:00 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a698c8b450bdc7160dc4aec60aec1b5bf12d3eba41cacac8016a21efc396f6`  
		Last Modified: Wed, 03 Aug 2022 14:16:00 GMT  
		Size: 10.7 KB (10731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d3164f01d38ac4bfa365542bbba93799c6f0fdd8ac6a8ae099ff4b510397a5`  
		Last Modified: Wed, 03 Aug 2022 14:16:01 GMT  
		Size: 2.5 MB (2534099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.6-kernel-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:6d35cf4b76f82fa41cd99fb78d6adbc77fd06a4a15bb2873d7a9a71ae50836cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.3 MB (119269912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a92fab9e70bea7e1a9541da717f0c50e9fd2ce6e1f66b833f8daf8666f38fdc`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 07:16:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 07:18:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:46:26 GMT
ENV JAVA_VERSION=jdk-11.0.15+10_openj9-0.32.0
# Tue, 07 Jun 2022 09:48:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69e4a0b383c7b4187478ddb196de3cdc91560e2be40b8ef66354591e87c36e85';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5e82f7df54786c557d2d9e9ac22df655fd94b9702c73261390903ac87532d545';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='25d4d5e2bbe3eb19bcb9a76aec4b43d4eef5ad66200df3122118f69da5325cf6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='def85f1b00e9c65a8c3b5dcf4da0f1b04c17675b4ff9cd6f5dad61d8dcbd03d0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 09:48:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 09:48:28 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 07 Jun 2022 09:49:12 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 07 Jun 2022 11:28:13 GMT
ARG VERBOSE=false
# Tue, 07 Jun 2022 11:28:23 GMT
ARG OPENJ9_SCC=true
# Mon, 27 Jun 2022 19:05:58 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Mon, 27 Jun 2022 19:06:02 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Mon, 27 Jun 2022 19:06:05 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Mon, 27 Jun 2022 19:06:10 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 27 Jun 2022 19:06:13 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Mon, 27 Jun 2022 19:06:17 GMT
ARG LIBERTY_URL
# Mon, 27 Jun 2022 19:06:22 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 27 Jun 2022 19:07:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 27 Jun 2022 19:07:15 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Jun 2022 19:07:20 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Mon, 27 Jun 2022 19:07:23 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 27 Jun 2022 19:07:30 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 27 Jun 2022 19:07:32 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Mon, 27 Jun 2022 19:07:33 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 27 Jun 2022 19:07:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 27 Jun 2022 19:07:55 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 27 Jun 2022 19:07:57 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Mon, 27 Jun 2022 19:08:01 GMT
USER 1001
# Mon, 27 Jun 2022 19:08:05 GMT
EXPOSE 9080 9443
# Mon, 27 Jun 2022 19:08:08 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 27 Jun 2022 19:08:10 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6c621e52fdf1e59e073b1c51c52e2e5a829be92510ef56949c609a03af2492`  
		Last Modified: Tue, 07 Jun 2022 07:30:19 GMT  
		Size: 17.2 MB (17203633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06eb9350ab17a87b8e47ac6a3389da7e21786ee038077cf7b627f90b125f1acf`  
		Last Modified: Tue, 07 Jun 2022 10:01:58 GMT  
		Size: 48.4 MB (48378487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc0d65d22cb0b40edcecacc4b8c684bc4bf1ddc89b24fd16e7abefba2b0c7df`  
		Last Modified: Tue, 07 Jun 2022 10:01:49 GMT  
		Size: 3.3 MB (3334009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5ff26c4cf89eaa05313a18d91d7309df617938eb84d02061347a609a33a7b8`  
		Last Modified: Mon, 27 Jun 2022 20:21:41 GMT  
		Size: 14.5 MB (14515853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ccfddb3da6a003c78fba8f80fd75c65f4fc295e3cc5bdf38bacf9e33c4844f`  
		Last Modified: Mon, 27 Jun 2022 20:21:32 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e827be780b6a43a9e9798fec11910f661a036eb43e9b207bd5a09dc0931e9b`  
		Last Modified: Mon, 27 Jun 2022 20:21:32 GMT  
		Size: 9.8 KB (9751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79a0d64d22b6a5861752d66f9cef744682bef6f31b78ac467d9065fadc0587c`  
		Last Modified: Mon, 27 Jun 2022 20:21:32 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93afd12b58a928c66cb4067a1a977a97bc0dacfe201dc9ad79c4800176e8cca`  
		Last Modified: Mon, 27 Jun 2022 20:21:32 GMT  
		Size: 10.7 KB (10734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210f9edeb69d5d47378b5b0de8220cb51a99548682efd824bb4fc5dce63089c3`  
		Last Modified: Mon, 27 Jun 2022 20:21:33 GMT  
		Size: 2.5 MB (2522136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.6-kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:0f4e2e03e7d5dbe6876dfb2c896c099cfb95a09b614bf2545aa10721cd0eb89e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110565665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4769a9a75c92ec85d9c8cd0a11812c5d4025e00ed223ebfe7cd8a0db797c0da7`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:41:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 12:41:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:43:42 GMT
ENV JAVA_VERSION=jdk-11.0.15+10_openj9-0.32.0
# Tue, 02 Aug 2022 12:44:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69e4a0b383c7b4187478ddb196de3cdc91560e2be40b8ef66354591e87c36e85';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5e82f7df54786c557d2d9e9ac22df655fd94b9702c73261390903ac87532d545';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='25d4d5e2bbe3eb19bcb9a76aec4b43d4eef5ad66200df3122118f69da5325cf6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='def85f1b00e9c65a8c3b5dcf4da0f1b04c17675b4ff9cd6f5dad61d8dcbd03d0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 12:44:51 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 12:44:51 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 12:45:24 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 00:31:25 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:31:25 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:31:25 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 00:31:25 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 00:31:25 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 00:31:26 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 00:31:26 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 00:31:26 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 00:31:26 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 00:31:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 00:31:38 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 00:31:38 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 00:31:38 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:31:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 00:31:39 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 00:31:39 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 00:31:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 00:31:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 00:31:46 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 00:31:46 GMT
USER 1001
# Wed, 03 Aug 2022 00:31:47 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 00:31:47 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 00:31:47 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:3f28b38375577480d13a8d78bab4c30073086c8a51a4ff217f32365aa0847411`  
		Last Modified: Tue, 02 Aug 2022 12:53:12 GMT  
		Size: 46.7 MB (46721680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3142744ed0637685528da62bbcb28da17d0b48fdc151bd52e7b22274eeb2c5da`  
		Last Modified: Tue, 02 Aug 2022 12:53:07 GMT  
		Size: 4.3 MB (4313565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9e7b387efd480990d6c64a866fba64fb104280672f530db487652f6a8b2420`  
		Last Modified: Wed, 03 Aug 2022 01:21:19 GMT  
		Size: 14.2 MB (14184080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d846195251009f85f9e3322ee32d4f6714c2208a979e2878e07e74634075b2`  
		Last Modified: Wed, 03 Aug 2022 01:21:17 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a4da3cc546eda0832bbac5eea20e393ef5335b890a0401290b55655e909ae4`  
		Last Modified: Wed, 03 Aug 2022 01:21:17 GMT  
		Size: 9.8 KB (9753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc9ec89f07bd2ea2472397191fdaf70131a284380baa496449e81346c8f9e97`  
		Last Modified: Wed, 03 Aug 2022 01:21:17 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6edb8309c1fef9cc240f64d15d2875b926152ce9f44aa1e3a2fa26b7eacecb`  
		Last Modified: Wed, 03 Aug 2022 01:21:16 GMT  
		Size: 10.7 KB (10726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c61c79763634b9154ab44813cd5f16fac38e3a947bc0e0a208f3468ae4c3910`  
		Last Modified: Wed, 03 Aug 2022 01:21:18 GMT  
		Size: 2.5 MB (2549406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.6-kernel-java17-openj9`

```console
$ docker pull websphere-liberty@sha256:e0544fe0929c36917d1641597cdc03bdcf16626d2be3e9c2c4525e10310e8390
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:22.0.0.6-kernel-java17-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:45d0cb42a4ca31d7a0b7c3a9c08bdff54d901e3a02f5035e27c128bb4e031b5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113855947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ca8e945cab711ceb4b45dae42e16abb300f5977010c6022309c35e48d9727bc`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 19:04:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 19:05:01 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:00:47 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Tue, 02 Aug 2022 20:02:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f899948ea0c5dc80a66f801db585939a25a4ae7e1f21a9a8f3bf3749c3baa87f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9c54166490ac55a6bd26249b57eae5df4531635f4871e6642e7979affc894875';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='dad35fec82047e3a82c6e2dda8b53ee763b55aaedaed13b7b130856f4a3ffd35';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='4e2f631ad18c288e419db5c35295829dd7e83f4cd1be95252db06eb622b23090';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 20:02:05 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 20:02:05 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 20:02:40 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 13:23:34 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:23:34 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:23:34 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 13:23:34 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 13:23:35 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 13:23:35 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 13:23:35 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 13:23:35 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 13:23:35 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 13:23:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 13:23:48 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 13:23:48 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 13:23:48 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:23:49 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 13:23:49 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 13:23:49 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 13:23:50 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 13:23:57 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 13:23:57 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 13:23:57 GMT
USER 1001
# Wed, 03 Aug 2022 13:23:57 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 13:23:58 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 13:23:58 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:7b6279e9931cb0efc3b60659be8fd46c95156f958f00818850fba3ac0ecd0616`  
		Last Modified: Tue, 02 Aug 2022 20:08:11 GMT  
		Size: 47.8 MB (47754438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e834be70bdf636e5c875d9e2badbf281d32ff675b9eb7db8768a2da9dbdf5e`  
		Last Modified: Tue, 02 Aug 2022 20:08:05 GMT  
		Size: 4.7 MB (4744099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b29111272e76b623f6a1c705052b79e4aed2ed08bb404f433fd8a20cd7c752`  
		Last Modified: Wed, 03 Aug 2022 14:16:14 GMT  
		Size: 14.2 MB (14183924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6606826ea4776a63f20adb28aca4a26e64d000ea040af34471de8c2366784452`  
		Last Modified: Wed, 03 Aug 2022 14:16:11 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa6ada95f6df02ffacedde72e53786a3bc150cc4bf94f7861f91a2cb9e026b0`  
		Last Modified: Wed, 03 Aug 2022 14:16:11 GMT  
		Size: 9.7 KB (9749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9521245474cad0537df9cfe305a8f740cb08a15941eea9bbd4b6d48ca6f91cd7`  
		Last Modified: Wed, 03 Aug 2022 14:16:11 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3f9ef840580663cf3012d2a8a7d7b03dab23484c4e62f2eba0004d6f4adaa`  
		Last Modified: Wed, 03 Aug 2022 14:16:11 GMT  
		Size: 10.7 KB (10725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f946b913fac313fce2c6d202c5ea9c9da8039c23dda2c638d1035e62305bc81`  
		Last Modified: Wed, 03 Aug 2022 14:16:11 GMT  
		Size: 2.5 MB (2549516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.6-kernel-java17-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:e07434f05a0ce037deb7160f615fd2c70ac87cd34fe541dfb1376ab0c729e822
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.4 MB (119366206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22291564784ba272c1f2bc0584e564e4bf1b4d7e1a1f88c7d48c94972dc2b219`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 07:16:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 07:18:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:52:39 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Tue, 07 Jun 2022 09:54:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f899948ea0c5dc80a66f801db585939a25a4ae7e1f21a9a8f3bf3749c3baa87f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9c54166490ac55a6bd26249b57eae5df4531635f4871e6642e7979affc894875';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='dad35fec82047e3a82c6e2dda8b53ee763b55aaedaed13b7b130856f4a3ffd35';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='4e2f631ad18c288e419db5c35295829dd7e83f4cd1be95252db06eb622b23090';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 09:54:20 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 09:54:22 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 07 Jun 2022 09:55:03 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 07 Jun 2022 11:31:51 GMT
ARG VERBOSE=false
# Tue, 07 Jun 2022 11:31:54 GMT
ARG OPENJ9_SCC=true
# Mon, 27 Jun 2022 19:08:20 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Mon, 27 Jun 2022 19:08:23 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Mon, 27 Jun 2022 19:08:26 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Mon, 27 Jun 2022 19:08:29 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 27 Jun 2022 19:08:32 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Mon, 27 Jun 2022 19:08:33 GMT
ARG LIBERTY_URL
# Mon, 27 Jun 2022 19:08:37 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 27 Jun 2022 19:09:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 27 Jun 2022 19:09:29 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Jun 2022 19:09:31 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Mon, 27 Jun 2022 19:09:32 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 27 Jun 2022 19:09:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 27 Jun 2022 19:09:42 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Mon, 27 Jun 2022 19:09:43 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 27 Jun 2022 19:09:52 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 27 Jun 2022 19:10:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 27 Jun 2022 19:10:11 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Mon, 27 Jun 2022 19:10:14 GMT
USER 1001
# Mon, 27 Jun 2022 19:10:17 GMT
EXPOSE 9080 9443
# Mon, 27 Jun 2022 19:10:18 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 27 Jun 2022 19:10:23 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6c621e52fdf1e59e073b1c51c52e2e5a829be92510ef56949c609a03af2492`  
		Last Modified: Tue, 07 Jun 2022 07:30:19 GMT  
		Size: 17.2 MB (17203633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643e82d1f37eb2778986afcd7aa289e4f42b3c21d19b6dc2b50320f2836d580e`  
		Last Modified: Tue, 07 Jun 2022 10:03:59 GMT  
		Size: 48.1 MB (48115319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe972a29b91980b448bef8b1d66c53f248a582f57eb8476283dad120863f562`  
		Last Modified: Tue, 07 Jun 2022 10:03:52 GMT  
		Size: 3.7 MB (3691417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c056cb98358395a411cf5384fbbdbec5ccfd5f81859801ac0c85148bbb98a4`  
		Last Modified: Mon, 27 Jun 2022 20:22:00 GMT  
		Size: 14.5 MB (14515851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd06b09fbbdc503b03e823a42d86309633c6d84767fa73330825bc907e14df3`  
		Last Modified: Mon, 27 Jun 2022 20:21:51 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbb19c1ede5ad19ca10791cc60a2f22dd80c54475f408a0e73abdccbca16792`  
		Last Modified: Mon, 27 Jun 2022 20:21:51 GMT  
		Size: 9.8 KB (9753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948cca84307d534dd3b66a3ccd42411c24283967d6c73d87983819647f564e0c`  
		Last Modified: Mon, 27 Jun 2022 20:21:51 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39dcdc56c341ef84605200c2bc492ee7ebd2d7d6c088f9188b4b724f2316504`  
		Last Modified: Mon, 27 Jun 2022 20:21:51 GMT  
		Size: 10.7 KB (10740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdde75f3ce0ceab51ecdf4a88f513912d5744afccff705acaa98d4d96a9399d1`  
		Last Modified: Mon, 27 Jun 2022 20:21:52 GMT  
		Size: 2.5 MB (2524189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.6-kernel-java17-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:c62c52f84546bd642194fb4433c49285d544ec2cd2f24248cca8005d22f5f795
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110744273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6eec6e01d0a5f110955696012d2ebe0ad4a9e76851e0e127c93e62daf1ad5f3`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:41:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 12:41:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:47:17 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Tue, 02 Aug 2022 12:48:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f899948ea0c5dc80a66f801db585939a25a4ae7e1f21a9a8f3bf3749c3baa87f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9c54166490ac55a6bd26249b57eae5df4531635f4871e6642e7979affc894875';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='dad35fec82047e3a82c6e2dda8b53ee763b55aaedaed13b7b130856f4a3ffd35';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='4e2f631ad18c288e419db5c35295829dd7e83f4cd1be95252db06eb622b23090';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 12:48:20 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 12:48:20 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 12:48:53 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 00:31:56 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:31:56 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:31:56 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 00:31:57 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 00:31:57 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 00:31:57 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 00:31:57 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 00:31:57 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 00:31:57 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 00:32:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 00:32:08 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 00:32:08 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 00:32:08 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:32:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 00:32:09 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 00:32:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 00:32:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 00:32:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 00:32:16 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 00:32:16 GMT
USER 1001
# Wed, 03 Aug 2022 00:32:16 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 00:32:17 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 00:32:17 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:8366f0be07eee724257935ccff074ac6069837c38e228be50a0b6f2e058ab16c`  
		Last Modified: Tue, 02 Aug 2022 12:54:24 GMT  
		Size: 46.2 MB (46241889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc471632f4e136d4fa45d0a7216573974cc332f3e9fa969846cb74f259e5e9cc`  
		Last Modified: Tue, 02 Aug 2022 12:54:19 GMT  
		Size: 4.9 MB (4939140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88edf1255c796274783dd2b408dda42ea663cad4b64810259c6acc1259419aa0`  
		Last Modified: Wed, 03 Aug 2022 01:21:26 GMT  
		Size: 14.2 MB (14184036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353a76e46cfbb610eda04921de105adf89120c8930d1974118798f627627b68b`  
		Last Modified: Wed, 03 Aug 2022 01:21:24 GMT  
		Size: 688.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfabfad0e607d1360481e4e76a8538189f1d761829c85652481cc8110f7abd2`  
		Last Modified: Wed, 03 Aug 2022 01:21:24 GMT  
		Size: 9.8 KB (9755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1851082a958effaac3cac4eddcea238e723fb008a9460dc32982226790cf22`  
		Last Modified: Wed, 03 Aug 2022 01:21:24 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3260426547d5393a73a84720e7ff09a76a39680394581d9c50107cb7f6f2489f`  
		Last Modified: Wed, 03 Aug 2022 01:21:24 GMT  
		Size: 10.7 KB (10734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fef24753132b515d30c6966531a9a4e35f7b4cc2441ecbe77dcaf61055f2ce0`  
		Last Modified: Wed, 03 Aug 2022 01:21:25 GMT  
		Size: 2.6 MB (2582268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.6-kernel-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:44a0e30e3602f0d562fd5e414320a91734fa268a9f7efdae99ab33928dd9ccc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:22.0.0.6-kernel-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:d258f8eef3e47e391cb9905ef349c148331ea5a324f0a3bd52bd4d1ad8b04b67
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.6 MB (178570162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b43de9f178d2b44f2956c8812deaed28d2515219c2bb51361d25585ca5e28dd`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:09:52 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 02 Aug 2022 20:10:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:10:01 GMT
ENV JAVA_VERSION=8.0.7.11
# Tue, 02 Aug 2022 20:10:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 02 Aug 2022 20:10:53 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 03 Aug 2022 13:22:32 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:22:32 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:22:32 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 13:22:33 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 13:22:33 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 13:22:33 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 13:22:33 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 13:22:33 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 13:22:33 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 13:22:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 13:22:51 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 13:22:51 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 13:22:51 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:22:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 13:22:53 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 13:22:53 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 13:22:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 13:23:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 13:23:02 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 03 Aug 2022 13:23:03 GMT
USER 1001
# Wed, 03 Aug 2022 13:23:03 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 13:23:03 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 13:23:03 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6715a1bb89fcf5e91403be2bc6130f23e6b3cfd0da73e6b09e937d028409d3`  
		Last Modified: Tue, 02 Aug 2022 20:13:24 GMT  
		Size: 3.0 MB (2957815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1607240ca884b25e20b8db8c53c4aea519b76a50e23c19a40aaadd508939589`  
		Last Modified: Tue, 02 Aug 2022 20:13:35 GMT  
		Size: 129.1 MB (129092301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb38c444df15407ab436886281e04c48950509ec0de9d9bc5203e14640165ddb`  
		Last Modified: Wed, 03 Aug 2022 14:15:54 GMT  
		Size: 14.1 MB (14085453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05aa53415f32b814deebc075a7bb595df58d79cf67a5fe218c1cd111e5b6ee0a`  
		Last Modified: Wed, 03 Aug 2022 14:15:50 GMT  
		Size: 679.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ddbf21b719f1a92ad3ee2ffed35afb7f2c0836d372a03e8ef6c86bc5546c4a`  
		Last Modified: Wed, 03 Aug 2022 14:15:50 GMT  
		Size: 9.8 KB (9757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5492e88c0d013bf0d79353e5c81b4167fe2b1aa74465b5c05edbf3b14658858a`  
		Last Modified: Wed, 03 Aug 2022 14:15:50 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f086c2ef5ce4893aeade47c11c788a8992b4e43bfa5e8316e9a13a422acb4b06`  
		Last Modified: Wed, 03 Aug 2022 14:15:50 GMT  
		Size: 10.7 KB (10735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3191d937acd525f20b08c085e17bb91eb22cf727d6199fd8049c53e3332a232`  
		Last Modified: Wed, 03 Aug 2022 14:15:51 GMT  
		Size: 5.7 MB (5702881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.6-kernel-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:d4b84c94d6be89b9404d44c13acf3d3ff5fec9d0d5d7d11821cc8b0186c2fd02
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.9 MB (181928476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a8aabaa6b07007819fd03084677523cb5f56c68083e93341cadd61df694d6ce`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:49:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 07 Jun 2022 08:50:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 18:31:53 GMT
ENV JAVA_VERSION=8.0.7.11
# Wed, 29 Jun 2022 18:33:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 29 Jun 2022 18:33:35 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 29 Jun 2022 19:03:57 GMT
ARG VERBOSE=false
# Wed, 29 Jun 2022 19:04:05 GMT
ARG OPENJ9_SCC=true
# Wed, 29 Jun 2022 19:04:16 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 29 Jun 2022 19:04:32 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 29 Jun 2022 19:04:39 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 29 Jun 2022 19:04:46 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 29 Jun 2022 19:04:53 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 29 Jun 2022 19:04:57 GMT
ARG LIBERTY_URL
# Wed, 29 Jun 2022 19:05:02 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 29 Jun 2022 19:06:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 19:06:54 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Jun 2022 19:06:59 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 29 Jun 2022 19:07:04 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 29 Jun 2022 19:07:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 29 Jun 2022 19:07:22 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 29 Jun 2022 19:07:27 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 29 Jun 2022 19:07:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 29 Jun 2022 19:08:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 29 Jun 2022 19:08:16 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 29 Jun 2022 19:08:20 GMT
USER 1001
# Wed, 29 Jun 2022 19:08:28 GMT
EXPOSE 9080 9443
# Wed, 29 Jun 2022 19:08:35 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 29 Jun 2022 19:08:44 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4a22aedc3b9f2593635b0a3f6fe64e6dd424850b9782f66e88c8c162926d6a`  
		Last Modified: Tue, 07 Jun 2022 08:54:16 GMT  
		Size: 3.1 MB (3082521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448aed354e59dc01b7da997655c86778001067ef107a5c1fb36a7c38fcf5fdda`  
		Last Modified: Wed, 29 Jun 2022 18:38:02 GMT  
		Size: 128.6 MB (128629743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ee64dfa956bec7a3911c4fbcec85677da5eb3557fdd1fad0cd05371b418ed3`  
		Last Modified: Wed, 29 Jun 2022 19:36:18 GMT  
		Size: 14.4 MB (14414087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f44198605bccf1a3fd327e2929165c362826698ef117c8ed5e5f61cf8471cce`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 685.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8008efd74eeabae4093e325cb3ee9f17c49e27f7dbb19564636c92acb9051471`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 9.8 KB (9757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df8e4e4d330f9771962db9ea9c4da8f370e92f1745f117e9db5baae643dfff3`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa888647a678f768a7a68d44ee29bc98b5834e1d4b43481f1d79fb22ae798d8`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 10.7 KB (10748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24233765490b95aea52162ad51e9982a4c6bd67895d93467ca629ea8bfb5a68`  
		Last Modified: Wed, 29 Jun 2022 19:36:15 GMT  
		Size: 5.3 MB (5337804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.6-kernel-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:311be6c24f4d54b605d3f60376debefcefe5db4fa5dffe4f0b853a68cd8d071f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.2 MB (174181742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba9247e8964bc01dc0c736aee5e2e2f6a718ee1017f272f2b918c7b93a98c542`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:01:57 GMT
ADD file:3d2e9b401524527b395347bc3847be7c9cb465b9a214a1a1d31e74330e293c45 in / 
# Tue, 02 Aug 2022 01:01:58 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 13:19:12 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 02 Aug 2022 13:19:25 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:19:25 GMT
ENV JAVA_VERSION=8.0.7.11
# Tue, 02 Aug 2022 13:20:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 02 Aug 2022 13:20:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 03 Aug 2022 00:30:47 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:30:48 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:30:48 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 00:30:48 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 00:30:48 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 00:30:49 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 00:30:49 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 00:30:49 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 00:30:49 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 00:31:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 00:31:03 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 00:31:03 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 00:31:03 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:31:06 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 00:31:07 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 00:31:07 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 00:31:08 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 00:31:17 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 00:31:18 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 03 Aug 2022 00:31:18 GMT
USER 1001
# Wed, 03 Aug 2022 00:31:18 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 00:31:18 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 00:31:19 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:be3ed498266c519f84268ff1f02085fa249c0e32fb60a59466e24c862b5f094b`  
		Last Modified: Tue, 02 Aug 2022 01:03:25 GMT  
		Size: 25.4 MB (25369584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2ed0adcefe11b30e3dff027bcb1cb9fe759f39f50b008bafb3644d3d2fcba8`  
		Last Modified: Tue, 02 Aug 2022 13:22:41 GMT  
		Size: 2.7 MB (2671706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745854ef92308f8e24873e2cf64eb998c725371b7d10ba8318989b37bba26f33`  
		Last Modified: Tue, 02 Aug 2022 13:22:49 GMT  
		Size: 126.1 MB (126143967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a59a661cbbb2b8555a22d1f6e2943fbf1eaa8381c6a30030ac4c3276c7cf1e8`  
		Last Modified: Wed, 03 Aug 2022 01:21:11 GMT  
		Size: 14.1 MB (14085532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19a28dc7880331492105ef80fe1628f9d15c71bc959cd9765cdcd64a139c472`  
		Last Modified: Wed, 03 Aug 2022 01:21:09 GMT  
		Size: 679.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc961a105d81f315d8af16fb228d90842f45dd9ff3a0ce06580d31bf5ae346c3`  
		Last Modified: Wed, 03 Aug 2022 01:21:09 GMT  
		Size: 9.8 KB (9763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07467c7f0c1b48d655b4ff47a1a5101cb4f28e77adce3d47f9c5bfaaaa1968a7`  
		Last Modified: Wed, 03 Aug 2022 01:21:08 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55abb9ff522a8f086c734b47a7b69b3d2770c58ec832b8d992f7e67766700ca8`  
		Last Modified: Wed, 03 Aug 2022 01:21:09 GMT  
		Size: 10.7 KB (10735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4009dc9f786bc5ce10ba8ebf96892fd74d20c3548ff8acc69160e27dcb3a615`  
		Last Modified: Wed, 03 Aug 2022 01:21:09 GMT  
		Size: 5.9 MB (5889501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:full`

```console
$ docker pull websphere-liberty@sha256:3a27bdeb56129c14e7bd4a664be6774a78b910e3d5203d585e55a23137c7c009
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:886abf89eb3316d1fa1e344b1c566b12c8c56dbdfe67ef1ab450f516026e19ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **461.9 MB (461889376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90501b5e0a18925bbd8d499cd561137878b9b24d6b69dcb7f15f4ad327d68c64`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:09:52 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 02 Aug 2022 20:10:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:10:01 GMT
ENV JAVA_VERSION=8.0.7.11
# Tue, 02 Aug 2022 20:10:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 02 Aug 2022 20:10:53 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 03 Aug 2022 13:22:32 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:22:32 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:22:32 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 13:22:33 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 13:22:33 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 13:22:33 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 13:22:33 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 13:22:33 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 13:22:33 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 13:22:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 13:22:51 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 13:22:51 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 13:22:51 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:22:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 13:22:53 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 13:22:53 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 13:22:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 13:23:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 13:23:02 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 03 Aug 2022 13:23:03 GMT
USER 1001
# Wed, 03 Aug 2022 13:23:03 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 13:23:03 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 13:23:03 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 03 Aug 2022 13:24:02 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:24:02 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 03 Aug 2022 13:31:35 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 03 Aug 2022 13:31:36 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 03 Aug 2022 13:32:07 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6715a1bb89fcf5e91403be2bc6130f23e6b3cfd0da73e6b09e937d028409d3`  
		Last Modified: Tue, 02 Aug 2022 20:13:24 GMT  
		Size: 3.0 MB (2957815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1607240ca884b25e20b8db8c53c4aea519b76a50e23c19a40aaadd508939589`  
		Last Modified: Tue, 02 Aug 2022 20:13:35 GMT  
		Size: 129.1 MB (129092301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb38c444df15407ab436886281e04c48950509ec0de9d9bc5203e14640165ddb`  
		Last Modified: Wed, 03 Aug 2022 14:15:54 GMT  
		Size: 14.1 MB (14085453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05aa53415f32b814deebc075a7bb595df58d79cf67a5fe218c1cd111e5b6ee0a`  
		Last Modified: Wed, 03 Aug 2022 14:15:50 GMT  
		Size: 679.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ddbf21b719f1a92ad3ee2ffed35afb7f2c0836d372a03e8ef6c86bc5546c4a`  
		Last Modified: Wed, 03 Aug 2022 14:15:50 GMT  
		Size: 9.8 KB (9757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5492e88c0d013bf0d79353e5c81b4167fe2b1aa74465b5c05edbf3b14658858a`  
		Last Modified: Wed, 03 Aug 2022 14:15:50 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f086c2ef5ce4893aeade47c11c788a8992b4e43bfa5e8316e9a13a422acb4b06`  
		Last Modified: Wed, 03 Aug 2022 14:15:50 GMT  
		Size: 10.7 KB (10735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3191d937acd525f20b08c085e17bb91eb22cf727d6199fd8049c53e3332a232`  
		Last Modified: Wed, 03 Aug 2022 14:15:51 GMT  
		Size: 5.7 MB (5702881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17cdf033149a3de277684874263c1eb2bedf5f30eb0a4012432b12def4c7822`  
		Last Modified: Wed, 03 Aug 2022 14:16:36 GMT  
		Size: 267.1 MB (267144319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10376ddb37d6232ae5252c9bdf6f04422f9557849cd611df7d58c8bf1185eede`  
		Last Modified: Wed, 03 Aug 2022 14:16:21 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5c901d7e4747e67d324ddb82affbf24e080a953b3ce5ed31ad1504258d171a`  
		Last Modified: Wed, 03 Aug 2022 14:16:24 GMT  
		Size: 16.2 MB (16173947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:20b8c8568ac1ace5302e32de4580705070ad867b1267fc10eddecc0342efb233
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.1 MB (463103256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24bec26d5b6e33bfa1465f31c5486fb46d341b64a8a89ebecee746a78fd2086b`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:49:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 07 Jun 2022 08:50:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 18:31:53 GMT
ENV JAVA_VERSION=8.0.7.11
# Wed, 29 Jun 2022 18:33:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 29 Jun 2022 18:33:35 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 29 Jun 2022 19:03:57 GMT
ARG VERBOSE=false
# Wed, 29 Jun 2022 19:04:05 GMT
ARG OPENJ9_SCC=true
# Wed, 29 Jun 2022 19:04:16 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 29 Jun 2022 19:04:32 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 29 Jun 2022 19:04:39 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 29 Jun 2022 19:04:46 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 29 Jun 2022 19:04:53 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 29 Jun 2022 19:04:57 GMT
ARG LIBERTY_URL
# Wed, 29 Jun 2022 19:05:02 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 29 Jun 2022 19:06:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 19:06:54 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Jun 2022 19:06:59 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 29 Jun 2022 19:07:04 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 29 Jun 2022 19:07:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 29 Jun 2022 19:07:22 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 29 Jun 2022 19:07:27 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 29 Jun 2022 19:07:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 29 Jun 2022 19:08:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 29 Jun 2022 19:08:16 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 29 Jun 2022 19:08:20 GMT
USER 1001
# Wed, 29 Jun 2022 19:08:28 GMT
EXPOSE 9080 9443
# Wed, 29 Jun 2022 19:08:35 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 29 Jun 2022 19:08:44 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 29 Jun 2022 19:09:19 GMT
ARG VERBOSE=false
# Wed, 29 Jun 2022 19:09:27 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 29 Jun 2022 19:18:40 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 29 Jun 2022 19:18:47 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 29 Jun 2022 19:19:57 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4a22aedc3b9f2593635b0a3f6fe64e6dd424850b9782f66e88c8c162926d6a`  
		Last Modified: Tue, 07 Jun 2022 08:54:16 GMT  
		Size: 3.1 MB (3082521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448aed354e59dc01b7da997655c86778001067ef107a5c1fb36a7c38fcf5fdda`  
		Last Modified: Wed, 29 Jun 2022 18:38:02 GMT  
		Size: 128.6 MB (128629743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ee64dfa956bec7a3911c4fbcec85677da5eb3557fdd1fad0cd05371b418ed3`  
		Last Modified: Wed, 29 Jun 2022 19:36:18 GMT  
		Size: 14.4 MB (14414087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f44198605bccf1a3fd327e2929165c362826698ef117c8ed5e5f61cf8471cce`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 685.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8008efd74eeabae4093e325cb3ee9f17c49e27f7dbb19564636c92acb9051471`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 9.8 KB (9757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df8e4e4d330f9771962db9ea9c4da8f370e92f1745f117e9db5baae643dfff3`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa888647a678f768a7a68d44ee29bc98b5834e1d4b43481f1d79fb22ae798d8`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 10.7 KB (10748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24233765490b95aea52162ad51e9982a4c6bd67895d93467ca629ea8bfb5a68`  
		Last Modified: Wed, 29 Jun 2022 19:36:15 GMT  
		Size: 5.3 MB (5337804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a597fe1c695442d024092e9ba428ea88ffa886c912a199fbe492b776a53a7595`  
		Last Modified: Wed, 29 Jun 2022 19:36:52 GMT  
		Size: 267.1 MB (267144840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165a7c33a3339f487205b064950b8fb81222d47d74c6fdfef158d7464150dbbb`  
		Last Modified: Wed, 29 Jun 2022 19:36:29 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ede9c741b2ef54fc67a38aab455cdc0ef8bea790cfdf300b7e1d01aa4486ec`  
		Last Modified: Wed, 29 Jun 2022 19:36:35 GMT  
		Size: 14.0 MB (14028991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:f6b028efccb8a1d3a8e7633ab097afc5ef7ea9eb145ecff4d148ebf489240309
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **457.5 MB (457473936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52b2b35b4ae3c6168a008c1dd5dccb115e7bc94a70e161ac19b8340a87a722b7`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:01:57 GMT
ADD file:3d2e9b401524527b395347bc3847be7c9cb465b9a214a1a1d31e74330e293c45 in / 
# Tue, 02 Aug 2022 01:01:58 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 13:19:12 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 02 Aug 2022 13:19:25 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:19:25 GMT
ENV JAVA_VERSION=8.0.7.11
# Tue, 02 Aug 2022 13:20:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 02 Aug 2022 13:20:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 03 Aug 2022 00:30:47 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:30:48 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:30:48 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 00:30:48 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 00:30:48 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 00:30:49 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 00:30:49 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 00:30:49 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 00:30:49 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 00:31:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 00:31:03 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 00:31:03 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 00:31:03 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:31:06 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 00:31:07 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 00:31:07 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 00:31:08 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 00:31:17 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 00:31:18 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 03 Aug 2022 00:31:18 GMT
USER 1001
# Wed, 03 Aug 2022 00:31:18 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 00:31:18 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 00:31:19 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 03 Aug 2022 00:32:24 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:32:24 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 03 Aug 2022 00:39:41 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 03 Aug 2022 00:40:02 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 03 Aug 2022 00:40:42 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:be3ed498266c519f84268ff1f02085fa249c0e32fb60a59466e24c862b5f094b`  
		Last Modified: Tue, 02 Aug 2022 01:03:25 GMT  
		Size: 25.4 MB (25369584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2ed0adcefe11b30e3dff027bcb1cb9fe759f39f50b008bafb3644d3d2fcba8`  
		Last Modified: Tue, 02 Aug 2022 13:22:41 GMT  
		Size: 2.7 MB (2671706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745854ef92308f8e24873e2cf64eb998c725371b7d10ba8318989b37bba26f33`  
		Last Modified: Tue, 02 Aug 2022 13:22:49 GMT  
		Size: 126.1 MB (126143967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a59a661cbbb2b8555a22d1f6e2943fbf1eaa8381c6a30030ac4c3276c7cf1e8`  
		Last Modified: Wed, 03 Aug 2022 01:21:11 GMT  
		Size: 14.1 MB (14085532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19a28dc7880331492105ef80fe1628f9d15c71bc959cd9765cdcd64a139c472`  
		Last Modified: Wed, 03 Aug 2022 01:21:09 GMT  
		Size: 679.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc961a105d81f315d8af16fb228d90842f45dd9ff3a0ce06580d31bf5ae346c3`  
		Last Modified: Wed, 03 Aug 2022 01:21:09 GMT  
		Size: 9.8 KB (9763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07467c7f0c1b48d655b4ff47a1a5101cb4f28e77adce3d47f9c5bfaaaa1968a7`  
		Last Modified: Wed, 03 Aug 2022 01:21:08 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55abb9ff522a8f086c734b47a7b69b3d2770c58ec832b8d992f7e67766700ca8`  
		Last Modified: Wed, 03 Aug 2022 01:21:09 GMT  
		Size: 10.7 KB (10735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4009dc9f786bc5ce10ba8ebf96892fd74d20c3548ff8acc69160e27dcb3a615`  
		Last Modified: Wed, 03 Aug 2022 01:21:09 GMT  
		Size: 5.9 MB (5889501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e27310727e03cbd34d78cf4d4b95a8e316a4b322be112db401ab8c19e495739`  
		Last Modified: Wed, 03 Aug 2022 01:21:43 GMT  
		Size: 267.1 MB (267143557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7fa949e35b734374f99454dc3a7a9f7dba0a28dd865c7ca9514f169950d991`  
		Last Modified: Wed, 03 Aug 2022 01:21:31 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3f51986dc9d010c1551d1d44b8efb475ea65824d2ae8e3fba9476278e13ff0`  
		Last Modified: Wed, 03 Aug 2022 01:21:33 GMT  
		Size: 16.1 MB (16147687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:326189db7af92893f0e3b341351f8a334fb5cf93f5735d768529122da6b858e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:9b3977be801ee7d384fb934fd6c8c24640b0de518141ee7efa557b280e6f4b40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **394.9 MB (394928920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cdb74cfa2ffeffb22e4d0b330871c4e06e42acb96eb1fb693d45fb5222577d6`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 19:04:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 19:05:01 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 19:56:56 GMT
ENV JAVA_VERSION=jdk-11.0.15+10_openj9-0.32.0
# Tue, 02 Aug 2022 19:58:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69e4a0b383c7b4187478ddb196de3cdc91560e2be40b8ef66354591e87c36e85';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5e82f7df54786c557d2d9e9ac22df655fd94b9702c73261390903ac87532d545';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='25d4d5e2bbe3eb19bcb9a76aec4b43d4eef5ad66200df3122118f69da5325cf6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='def85f1b00e9c65a8c3b5dcf4da0f1b04c17675b4ff9cd6f5dad61d8dcbd03d0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 19:58:02 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 19:58:02 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 19:58:37 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 13:23:06 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:23:06 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:23:06 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 13:23:06 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 13:23:06 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 13:23:06 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 13:23:07 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 13:23:07 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 13:23:07 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 13:23:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 13:23:20 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 13:23:20 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 13:23:20 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:23:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 13:23:21 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 13:23:21 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 13:23:22 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 13:23:29 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 13:23:29 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 13:23:29 GMT
USER 1001
# Wed, 03 Aug 2022 13:23:29 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 13:23:29 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 13:23:29 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 03 Aug 2022 13:32:10 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:32:11 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 03 Aug 2022 13:39:49 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 03 Aug 2022 13:39:51 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 03 Aug 2022 13:40:20 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:a84b3718e4bf43f94609ec6fedf833567945fd97d9b8c324995df295d627fbb7`  
		Last Modified: Tue, 02 Aug 2022 20:06:46 GMT  
		Size: 47.7 MB (47691482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c02c82f8c35f778ae48a325cbccf65292ecbdea6e70272147ca65f72cda4dd`  
		Last Modified: Tue, 02 Aug 2022 20:06:39 GMT  
		Size: 4.2 MB (4183653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f41d289bc930a3a92caf3a90f84db2362a42680dd7ce48a2e1befa89078e3d`  
		Last Modified: Wed, 03 Aug 2022 14:16:04 GMT  
		Size: 14.2 MB (14183927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe3d80467e0f8bbeb61b656c7c4ed7ce644a4d1c7eab501f1b6a0e7fe8375b4`  
		Last Modified: Wed, 03 Aug 2022 14:16:00 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b9afcc7c926f3a529e2ea516fde829c98dbefe91c9d6f6ad3da2566ac205aff`  
		Last Modified: Wed, 03 Aug 2022 14:16:00 GMT  
		Size: 9.8 KB (9754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1691ca21cc220ab5c388a3736a7d146f33ae925532fb1608e128ef9b5d0bae8`  
		Last Modified: Wed, 03 Aug 2022 14:16:00 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a698c8b450bdc7160dc4aec60aec1b5bf12d3eba41cacac8016a21efc396f6`  
		Last Modified: Wed, 03 Aug 2022 14:16:00 GMT  
		Size: 10.7 KB (10731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d3164f01d38ac4bfa365542bbba93799c6f0fdd8ac6a8ae099ff4b510397a5`  
		Last Modified: Wed, 03 Aug 2022 14:16:01 GMT  
		Size: 2.5 MB (2534099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1ab2301875a334deb371209e9dca924755437756da96780092a995e0a1f0c6`  
		Last Modified: Wed, 03 Aug 2022 14:16:59 GMT  
		Size: 267.1 MB (267144880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14816fa7889d9e1162dce8c26791c4f7fdd3205871ffd806993820d0dcf26e59`  
		Last Modified: Wed, 03 Aug 2022 14:16:46 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ff575ec50297731f1e101a1281569273f275b1b37d235d1ef010528a460cdc`  
		Last Modified: Wed, 03 Aug 2022 14:16:48 GMT  
		Size: 14.6 MB (14565953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:568ef80bcca1347cbe226376d843073d6a27ba7c43cc818dc85e6d15bf59e28f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.9 MB (399864626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:270f4646bfd8b7ae7175d55df724300751667413afa34555b6d898b0fd2ab212`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 07:16:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 07:18:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:46:26 GMT
ENV JAVA_VERSION=jdk-11.0.15+10_openj9-0.32.0
# Tue, 07 Jun 2022 09:48:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69e4a0b383c7b4187478ddb196de3cdc91560e2be40b8ef66354591e87c36e85';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5e82f7df54786c557d2d9e9ac22df655fd94b9702c73261390903ac87532d545';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='25d4d5e2bbe3eb19bcb9a76aec4b43d4eef5ad66200df3122118f69da5325cf6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='def85f1b00e9c65a8c3b5dcf4da0f1b04c17675b4ff9cd6f5dad61d8dcbd03d0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 09:48:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 09:48:28 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 07 Jun 2022 09:49:12 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 07 Jun 2022 11:28:13 GMT
ARG VERBOSE=false
# Tue, 07 Jun 2022 11:28:23 GMT
ARG OPENJ9_SCC=true
# Mon, 27 Jun 2022 19:05:58 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Mon, 27 Jun 2022 19:06:02 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Mon, 27 Jun 2022 19:06:05 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Mon, 27 Jun 2022 19:06:10 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 27 Jun 2022 19:06:13 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Mon, 27 Jun 2022 19:06:17 GMT
ARG LIBERTY_URL
# Mon, 27 Jun 2022 19:06:22 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 27 Jun 2022 19:07:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 27 Jun 2022 19:07:15 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Jun 2022 19:07:20 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Mon, 27 Jun 2022 19:07:23 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 27 Jun 2022 19:07:30 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 27 Jun 2022 19:07:32 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Mon, 27 Jun 2022 19:07:33 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 27 Jun 2022 19:07:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 27 Jun 2022 19:07:55 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 27 Jun 2022 19:07:57 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Mon, 27 Jun 2022 19:08:01 GMT
USER 1001
# Mon, 27 Jun 2022 19:08:05 GMT
EXPOSE 9080 9443
# Mon, 27 Jun 2022 19:08:08 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 27 Jun 2022 19:08:10 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Mon, 27 Jun 2022 19:20:56 GMT
ARG VERBOSE=false
# Mon, 27 Jun 2022 19:20:59 GMT
ARG REPOSITORIES_PROPERTIES=
# Mon, 27 Jun 2022 19:30:13 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Mon, 27 Jun 2022 19:30:26 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Mon, 27 Jun 2022 19:31:35 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6c621e52fdf1e59e073b1c51c52e2e5a829be92510ef56949c609a03af2492`  
		Last Modified: Tue, 07 Jun 2022 07:30:19 GMT  
		Size: 17.2 MB (17203633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06eb9350ab17a87b8e47ac6a3389da7e21786ee038077cf7b627f90b125f1acf`  
		Last Modified: Tue, 07 Jun 2022 10:01:58 GMT  
		Size: 48.4 MB (48378487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc0d65d22cb0b40edcecacc4b8c684bc4bf1ddc89b24fd16e7abefba2b0c7df`  
		Last Modified: Tue, 07 Jun 2022 10:01:49 GMT  
		Size: 3.3 MB (3334009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5ff26c4cf89eaa05313a18d91d7309df617938eb84d02061347a609a33a7b8`  
		Last Modified: Mon, 27 Jun 2022 20:21:41 GMT  
		Size: 14.5 MB (14515853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ccfddb3da6a003c78fba8f80fd75c65f4fc295e3cc5bdf38bacf9e33c4844f`  
		Last Modified: Mon, 27 Jun 2022 20:21:32 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e827be780b6a43a9e9798fec11910f661a036eb43e9b207bd5a09dc0931e9b`  
		Last Modified: Mon, 27 Jun 2022 20:21:32 GMT  
		Size: 9.8 KB (9751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79a0d64d22b6a5861752d66f9cef744682bef6f31b78ac467d9065fadc0587c`  
		Last Modified: Mon, 27 Jun 2022 20:21:32 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93afd12b58a928c66cb4067a1a977a97bc0dacfe201dc9ad79c4800176e8cca`  
		Last Modified: Mon, 27 Jun 2022 20:21:32 GMT  
		Size: 10.7 KB (10734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210f9edeb69d5d47378b5b0de8220cb51a99548682efd824bb4fc5dce63089c3`  
		Last Modified: Mon, 27 Jun 2022 20:21:33 GMT  
		Size: 2.5 MB (2522136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610e5d1cf0778b270585e8c568433ebe0d1721c289aef87a4e33139fbfc8be22`  
		Last Modified: Mon, 27 Jun 2022 20:23:50 GMT  
		Size: 267.1 MB (267145041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823da95363ffd3cef0df423c707c5741e0e46d33a1211239731e7020f132c98b`  
		Last Modified: Mon, 27 Jun 2022 20:23:27 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a806cb8e7c52d02a647b832925c7dd227d390e06af95aa5ca784a9e3e796a7`  
		Last Modified: Mon, 27 Jun 2022 20:23:30 GMT  
		Size: 13.4 MB (13448725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:30360124bffc5d586450ed00757b3da2b07527fdd14f607522e7113a68c4d6c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.3 MB (392311995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6380aa33c3d2bf9aa3cda4cb99b404ff94433d361c0026bcd2d70911bf9fc2fa`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:41:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 12:41:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:43:42 GMT
ENV JAVA_VERSION=jdk-11.0.15+10_openj9-0.32.0
# Tue, 02 Aug 2022 12:44:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69e4a0b383c7b4187478ddb196de3cdc91560e2be40b8ef66354591e87c36e85';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5e82f7df54786c557d2d9e9ac22df655fd94b9702c73261390903ac87532d545';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='25d4d5e2bbe3eb19bcb9a76aec4b43d4eef5ad66200df3122118f69da5325cf6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='def85f1b00e9c65a8c3b5dcf4da0f1b04c17675b4ff9cd6f5dad61d8dcbd03d0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 12:44:51 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 12:44:51 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 12:45:24 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 00:31:25 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:31:25 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:31:25 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 00:31:25 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 00:31:25 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 00:31:26 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 00:31:26 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 00:31:26 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 00:31:26 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 00:31:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 00:31:38 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 00:31:38 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 00:31:38 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:31:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 00:31:39 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 00:31:39 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 00:31:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 00:31:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 00:31:46 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 00:31:46 GMT
USER 1001
# Wed, 03 Aug 2022 00:31:47 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 00:31:47 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 00:31:47 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 03 Aug 2022 00:40:52 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:40:53 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 03 Aug 2022 00:48:29 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 03 Aug 2022 00:48:41 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 03 Aug 2022 00:49:06 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:3f28b38375577480d13a8d78bab4c30073086c8a51a4ff217f32365aa0847411`  
		Last Modified: Tue, 02 Aug 2022 12:53:12 GMT  
		Size: 46.7 MB (46721680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3142744ed0637685528da62bbcb28da17d0b48fdc151bd52e7b22274eeb2c5da`  
		Last Modified: Tue, 02 Aug 2022 12:53:07 GMT  
		Size: 4.3 MB (4313565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9e7b387efd480990d6c64a866fba64fb104280672f530db487652f6a8b2420`  
		Last Modified: Wed, 03 Aug 2022 01:21:19 GMT  
		Size: 14.2 MB (14184080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d846195251009f85f9e3322ee32d4f6714c2208a979e2878e07e74634075b2`  
		Last Modified: Wed, 03 Aug 2022 01:21:17 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a4da3cc546eda0832bbac5eea20e393ef5335b890a0401290b55655e909ae4`  
		Last Modified: Wed, 03 Aug 2022 01:21:17 GMT  
		Size: 9.8 KB (9753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc9ec89f07bd2ea2472397191fdaf70131a284380baa496449e81346c8f9e97`  
		Last Modified: Wed, 03 Aug 2022 01:21:17 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6edb8309c1fef9cc240f64d15d2875b926152ce9f44aa1e3a2fa26b7eacecb`  
		Last Modified: Wed, 03 Aug 2022 01:21:16 GMT  
		Size: 10.7 KB (10726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c61c79763634b9154ab44813cd5f16fac38e3a947bc0e0a208f3468ae4c3910`  
		Last Modified: Wed, 03 Aug 2022 01:21:18 GMT  
		Size: 2.5 MB (2549406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc0bd9df0380ed2d04e74a81ae642853add021ebef188564b042d142d7b5faa`  
		Last Modified: Wed, 03 Aug 2022 01:22:02 GMT  
		Size: 267.1 MB (267143265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e189831428d2706995b316dcfcdb2f9dbde838fbd1a188ac5d869aaf028d1f4a`  
		Last Modified: Wed, 03 Aug 2022 01:21:51 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557ad0e62e6ef6a383af9d2f91a0b9d5fc0ebefdbd530332b73d31367e3ac446`  
		Last Modified: Wed, 03 Aug 2022 01:21:52 GMT  
		Size: 14.6 MB (14602122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:full-java17-openj9`

```console
$ docker pull websphere-liberty@sha256:34362463fcb358b55f026fefe7cc6e114bcfe9508795a4d11d4487d090c2a389
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full-java17-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:8337943a15d51cb83b3b793640a07bd4e5fcba7e5416ce631c2ff0aefee030c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (396008706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0c46e520aae2f1050803a9fb2df6a5a9a897d207ae26a4449a0faea6499711e`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 19:04:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 19:05:01 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:00:47 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Tue, 02 Aug 2022 20:02:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f899948ea0c5dc80a66f801db585939a25a4ae7e1f21a9a8f3bf3749c3baa87f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9c54166490ac55a6bd26249b57eae5df4531635f4871e6642e7979affc894875';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='dad35fec82047e3a82c6e2dda8b53ee763b55aaedaed13b7b130856f4a3ffd35';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='4e2f631ad18c288e419db5c35295829dd7e83f4cd1be95252db06eb622b23090';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 20:02:05 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 20:02:05 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 20:02:40 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 13:23:34 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:23:34 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:23:34 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 13:23:34 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 13:23:35 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 13:23:35 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 13:23:35 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 13:23:35 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 13:23:35 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 13:23:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 13:23:48 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 13:23:48 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 13:23:48 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:23:49 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 13:23:49 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 13:23:49 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 13:23:50 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 13:23:57 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 13:23:57 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 13:23:57 GMT
USER 1001
# Wed, 03 Aug 2022 13:23:57 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 13:23:58 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 13:23:58 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 03 Aug 2022 13:40:34 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:40:34 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 03 Aug 2022 13:48:12 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 03 Aug 2022 13:48:14 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 03 Aug 2022 13:48:44 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:7b6279e9931cb0efc3b60659be8fd46c95156f958f00818850fba3ac0ecd0616`  
		Last Modified: Tue, 02 Aug 2022 20:08:11 GMT  
		Size: 47.8 MB (47754438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e834be70bdf636e5c875d9e2badbf281d32ff675b9eb7db8768a2da9dbdf5e`  
		Last Modified: Tue, 02 Aug 2022 20:08:05 GMT  
		Size: 4.7 MB (4744099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b29111272e76b623f6a1c705052b79e4aed2ed08bb404f433fd8a20cd7c752`  
		Last Modified: Wed, 03 Aug 2022 14:16:14 GMT  
		Size: 14.2 MB (14183924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6606826ea4776a63f20adb28aca4a26e64d000ea040af34471de8c2366784452`  
		Last Modified: Wed, 03 Aug 2022 14:16:11 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa6ada95f6df02ffacedde72e53786a3bc150cc4bf94f7861f91a2cb9e026b0`  
		Last Modified: Wed, 03 Aug 2022 14:16:11 GMT  
		Size: 9.7 KB (9749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9521245474cad0537df9cfe305a8f740cb08a15941eea9bbd4b6d48ca6f91cd7`  
		Last Modified: Wed, 03 Aug 2022 14:16:11 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3f9ef840580663cf3012d2a8a7d7b03dab23484c4e62f2eba0004d6f4adaa`  
		Last Modified: Wed, 03 Aug 2022 14:16:11 GMT  
		Size: 10.7 KB (10725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f946b913fac313fce2c6d202c5ea9c9da8039c23dda2c638d1035e62305bc81`  
		Last Modified: Wed, 03 Aug 2022 14:16:11 GMT  
		Size: 2.5 MB (2549516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d00dd2ab51ffc9eeabfa9eca2f588e9cb53c5fc4ba3ef2021fb3f12e357f19`  
		Last Modified: Wed, 03 Aug 2022 14:17:20 GMT  
		Size: 267.1 MB (267144532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b633affe3bbc937124f9773be4f737c55d2f47a37f2308dbfb0a7199110753`  
		Last Modified: Wed, 03 Aug 2022 14:17:06 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a02c200927d909642073247ea75742a772e35a2e308cb01aa2ab9a5f81f82d`  
		Last Modified: Wed, 03 Aug 2022 14:17:08 GMT  
		Size: 15.0 MB (15007284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java17-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:d2b38cf5aeaf7df489e9b960daf12f80ff3351af7cb88d0f598dfe388b1cc414
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.3 MB (399269706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce1658e884c9121f94bdddfa7883b8ca0797266dc1a09218a559585fe3960aef`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 07:16:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 07:18:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:52:39 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Tue, 07 Jun 2022 09:54:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f899948ea0c5dc80a66f801db585939a25a4ae7e1f21a9a8f3bf3749c3baa87f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9c54166490ac55a6bd26249b57eae5df4531635f4871e6642e7979affc894875';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='dad35fec82047e3a82c6e2dda8b53ee763b55aaedaed13b7b130856f4a3ffd35';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='4e2f631ad18c288e419db5c35295829dd7e83f4cd1be95252db06eb622b23090';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 09:54:20 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 09:54:22 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 07 Jun 2022 09:55:03 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 07 Jun 2022 11:31:51 GMT
ARG VERBOSE=false
# Tue, 07 Jun 2022 11:31:54 GMT
ARG OPENJ9_SCC=true
# Mon, 27 Jun 2022 19:08:20 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Mon, 27 Jun 2022 19:08:23 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Mon, 27 Jun 2022 19:08:26 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Mon, 27 Jun 2022 19:08:29 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 27 Jun 2022 19:08:32 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Mon, 27 Jun 2022 19:08:33 GMT
ARG LIBERTY_URL
# Mon, 27 Jun 2022 19:08:37 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 27 Jun 2022 19:09:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 27 Jun 2022 19:09:29 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Jun 2022 19:09:31 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Mon, 27 Jun 2022 19:09:32 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 27 Jun 2022 19:09:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 27 Jun 2022 19:09:42 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Mon, 27 Jun 2022 19:09:43 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 27 Jun 2022 19:09:52 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 27 Jun 2022 19:10:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 27 Jun 2022 19:10:11 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Mon, 27 Jun 2022 19:10:14 GMT
USER 1001
# Mon, 27 Jun 2022 19:10:17 GMT
EXPOSE 9080 9443
# Mon, 27 Jun 2022 19:10:18 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 27 Jun 2022 19:10:23 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Mon, 27 Jun 2022 19:31:54 GMT
ARG VERBOSE=false
# Mon, 27 Jun 2022 19:31:58 GMT
ARG REPOSITORIES_PROPERTIES=
# Mon, 27 Jun 2022 19:41:31 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Mon, 27 Jun 2022 19:41:38 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Mon, 27 Jun 2022 19:42:34 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6c621e52fdf1e59e073b1c51c52e2e5a829be92510ef56949c609a03af2492`  
		Last Modified: Tue, 07 Jun 2022 07:30:19 GMT  
		Size: 17.2 MB (17203633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643e82d1f37eb2778986afcd7aa289e4f42b3c21d19b6dc2b50320f2836d580e`  
		Last Modified: Tue, 07 Jun 2022 10:03:59 GMT  
		Size: 48.1 MB (48115319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe972a29b91980b448bef8b1d66c53f248a582f57eb8476283dad120863f562`  
		Last Modified: Tue, 07 Jun 2022 10:03:52 GMT  
		Size: 3.7 MB (3691417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c056cb98358395a411cf5384fbbdbec5ccfd5f81859801ac0c85148bbb98a4`  
		Last Modified: Mon, 27 Jun 2022 20:22:00 GMT  
		Size: 14.5 MB (14515851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd06b09fbbdc503b03e823a42d86309633c6d84767fa73330825bc907e14df3`  
		Last Modified: Mon, 27 Jun 2022 20:21:51 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbb19c1ede5ad19ca10791cc60a2f22dd80c54475f408a0e73abdccbca16792`  
		Last Modified: Mon, 27 Jun 2022 20:21:51 GMT  
		Size: 9.8 KB (9753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948cca84307d534dd3b66a3ccd42411c24283967d6c73d87983819647f564e0c`  
		Last Modified: Mon, 27 Jun 2022 20:21:51 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39dcdc56c341ef84605200c2bc492ee7ebd2d7d6c088f9188b4b724f2316504`  
		Last Modified: Mon, 27 Jun 2022 20:21:51 GMT  
		Size: 10.7 KB (10740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdde75f3ce0ceab51ecdf4a88f513912d5744afccff705acaa98d4d96a9399d1`  
		Last Modified: Mon, 27 Jun 2022 20:21:52 GMT  
		Size: 2.5 MB (2524189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70d3a471d83cfe5ea6fb0e3494c7237e036a1b239cdd198d683ced84e37b6b8`  
		Last Modified: Mon, 27 Jun 2022 20:24:24 GMT  
		Size: 267.1 MB (267144514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cd749118a548d29d9d565402d900fd0e6cf95d4f72a07133d3adf7cd3c4b29`  
		Last Modified: Mon, 27 Jun 2022 20:24:00 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca0169250169b2ddc110e2a4d47306077c03fc3040d77c4d134e177924a5193`  
		Last Modified: Mon, 27 Jun 2022 20:24:03 GMT  
		Size: 12.8 MB (12758043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java17-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:f69a28b7536236c0a60225c9f8f051862dc9a5e3f7cddcc3765ad686052fc9a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.7 MB (392657062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9618452d33ff355bf5b087737ad9ac477c3db4bc630c4a75304cbb38ca5142da`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:41:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 12:41:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:47:17 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Tue, 02 Aug 2022 12:48:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f899948ea0c5dc80a66f801db585939a25a4ae7e1f21a9a8f3bf3749c3baa87f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9c54166490ac55a6bd26249b57eae5df4531635f4871e6642e7979affc894875';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='dad35fec82047e3a82c6e2dda8b53ee763b55aaedaed13b7b130856f4a3ffd35';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='4e2f631ad18c288e419db5c35295829dd7e83f4cd1be95252db06eb622b23090';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 12:48:20 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 12:48:20 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 12:48:53 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 00:31:56 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:31:56 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:31:56 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 00:31:57 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 00:31:57 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 00:31:57 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 00:31:57 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 00:31:57 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 00:31:57 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 00:32:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 00:32:08 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 00:32:08 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 00:32:08 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:32:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 00:32:09 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 00:32:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 00:32:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 00:32:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 00:32:16 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 00:32:16 GMT
USER 1001
# Wed, 03 Aug 2022 00:32:16 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 00:32:17 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 00:32:17 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 03 Aug 2022 00:49:19 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:49:19 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 03 Aug 2022 00:56:16 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 03 Aug 2022 00:56:21 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 03 Aug 2022 00:56:46 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:8366f0be07eee724257935ccff074ac6069837c38e228be50a0b6f2e058ab16c`  
		Last Modified: Tue, 02 Aug 2022 12:54:24 GMT  
		Size: 46.2 MB (46241889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc471632f4e136d4fa45d0a7216573974cc332f3e9fa969846cb74f259e5e9cc`  
		Last Modified: Tue, 02 Aug 2022 12:54:19 GMT  
		Size: 4.9 MB (4939140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88edf1255c796274783dd2b408dda42ea663cad4b64810259c6acc1259419aa0`  
		Last Modified: Wed, 03 Aug 2022 01:21:26 GMT  
		Size: 14.2 MB (14184036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353a76e46cfbb610eda04921de105adf89120c8930d1974118798f627627b68b`  
		Last Modified: Wed, 03 Aug 2022 01:21:24 GMT  
		Size: 688.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfabfad0e607d1360481e4e76a8538189f1d761829c85652481cc8110f7abd2`  
		Last Modified: Wed, 03 Aug 2022 01:21:24 GMT  
		Size: 9.8 KB (9755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1851082a958effaac3cac4eddcea238e723fb008a9460dc32982226790cf22`  
		Last Modified: Wed, 03 Aug 2022 01:21:24 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3260426547d5393a73a84720e7ff09a76a39680394581d9c50107cb7f6f2489f`  
		Last Modified: Wed, 03 Aug 2022 01:21:24 GMT  
		Size: 10.7 KB (10734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fef24753132b515d30c6966531a9a4e35f7b4cc2441ecbe77dcaf61055f2ce0`  
		Last Modified: Wed, 03 Aug 2022 01:21:25 GMT  
		Size: 2.6 MB (2582268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8976d85227f2d0aba5790a1cea3c5acf86bbae43c589ad3f20b2a7c21dd101b`  
		Last Modified: Wed, 03 Aug 2022 01:22:19 GMT  
		Size: 267.1 MB (267143376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5168ad06a92f4ca58fcdb0144b2c1921376af9657fcaf25b6a85d25b2af1732c`  
		Last Modified: Wed, 03 Aug 2022 01:22:07 GMT  
		Size: 941.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afc1985dd70a701d3ee6a9b6ffcbc88686fe3d09ccc6811624d5c32a95d69e7`  
		Last Modified: Wed, 03 Aug 2022 01:22:09 GMT  
		Size: 14.8 MB (14768472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:kernel`

```console
$ docker pull websphere-liberty@sha256:44a0e30e3602f0d562fd5e414320a91734fa268a9f7efdae99ab33928dd9ccc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:kernel` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:d258f8eef3e47e391cb9905ef349c148331ea5a324f0a3bd52bd4d1ad8b04b67
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.6 MB (178570162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b43de9f178d2b44f2956c8812deaed28d2515219c2bb51361d25585ca5e28dd`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:09:52 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 02 Aug 2022 20:10:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:10:01 GMT
ENV JAVA_VERSION=8.0.7.11
# Tue, 02 Aug 2022 20:10:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 02 Aug 2022 20:10:53 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 03 Aug 2022 13:22:32 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:22:32 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:22:32 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 13:22:33 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 13:22:33 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 13:22:33 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 13:22:33 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 13:22:33 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 13:22:33 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 13:22:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 13:22:51 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 13:22:51 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 13:22:51 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:22:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 13:22:53 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 13:22:53 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 13:22:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 13:23:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 13:23:02 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 03 Aug 2022 13:23:03 GMT
USER 1001
# Wed, 03 Aug 2022 13:23:03 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 13:23:03 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 13:23:03 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6715a1bb89fcf5e91403be2bc6130f23e6b3cfd0da73e6b09e937d028409d3`  
		Last Modified: Tue, 02 Aug 2022 20:13:24 GMT  
		Size: 3.0 MB (2957815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1607240ca884b25e20b8db8c53c4aea519b76a50e23c19a40aaadd508939589`  
		Last Modified: Tue, 02 Aug 2022 20:13:35 GMT  
		Size: 129.1 MB (129092301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb38c444df15407ab436886281e04c48950509ec0de9d9bc5203e14640165ddb`  
		Last Modified: Wed, 03 Aug 2022 14:15:54 GMT  
		Size: 14.1 MB (14085453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05aa53415f32b814deebc075a7bb595df58d79cf67a5fe218c1cd111e5b6ee0a`  
		Last Modified: Wed, 03 Aug 2022 14:15:50 GMT  
		Size: 679.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ddbf21b719f1a92ad3ee2ffed35afb7f2c0836d372a03e8ef6c86bc5546c4a`  
		Last Modified: Wed, 03 Aug 2022 14:15:50 GMT  
		Size: 9.8 KB (9757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5492e88c0d013bf0d79353e5c81b4167fe2b1aa74465b5c05edbf3b14658858a`  
		Last Modified: Wed, 03 Aug 2022 14:15:50 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f086c2ef5ce4893aeade47c11c788a8992b4e43bfa5e8316e9a13a422acb4b06`  
		Last Modified: Wed, 03 Aug 2022 14:15:50 GMT  
		Size: 10.7 KB (10735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3191d937acd525f20b08c085e17bb91eb22cf727d6199fd8049c53e3332a232`  
		Last Modified: Wed, 03 Aug 2022 14:15:51 GMT  
		Size: 5.7 MB (5702881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:d4b84c94d6be89b9404d44c13acf3d3ff5fec9d0d5d7d11821cc8b0186c2fd02
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.9 MB (181928476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a8aabaa6b07007819fd03084677523cb5f56c68083e93341cadd61df694d6ce`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:49:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 07 Jun 2022 08:50:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 18:31:53 GMT
ENV JAVA_VERSION=8.0.7.11
# Wed, 29 Jun 2022 18:33:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 29 Jun 2022 18:33:35 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 29 Jun 2022 19:03:57 GMT
ARG VERBOSE=false
# Wed, 29 Jun 2022 19:04:05 GMT
ARG OPENJ9_SCC=true
# Wed, 29 Jun 2022 19:04:16 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 29 Jun 2022 19:04:32 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 29 Jun 2022 19:04:39 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 29 Jun 2022 19:04:46 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 29 Jun 2022 19:04:53 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 29 Jun 2022 19:04:57 GMT
ARG LIBERTY_URL
# Wed, 29 Jun 2022 19:05:02 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 29 Jun 2022 19:06:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 19:06:54 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Jun 2022 19:06:59 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 29 Jun 2022 19:07:04 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 29 Jun 2022 19:07:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 29 Jun 2022 19:07:22 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 29 Jun 2022 19:07:27 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 29 Jun 2022 19:07:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 29 Jun 2022 19:08:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 29 Jun 2022 19:08:16 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 29 Jun 2022 19:08:20 GMT
USER 1001
# Wed, 29 Jun 2022 19:08:28 GMT
EXPOSE 9080 9443
# Wed, 29 Jun 2022 19:08:35 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 29 Jun 2022 19:08:44 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4a22aedc3b9f2593635b0a3f6fe64e6dd424850b9782f66e88c8c162926d6a`  
		Last Modified: Tue, 07 Jun 2022 08:54:16 GMT  
		Size: 3.1 MB (3082521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448aed354e59dc01b7da997655c86778001067ef107a5c1fb36a7c38fcf5fdda`  
		Last Modified: Wed, 29 Jun 2022 18:38:02 GMT  
		Size: 128.6 MB (128629743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ee64dfa956bec7a3911c4fbcec85677da5eb3557fdd1fad0cd05371b418ed3`  
		Last Modified: Wed, 29 Jun 2022 19:36:18 GMT  
		Size: 14.4 MB (14414087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f44198605bccf1a3fd327e2929165c362826698ef117c8ed5e5f61cf8471cce`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 685.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8008efd74eeabae4093e325cb3ee9f17c49e27f7dbb19564636c92acb9051471`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 9.8 KB (9757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df8e4e4d330f9771962db9ea9c4da8f370e92f1745f117e9db5baae643dfff3`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa888647a678f768a7a68d44ee29bc98b5834e1d4b43481f1d79fb22ae798d8`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 10.7 KB (10748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24233765490b95aea52162ad51e9982a4c6bd67895d93467ca629ea8bfb5a68`  
		Last Modified: Wed, 29 Jun 2022 19:36:15 GMT  
		Size: 5.3 MB (5337804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:311be6c24f4d54b605d3f60376debefcefe5db4fa5dffe4f0b853a68cd8d071f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.2 MB (174181742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba9247e8964bc01dc0c736aee5e2e2f6a718ee1017f272f2b918c7b93a98c542`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:01:57 GMT
ADD file:3d2e9b401524527b395347bc3847be7c9cb465b9a214a1a1d31e74330e293c45 in / 
# Tue, 02 Aug 2022 01:01:58 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 13:19:12 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 02 Aug 2022 13:19:25 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:19:25 GMT
ENV JAVA_VERSION=8.0.7.11
# Tue, 02 Aug 2022 13:20:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 02 Aug 2022 13:20:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 03 Aug 2022 00:30:47 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:30:48 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:30:48 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 00:30:48 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 00:30:48 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 00:30:49 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 00:30:49 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 00:30:49 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 00:30:49 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 00:31:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 00:31:03 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 00:31:03 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 00:31:03 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:31:06 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 00:31:07 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 00:31:07 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 00:31:08 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 00:31:17 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 00:31:18 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 03 Aug 2022 00:31:18 GMT
USER 1001
# Wed, 03 Aug 2022 00:31:18 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 00:31:18 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 00:31:19 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:be3ed498266c519f84268ff1f02085fa249c0e32fb60a59466e24c862b5f094b`  
		Last Modified: Tue, 02 Aug 2022 01:03:25 GMT  
		Size: 25.4 MB (25369584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2ed0adcefe11b30e3dff027bcb1cb9fe759f39f50b008bafb3644d3d2fcba8`  
		Last Modified: Tue, 02 Aug 2022 13:22:41 GMT  
		Size: 2.7 MB (2671706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745854ef92308f8e24873e2cf64eb998c725371b7d10ba8318989b37bba26f33`  
		Last Modified: Tue, 02 Aug 2022 13:22:49 GMT  
		Size: 126.1 MB (126143967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a59a661cbbb2b8555a22d1f6e2943fbf1eaa8381c6a30030ac4c3276c7cf1e8`  
		Last Modified: Wed, 03 Aug 2022 01:21:11 GMT  
		Size: 14.1 MB (14085532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19a28dc7880331492105ef80fe1628f9d15c71bc959cd9765cdcd64a139c472`  
		Last Modified: Wed, 03 Aug 2022 01:21:09 GMT  
		Size: 679.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc961a105d81f315d8af16fb228d90842f45dd9ff3a0ce06580d31bf5ae346c3`  
		Last Modified: Wed, 03 Aug 2022 01:21:09 GMT  
		Size: 9.8 KB (9763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07467c7f0c1b48d655b4ff47a1a5101cb4f28e77adce3d47f9c5bfaaaa1968a7`  
		Last Modified: Wed, 03 Aug 2022 01:21:08 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55abb9ff522a8f086c734b47a7b69b3d2770c58ec832b8d992f7e67766700ca8`  
		Last Modified: Wed, 03 Aug 2022 01:21:09 GMT  
		Size: 10.7 KB (10735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4009dc9f786bc5ce10ba8ebf96892fd74d20c3548ff8acc69160e27dcb3a615`  
		Last Modified: Wed, 03 Aug 2022 01:21:09 GMT  
		Size: 5.9 MB (5889501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:be2eae562c627321465756db2cb0fdaa4730028432e4a05f0c8c46ca32edfd8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:kernel-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:236bd357c37f0f21b7adff989a4dab6e6aadd5af1780f2e5b9f5ef684d159d28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113217145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:519b9356f1ab3952e988d47b506fd3a838137be4c4b0a6c9539a7f7c969c91e9`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 19:04:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 19:05:01 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 19:56:56 GMT
ENV JAVA_VERSION=jdk-11.0.15+10_openj9-0.32.0
# Tue, 02 Aug 2022 19:58:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69e4a0b383c7b4187478ddb196de3cdc91560e2be40b8ef66354591e87c36e85';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5e82f7df54786c557d2d9e9ac22df655fd94b9702c73261390903ac87532d545';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='25d4d5e2bbe3eb19bcb9a76aec4b43d4eef5ad66200df3122118f69da5325cf6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='def85f1b00e9c65a8c3b5dcf4da0f1b04c17675b4ff9cd6f5dad61d8dcbd03d0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 19:58:02 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 19:58:02 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 19:58:37 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 13:23:06 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:23:06 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:23:06 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 13:23:06 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 13:23:06 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 13:23:06 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 13:23:07 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 13:23:07 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 13:23:07 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 13:23:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 13:23:20 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 13:23:20 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 13:23:20 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:23:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 13:23:21 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 13:23:21 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 13:23:22 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 13:23:29 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 13:23:29 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 13:23:29 GMT
USER 1001
# Wed, 03 Aug 2022 13:23:29 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 13:23:29 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 13:23:29 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:a84b3718e4bf43f94609ec6fedf833567945fd97d9b8c324995df295d627fbb7`  
		Last Modified: Tue, 02 Aug 2022 20:06:46 GMT  
		Size: 47.7 MB (47691482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c02c82f8c35f778ae48a325cbccf65292ecbdea6e70272147ca65f72cda4dd`  
		Last Modified: Tue, 02 Aug 2022 20:06:39 GMT  
		Size: 4.2 MB (4183653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f41d289bc930a3a92caf3a90f84db2362a42680dd7ce48a2e1befa89078e3d`  
		Last Modified: Wed, 03 Aug 2022 14:16:04 GMT  
		Size: 14.2 MB (14183927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe3d80467e0f8bbeb61b656c7c4ed7ce644a4d1c7eab501f1b6a0e7fe8375b4`  
		Last Modified: Wed, 03 Aug 2022 14:16:00 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b9afcc7c926f3a529e2ea516fde829c98dbefe91c9d6f6ad3da2566ac205aff`  
		Last Modified: Wed, 03 Aug 2022 14:16:00 GMT  
		Size: 9.8 KB (9754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1691ca21cc220ab5c388a3736a7d146f33ae925532fb1608e128ef9b5d0bae8`  
		Last Modified: Wed, 03 Aug 2022 14:16:00 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a698c8b450bdc7160dc4aec60aec1b5bf12d3eba41cacac8016a21efc396f6`  
		Last Modified: Wed, 03 Aug 2022 14:16:00 GMT  
		Size: 10.7 KB (10731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d3164f01d38ac4bfa365542bbba93799c6f0fdd8ac6a8ae099ff4b510397a5`  
		Last Modified: Wed, 03 Aug 2022 14:16:01 GMT  
		Size: 2.5 MB (2534099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:6d35cf4b76f82fa41cd99fb78d6adbc77fd06a4a15bb2873d7a9a71ae50836cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.3 MB (119269912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a92fab9e70bea7e1a9541da717f0c50e9fd2ce6e1f66b833f8daf8666f38fdc`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 07:16:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 07:18:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:46:26 GMT
ENV JAVA_VERSION=jdk-11.0.15+10_openj9-0.32.0
# Tue, 07 Jun 2022 09:48:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69e4a0b383c7b4187478ddb196de3cdc91560e2be40b8ef66354591e87c36e85';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5e82f7df54786c557d2d9e9ac22df655fd94b9702c73261390903ac87532d545';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='25d4d5e2bbe3eb19bcb9a76aec4b43d4eef5ad66200df3122118f69da5325cf6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='def85f1b00e9c65a8c3b5dcf4da0f1b04c17675b4ff9cd6f5dad61d8dcbd03d0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 09:48:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 09:48:28 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 07 Jun 2022 09:49:12 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 07 Jun 2022 11:28:13 GMT
ARG VERBOSE=false
# Tue, 07 Jun 2022 11:28:23 GMT
ARG OPENJ9_SCC=true
# Mon, 27 Jun 2022 19:05:58 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Mon, 27 Jun 2022 19:06:02 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Mon, 27 Jun 2022 19:06:05 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Mon, 27 Jun 2022 19:06:10 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 27 Jun 2022 19:06:13 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Mon, 27 Jun 2022 19:06:17 GMT
ARG LIBERTY_URL
# Mon, 27 Jun 2022 19:06:22 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 27 Jun 2022 19:07:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 27 Jun 2022 19:07:15 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Jun 2022 19:07:20 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Mon, 27 Jun 2022 19:07:23 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 27 Jun 2022 19:07:30 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 27 Jun 2022 19:07:32 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Mon, 27 Jun 2022 19:07:33 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 27 Jun 2022 19:07:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 27 Jun 2022 19:07:55 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 27 Jun 2022 19:07:57 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Mon, 27 Jun 2022 19:08:01 GMT
USER 1001
# Mon, 27 Jun 2022 19:08:05 GMT
EXPOSE 9080 9443
# Mon, 27 Jun 2022 19:08:08 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 27 Jun 2022 19:08:10 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6c621e52fdf1e59e073b1c51c52e2e5a829be92510ef56949c609a03af2492`  
		Last Modified: Tue, 07 Jun 2022 07:30:19 GMT  
		Size: 17.2 MB (17203633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06eb9350ab17a87b8e47ac6a3389da7e21786ee038077cf7b627f90b125f1acf`  
		Last Modified: Tue, 07 Jun 2022 10:01:58 GMT  
		Size: 48.4 MB (48378487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc0d65d22cb0b40edcecacc4b8c684bc4bf1ddc89b24fd16e7abefba2b0c7df`  
		Last Modified: Tue, 07 Jun 2022 10:01:49 GMT  
		Size: 3.3 MB (3334009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5ff26c4cf89eaa05313a18d91d7309df617938eb84d02061347a609a33a7b8`  
		Last Modified: Mon, 27 Jun 2022 20:21:41 GMT  
		Size: 14.5 MB (14515853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ccfddb3da6a003c78fba8f80fd75c65f4fc295e3cc5bdf38bacf9e33c4844f`  
		Last Modified: Mon, 27 Jun 2022 20:21:32 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e827be780b6a43a9e9798fec11910f661a036eb43e9b207bd5a09dc0931e9b`  
		Last Modified: Mon, 27 Jun 2022 20:21:32 GMT  
		Size: 9.8 KB (9751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79a0d64d22b6a5861752d66f9cef744682bef6f31b78ac467d9065fadc0587c`  
		Last Modified: Mon, 27 Jun 2022 20:21:32 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93afd12b58a928c66cb4067a1a977a97bc0dacfe201dc9ad79c4800176e8cca`  
		Last Modified: Mon, 27 Jun 2022 20:21:32 GMT  
		Size: 10.7 KB (10734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210f9edeb69d5d47378b5b0de8220cb51a99548682efd824bb4fc5dce63089c3`  
		Last Modified: Mon, 27 Jun 2022 20:21:33 GMT  
		Size: 2.5 MB (2522136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:0f4e2e03e7d5dbe6876dfb2c896c099cfb95a09b614bf2545aa10721cd0eb89e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110565665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4769a9a75c92ec85d9c8cd0a11812c5d4025e00ed223ebfe7cd8a0db797c0da7`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:41:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 12:41:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:43:42 GMT
ENV JAVA_VERSION=jdk-11.0.15+10_openj9-0.32.0
# Tue, 02 Aug 2022 12:44:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69e4a0b383c7b4187478ddb196de3cdc91560e2be40b8ef66354591e87c36e85';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5e82f7df54786c557d2d9e9ac22df655fd94b9702c73261390903ac87532d545';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='25d4d5e2bbe3eb19bcb9a76aec4b43d4eef5ad66200df3122118f69da5325cf6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='def85f1b00e9c65a8c3b5dcf4da0f1b04c17675b4ff9cd6f5dad61d8dcbd03d0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 12:44:51 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 12:44:51 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 12:45:24 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 00:31:25 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:31:25 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:31:25 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 00:31:25 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 00:31:25 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 00:31:26 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 00:31:26 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 00:31:26 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 00:31:26 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 00:31:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 00:31:38 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 00:31:38 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 00:31:38 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:31:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 00:31:39 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 00:31:39 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 00:31:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 00:31:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 00:31:46 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 00:31:46 GMT
USER 1001
# Wed, 03 Aug 2022 00:31:47 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 00:31:47 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 00:31:47 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:3f28b38375577480d13a8d78bab4c30073086c8a51a4ff217f32365aa0847411`  
		Last Modified: Tue, 02 Aug 2022 12:53:12 GMT  
		Size: 46.7 MB (46721680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3142744ed0637685528da62bbcb28da17d0b48fdc151bd52e7b22274eeb2c5da`  
		Last Modified: Tue, 02 Aug 2022 12:53:07 GMT  
		Size: 4.3 MB (4313565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9e7b387efd480990d6c64a866fba64fb104280672f530db487652f6a8b2420`  
		Last Modified: Wed, 03 Aug 2022 01:21:19 GMT  
		Size: 14.2 MB (14184080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d846195251009f85f9e3322ee32d4f6714c2208a979e2878e07e74634075b2`  
		Last Modified: Wed, 03 Aug 2022 01:21:17 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a4da3cc546eda0832bbac5eea20e393ef5335b890a0401290b55655e909ae4`  
		Last Modified: Wed, 03 Aug 2022 01:21:17 GMT  
		Size: 9.8 KB (9753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc9ec89f07bd2ea2472397191fdaf70131a284380baa496449e81346c8f9e97`  
		Last Modified: Wed, 03 Aug 2022 01:21:17 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6edb8309c1fef9cc240f64d15d2875b926152ce9f44aa1e3a2fa26b7eacecb`  
		Last Modified: Wed, 03 Aug 2022 01:21:16 GMT  
		Size: 10.7 KB (10726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c61c79763634b9154ab44813cd5f16fac38e3a947bc0e0a208f3468ae4c3910`  
		Last Modified: Wed, 03 Aug 2022 01:21:18 GMT  
		Size: 2.5 MB (2549406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:kernel-java17-openj9`

```console
$ docker pull websphere-liberty@sha256:e0544fe0929c36917d1641597cdc03bdcf16626d2be3e9c2c4525e10310e8390
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:kernel-java17-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:45d0cb42a4ca31d7a0b7c3a9c08bdff54d901e3a02f5035e27c128bb4e031b5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113855947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ca8e945cab711ceb4b45dae42e16abb300f5977010c6022309c35e48d9727bc`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 19:04:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 19:05:01 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:00:47 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Tue, 02 Aug 2022 20:02:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f899948ea0c5dc80a66f801db585939a25a4ae7e1f21a9a8f3bf3749c3baa87f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9c54166490ac55a6bd26249b57eae5df4531635f4871e6642e7979affc894875';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='dad35fec82047e3a82c6e2dda8b53ee763b55aaedaed13b7b130856f4a3ffd35';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='4e2f631ad18c288e419db5c35295829dd7e83f4cd1be95252db06eb622b23090';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 20:02:05 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 20:02:05 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 20:02:40 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 13:23:34 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:23:34 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:23:34 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 13:23:34 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 13:23:35 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 13:23:35 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 13:23:35 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 13:23:35 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 13:23:35 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 13:23:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 13:23:48 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 13:23:48 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 13:23:48 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:23:49 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 13:23:49 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 13:23:49 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 13:23:50 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 13:23:57 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 13:23:57 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 13:23:57 GMT
USER 1001
# Wed, 03 Aug 2022 13:23:57 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 13:23:58 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 13:23:58 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:7b6279e9931cb0efc3b60659be8fd46c95156f958f00818850fba3ac0ecd0616`  
		Last Modified: Tue, 02 Aug 2022 20:08:11 GMT  
		Size: 47.8 MB (47754438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e834be70bdf636e5c875d9e2badbf281d32ff675b9eb7db8768a2da9dbdf5e`  
		Last Modified: Tue, 02 Aug 2022 20:08:05 GMT  
		Size: 4.7 MB (4744099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b29111272e76b623f6a1c705052b79e4aed2ed08bb404f433fd8a20cd7c752`  
		Last Modified: Wed, 03 Aug 2022 14:16:14 GMT  
		Size: 14.2 MB (14183924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6606826ea4776a63f20adb28aca4a26e64d000ea040af34471de8c2366784452`  
		Last Modified: Wed, 03 Aug 2022 14:16:11 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa6ada95f6df02ffacedde72e53786a3bc150cc4bf94f7861f91a2cb9e026b0`  
		Last Modified: Wed, 03 Aug 2022 14:16:11 GMT  
		Size: 9.7 KB (9749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9521245474cad0537df9cfe305a8f740cb08a15941eea9bbd4b6d48ca6f91cd7`  
		Last Modified: Wed, 03 Aug 2022 14:16:11 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3f9ef840580663cf3012d2a8a7d7b03dab23484c4e62f2eba0004d6f4adaa`  
		Last Modified: Wed, 03 Aug 2022 14:16:11 GMT  
		Size: 10.7 KB (10725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f946b913fac313fce2c6d202c5ea9c9da8039c23dda2c638d1035e62305bc81`  
		Last Modified: Wed, 03 Aug 2022 14:16:11 GMT  
		Size: 2.5 MB (2549516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java17-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:e07434f05a0ce037deb7160f615fd2c70ac87cd34fe541dfb1376ab0c729e822
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.4 MB (119366206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22291564784ba272c1f2bc0584e564e4bf1b4d7e1a1f88c7d48c94972dc2b219`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 07:16:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 07:18:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:52:39 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Tue, 07 Jun 2022 09:54:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f899948ea0c5dc80a66f801db585939a25a4ae7e1f21a9a8f3bf3749c3baa87f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9c54166490ac55a6bd26249b57eae5df4531635f4871e6642e7979affc894875';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='dad35fec82047e3a82c6e2dda8b53ee763b55aaedaed13b7b130856f4a3ffd35';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='4e2f631ad18c288e419db5c35295829dd7e83f4cd1be95252db06eb622b23090';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 09:54:20 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 09:54:22 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 07 Jun 2022 09:55:03 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 07 Jun 2022 11:31:51 GMT
ARG VERBOSE=false
# Tue, 07 Jun 2022 11:31:54 GMT
ARG OPENJ9_SCC=true
# Mon, 27 Jun 2022 19:08:20 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Mon, 27 Jun 2022 19:08:23 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Mon, 27 Jun 2022 19:08:26 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Mon, 27 Jun 2022 19:08:29 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 27 Jun 2022 19:08:32 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Mon, 27 Jun 2022 19:08:33 GMT
ARG LIBERTY_URL
# Mon, 27 Jun 2022 19:08:37 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 27 Jun 2022 19:09:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 27 Jun 2022 19:09:29 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Jun 2022 19:09:31 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Mon, 27 Jun 2022 19:09:32 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 27 Jun 2022 19:09:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Mon, 27 Jun 2022 19:09:42 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Mon, 27 Jun 2022 19:09:43 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 27 Jun 2022 19:09:52 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 27 Jun 2022 19:10:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 27 Jun 2022 19:10:11 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Mon, 27 Jun 2022 19:10:14 GMT
USER 1001
# Mon, 27 Jun 2022 19:10:17 GMT
EXPOSE 9080 9443
# Mon, 27 Jun 2022 19:10:18 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 27 Jun 2022 19:10:23 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6c621e52fdf1e59e073b1c51c52e2e5a829be92510ef56949c609a03af2492`  
		Last Modified: Tue, 07 Jun 2022 07:30:19 GMT  
		Size: 17.2 MB (17203633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643e82d1f37eb2778986afcd7aa289e4f42b3c21d19b6dc2b50320f2836d580e`  
		Last Modified: Tue, 07 Jun 2022 10:03:59 GMT  
		Size: 48.1 MB (48115319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe972a29b91980b448bef8b1d66c53f248a582f57eb8476283dad120863f562`  
		Last Modified: Tue, 07 Jun 2022 10:03:52 GMT  
		Size: 3.7 MB (3691417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c056cb98358395a411cf5384fbbdbec5ccfd5f81859801ac0c85148bbb98a4`  
		Last Modified: Mon, 27 Jun 2022 20:22:00 GMT  
		Size: 14.5 MB (14515851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd06b09fbbdc503b03e823a42d86309633c6d84767fa73330825bc907e14df3`  
		Last Modified: Mon, 27 Jun 2022 20:21:51 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbb19c1ede5ad19ca10791cc60a2f22dd80c54475f408a0e73abdccbca16792`  
		Last Modified: Mon, 27 Jun 2022 20:21:51 GMT  
		Size: 9.8 KB (9753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948cca84307d534dd3b66a3ccd42411c24283967d6c73d87983819647f564e0c`  
		Last Modified: Mon, 27 Jun 2022 20:21:51 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39dcdc56c341ef84605200c2bc492ee7ebd2d7d6c088f9188b4b724f2316504`  
		Last Modified: Mon, 27 Jun 2022 20:21:51 GMT  
		Size: 10.7 KB (10740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdde75f3ce0ceab51ecdf4a88f513912d5744afccff705acaa98d4d96a9399d1`  
		Last Modified: Mon, 27 Jun 2022 20:21:52 GMT  
		Size: 2.5 MB (2524189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java17-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:c62c52f84546bd642194fb4433c49285d544ec2cd2f24248cca8005d22f5f795
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110744273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6eec6e01d0a5f110955696012d2ebe0ad4a9e76851e0e127c93e62daf1ad5f3`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:41:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 12:41:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:47:17 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Tue, 02 Aug 2022 12:48:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f899948ea0c5dc80a66f801db585939a25a4ae7e1f21a9a8f3bf3749c3baa87f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9c54166490ac55a6bd26249b57eae5df4531635f4871e6642e7979affc894875';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='dad35fec82047e3a82c6e2dda8b53ee763b55aaedaed13b7b130856f4a3ffd35';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='4e2f631ad18c288e419db5c35295829dd7e83f4cd1be95252db06eb622b23090';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 12:48:20 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 12:48:20 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 02 Aug 2022 12:48:53 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 03 Aug 2022 00:31:56 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:31:56 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:31:56 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 00:31:57 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 00:31:57 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 00:31:57 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 00:31:57 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 00:31:57 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 00:31:57 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 00:32:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 00:32:08 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 00:32:08 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 00:32:08 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:32:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 00:32:09 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 00:32:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 00:32:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 00:32:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 00:32:16 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 03 Aug 2022 00:32:16 GMT
USER 1001
# Wed, 03 Aug 2022 00:32:16 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 00:32:17 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 00:32:17 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:8366f0be07eee724257935ccff074ac6069837c38e228be50a0b6f2e058ab16c`  
		Last Modified: Tue, 02 Aug 2022 12:54:24 GMT  
		Size: 46.2 MB (46241889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc471632f4e136d4fa45d0a7216573974cc332f3e9fa969846cb74f259e5e9cc`  
		Last Modified: Tue, 02 Aug 2022 12:54:19 GMT  
		Size: 4.9 MB (4939140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88edf1255c796274783dd2b408dda42ea663cad4b64810259c6acc1259419aa0`  
		Last Modified: Wed, 03 Aug 2022 01:21:26 GMT  
		Size: 14.2 MB (14184036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353a76e46cfbb610eda04921de105adf89120c8930d1974118798f627627b68b`  
		Last Modified: Wed, 03 Aug 2022 01:21:24 GMT  
		Size: 688.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfabfad0e607d1360481e4e76a8538189f1d761829c85652481cc8110f7abd2`  
		Last Modified: Wed, 03 Aug 2022 01:21:24 GMT  
		Size: 9.8 KB (9755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1851082a958effaac3cac4eddcea238e723fb008a9460dc32982226790cf22`  
		Last Modified: Wed, 03 Aug 2022 01:21:24 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3260426547d5393a73a84720e7ff09a76a39680394581d9c50107cb7f6f2489f`  
		Last Modified: Wed, 03 Aug 2022 01:21:24 GMT  
		Size: 10.7 KB (10734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fef24753132b515d30c6966531a9a4e35f7b4cc2441ecbe77dcaf61055f2ce0`  
		Last Modified: Wed, 03 Aug 2022 01:21:25 GMT  
		Size: 2.6 MB (2582268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:latest`

```console
$ docker pull websphere-liberty@sha256:3a27bdeb56129c14e7bd4a664be6774a78b910e3d5203d585e55a23137c7c009
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:latest` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:886abf89eb3316d1fa1e344b1c566b12c8c56dbdfe67ef1ab450f516026e19ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **461.9 MB (461889376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90501b5e0a18925bbd8d499cd561137878b9b24d6b69dcb7f15f4ad327d68c64`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 20:09:52 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 02 Aug 2022 20:10:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 20:10:01 GMT
ENV JAVA_VERSION=8.0.7.11
# Tue, 02 Aug 2022 20:10:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 02 Aug 2022 20:10:53 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 03 Aug 2022 13:22:32 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:22:32 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:22:32 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 13:22:33 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 13:22:33 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 13:22:33 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 13:22:33 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 13:22:33 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 13:22:33 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 13:22:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 13:22:51 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 13:22:51 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 13:22:51 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 13:22:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 13:22:53 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 13:22:53 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 13:22:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 13:23:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 13:23:02 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 03 Aug 2022 13:23:03 GMT
USER 1001
# Wed, 03 Aug 2022 13:23:03 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 13:23:03 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 13:23:03 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 03 Aug 2022 13:24:02 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 13:24:02 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 03 Aug 2022 13:31:35 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 03 Aug 2022 13:31:36 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 03 Aug 2022 13:32:07 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6715a1bb89fcf5e91403be2bc6130f23e6b3cfd0da73e6b09e937d028409d3`  
		Last Modified: Tue, 02 Aug 2022 20:13:24 GMT  
		Size: 3.0 MB (2957815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1607240ca884b25e20b8db8c53c4aea519b76a50e23c19a40aaadd508939589`  
		Last Modified: Tue, 02 Aug 2022 20:13:35 GMT  
		Size: 129.1 MB (129092301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb38c444df15407ab436886281e04c48950509ec0de9d9bc5203e14640165ddb`  
		Last Modified: Wed, 03 Aug 2022 14:15:54 GMT  
		Size: 14.1 MB (14085453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05aa53415f32b814deebc075a7bb595df58d79cf67a5fe218c1cd111e5b6ee0a`  
		Last Modified: Wed, 03 Aug 2022 14:15:50 GMT  
		Size: 679.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ddbf21b719f1a92ad3ee2ffed35afb7f2c0836d372a03e8ef6c86bc5546c4a`  
		Last Modified: Wed, 03 Aug 2022 14:15:50 GMT  
		Size: 9.8 KB (9757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5492e88c0d013bf0d79353e5c81b4167fe2b1aa74465b5c05edbf3b14658858a`  
		Last Modified: Wed, 03 Aug 2022 14:15:50 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f086c2ef5ce4893aeade47c11c788a8992b4e43bfa5e8316e9a13a422acb4b06`  
		Last Modified: Wed, 03 Aug 2022 14:15:50 GMT  
		Size: 10.7 KB (10735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3191d937acd525f20b08c085e17bb91eb22cf727d6199fd8049c53e3332a232`  
		Last Modified: Wed, 03 Aug 2022 14:15:51 GMT  
		Size: 5.7 MB (5702881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17cdf033149a3de277684874263c1eb2bedf5f30eb0a4012432b12def4c7822`  
		Last Modified: Wed, 03 Aug 2022 14:16:36 GMT  
		Size: 267.1 MB (267144319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10376ddb37d6232ae5252c9bdf6f04422f9557849cd611df7d58c8bf1185eede`  
		Last Modified: Wed, 03 Aug 2022 14:16:21 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5c901d7e4747e67d324ddb82affbf24e080a953b3ce5ed31ad1504258d171a`  
		Last Modified: Wed, 03 Aug 2022 14:16:24 GMT  
		Size: 16.2 MB (16173947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:20b8c8568ac1ace5302e32de4580705070ad867b1267fc10eddecc0342efb233
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.1 MB (463103256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24bec26d5b6e33bfa1465f31c5486fb46d341b64a8a89ebecee746a78fd2086b`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:49:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 07 Jun 2022 08:50:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 18:31:53 GMT
ENV JAVA_VERSION=8.0.7.11
# Wed, 29 Jun 2022 18:33:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 29 Jun 2022 18:33:35 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 29 Jun 2022 19:03:57 GMT
ARG VERBOSE=false
# Wed, 29 Jun 2022 19:04:05 GMT
ARG OPENJ9_SCC=true
# Wed, 29 Jun 2022 19:04:16 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 29 Jun 2022 19:04:32 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 29 Jun 2022 19:04:39 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 29 Jun 2022 19:04:46 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 29 Jun 2022 19:04:53 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 29 Jun 2022 19:04:57 GMT
ARG LIBERTY_URL
# Wed, 29 Jun 2022 19:05:02 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 29 Jun 2022 19:06:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 19:06:54 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Jun 2022 19:06:59 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 29 Jun 2022 19:07:04 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 29 Jun 2022 19:07:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 29 Jun 2022 19:07:22 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 29 Jun 2022 19:07:27 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 29 Jun 2022 19:07:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 29 Jun 2022 19:08:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 29 Jun 2022 19:08:16 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 29 Jun 2022 19:08:20 GMT
USER 1001
# Wed, 29 Jun 2022 19:08:28 GMT
EXPOSE 9080 9443
# Wed, 29 Jun 2022 19:08:35 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 29 Jun 2022 19:08:44 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 29 Jun 2022 19:09:19 GMT
ARG VERBOSE=false
# Wed, 29 Jun 2022 19:09:27 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 29 Jun 2022 19:18:40 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 29 Jun 2022 19:18:47 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 29 Jun 2022 19:19:57 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4a22aedc3b9f2593635b0a3f6fe64e6dd424850b9782f66e88c8c162926d6a`  
		Last Modified: Tue, 07 Jun 2022 08:54:16 GMT  
		Size: 3.1 MB (3082521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448aed354e59dc01b7da997655c86778001067ef107a5c1fb36a7c38fcf5fdda`  
		Last Modified: Wed, 29 Jun 2022 18:38:02 GMT  
		Size: 128.6 MB (128629743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ee64dfa956bec7a3911c4fbcec85677da5eb3557fdd1fad0cd05371b418ed3`  
		Last Modified: Wed, 29 Jun 2022 19:36:18 GMT  
		Size: 14.4 MB (14414087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f44198605bccf1a3fd327e2929165c362826698ef117c8ed5e5f61cf8471cce`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 685.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8008efd74eeabae4093e325cb3ee9f17c49e27f7dbb19564636c92acb9051471`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 9.8 KB (9757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df8e4e4d330f9771962db9ea9c4da8f370e92f1745f117e9db5baae643dfff3`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa888647a678f768a7a68d44ee29bc98b5834e1d4b43481f1d79fb22ae798d8`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 10.7 KB (10748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24233765490b95aea52162ad51e9982a4c6bd67895d93467ca629ea8bfb5a68`  
		Last Modified: Wed, 29 Jun 2022 19:36:15 GMT  
		Size: 5.3 MB (5337804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a597fe1c695442d024092e9ba428ea88ffa886c912a199fbe492b776a53a7595`  
		Last Modified: Wed, 29 Jun 2022 19:36:52 GMT  
		Size: 267.1 MB (267144840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165a7c33a3339f487205b064950b8fb81222d47d74c6fdfef158d7464150dbbb`  
		Last Modified: Wed, 29 Jun 2022 19:36:29 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ede9c741b2ef54fc67a38aab455cdc0ef8bea790cfdf300b7e1d01aa4486ec`  
		Last Modified: Wed, 29 Jun 2022 19:36:35 GMT  
		Size: 14.0 MB (14028991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:f6b028efccb8a1d3a8e7633ab097afc5ef7ea9eb145ecff4d148ebf489240309
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **457.5 MB (457473936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52b2b35b4ae3c6168a008c1dd5dccb115e7bc94a70e161ac19b8340a87a722b7`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:01:57 GMT
ADD file:3d2e9b401524527b395347bc3847be7c9cb465b9a214a1a1d31e74330e293c45 in / 
# Tue, 02 Aug 2022 01:01:58 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 13:19:12 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 02 Aug 2022 13:19:25 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:19:25 GMT
ENV JAVA_VERSION=8.0.7.11
# Tue, 02 Aug 2022 13:20:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 02 Aug 2022 13:20:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 03 Aug 2022 00:30:47 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:30:48 GMT
ARG OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:30:48 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 03 Aug 2022 00:30:48 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 03 Aug 2022 00:30:48 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 03 Aug 2022 00:30:49 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 03 Aug 2022 00:30:49 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 03 Aug 2022 00:30:49 GMT
ARG LIBERTY_URL
# Wed, 03 Aug 2022 00:30:49 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 03 Aug 2022 00:31:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 00:31:03 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 00:31:03 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 03 Aug 2022 00:31:03 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 03 Aug 2022 00:31:06 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 03 Aug 2022 00:31:07 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 03 Aug 2022 00:31:07 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 03 Aug 2022 00:31:08 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 03 Aug 2022 00:31:17 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 03 Aug 2022 00:31:18 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 03 Aug 2022 00:31:18 GMT
USER 1001
# Wed, 03 Aug 2022 00:31:18 GMT
EXPOSE 9080 9443
# Wed, 03 Aug 2022 00:31:18 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 03 Aug 2022 00:31:19 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 03 Aug 2022 00:32:24 GMT
ARG VERBOSE=false
# Wed, 03 Aug 2022 00:32:24 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 03 Aug 2022 00:39:41 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 03 Aug 2022 00:40:02 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 03 Aug 2022 00:40:42 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:be3ed498266c519f84268ff1f02085fa249c0e32fb60a59466e24c862b5f094b`  
		Last Modified: Tue, 02 Aug 2022 01:03:25 GMT  
		Size: 25.4 MB (25369584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2ed0adcefe11b30e3dff027bcb1cb9fe759f39f50b008bafb3644d3d2fcba8`  
		Last Modified: Tue, 02 Aug 2022 13:22:41 GMT  
		Size: 2.7 MB (2671706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745854ef92308f8e24873e2cf64eb998c725371b7d10ba8318989b37bba26f33`  
		Last Modified: Tue, 02 Aug 2022 13:22:49 GMT  
		Size: 126.1 MB (126143967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a59a661cbbb2b8555a22d1f6e2943fbf1eaa8381c6a30030ac4c3276c7cf1e8`  
		Last Modified: Wed, 03 Aug 2022 01:21:11 GMT  
		Size: 14.1 MB (14085532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19a28dc7880331492105ef80fe1628f9d15c71bc959cd9765cdcd64a139c472`  
		Last Modified: Wed, 03 Aug 2022 01:21:09 GMT  
		Size: 679.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc961a105d81f315d8af16fb228d90842f45dd9ff3a0ce06580d31bf5ae346c3`  
		Last Modified: Wed, 03 Aug 2022 01:21:09 GMT  
		Size: 9.8 KB (9763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07467c7f0c1b48d655b4ff47a1a5101cb4f28e77adce3d47f9c5bfaaaa1968a7`  
		Last Modified: Wed, 03 Aug 2022 01:21:08 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55abb9ff522a8f086c734b47a7b69b3d2770c58ec832b8d992f7e67766700ca8`  
		Last Modified: Wed, 03 Aug 2022 01:21:09 GMT  
		Size: 10.7 KB (10735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4009dc9f786bc5ce10ba8ebf96892fd74d20c3548ff8acc69160e27dcb3a615`  
		Last Modified: Wed, 03 Aug 2022 01:21:09 GMT  
		Size: 5.9 MB (5889501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e27310727e03cbd34d78cf4d4b95a8e316a4b322be112db401ab8c19e495739`  
		Last Modified: Wed, 03 Aug 2022 01:21:43 GMT  
		Size: 267.1 MB (267143557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7fa949e35b734374f99454dc3a7a9f7dba0a28dd865c7ca9514f169950d991`  
		Last Modified: Wed, 03 Aug 2022 01:21:31 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3f51986dc9d010c1551d1d44b8efb475ea65824d2ae8e3fba9476278e13ff0`  
		Last Modified: Wed, 03 Aug 2022 01:21:33 GMT  
		Size: 16.1 MB (16147687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
