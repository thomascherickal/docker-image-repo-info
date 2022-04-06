<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `websphere-liberty`

-	[`websphere-liberty:21.0.0.12-full-java11-openj9`](#websphere-liberty210012-full-java11-openj9)
-	[`websphere-liberty:21.0.0.12-full-java17-openj9`](#websphere-liberty210012-full-java17-openj9)
-	[`websphere-liberty:21.0.0.12-full-java8-ibmjava`](#websphere-liberty210012-full-java8-ibmjava)
-	[`websphere-liberty:21.0.0.12-kernel-java11-openj9`](#websphere-liberty210012-kernel-java11-openj9)
-	[`websphere-liberty:21.0.0.12-kernel-java17-openj9`](#websphere-liberty210012-kernel-java17-openj9)
-	[`websphere-liberty:21.0.0.12-kernel-java8-ibmjava`](#websphere-liberty210012-kernel-java8-ibmjava)
-	[`websphere-liberty:22.0.0.3-full-java11-openj9`](#websphere-liberty22003-full-java11-openj9)
-	[`websphere-liberty:22.0.0.3-full-java17-openj9`](#websphere-liberty22003-full-java17-openj9)
-	[`websphere-liberty:22.0.0.3-full-java8-ibmjava`](#websphere-liberty22003-full-java8-ibmjava)
-	[`websphere-liberty:22.0.0.3-kernel-java11-openj9`](#websphere-liberty22003-kernel-java11-openj9)
-	[`websphere-liberty:22.0.0.3-kernel-java17-openj9`](#websphere-liberty22003-kernel-java17-openj9)
-	[`websphere-liberty:22.0.0.3-kernel-java8-ibmjava`](#websphere-liberty22003-kernel-java8-ibmjava)
-	[`websphere-liberty:full`](#websphere-libertyfull)
-	[`websphere-liberty:full-java11-openj9`](#websphere-libertyfull-java11-openj9)
-	[`websphere-liberty:full-java17-openj9`](#websphere-libertyfull-java17-openj9)
-	[`websphere-liberty:kernel`](#websphere-libertykernel)
-	[`websphere-liberty:kernel-java11-openj9`](#websphere-libertykernel-java11-openj9)
-	[`websphere-liberty:kernel-java17-openj9`](#websphere-libertykernel-java17-openj9)
-	[`websphere-liberty:latest`](#websphere-libertylatest)

## `websphere-liberty:21.0.0.12-full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:85b1d23a0723c81fcf960e5a385ccac37a278d0db8453ae9710d726bca62193a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.12-full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:182cacffdc3c012ecbc9ff6ebba875960d6347fef02776fb118c75b186d6db53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.4 MB (392370383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d7f34c78ae497c4a00f97d42fb2d9045c1347ceb46fef04ea966528e2951374`
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
# Tue, 05 Apr 2022 23:31:52 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Tue, 05 Apr 2022 23:32:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 05 Apr 2022 23:32:58 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 23:32:58 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 05 Apr 2022 23:33:33 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 06 Apr 2022 06:05:18 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:05:18 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:20:07 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 06 Apr 2022 06:20:07 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 06 Apr 2022 06:20:07 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 06 Apr 2022 06:20:07 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl211220211117-1256 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 06:20:07 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 06 Apr 2022 06:20:07 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 06:20:07 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 06:20:15 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 06:20:15 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 06:20:16 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl211220211117-1256
# Wed, 06 Apr 2022 06:20:16 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:20:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 06:20:17 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 06:20:17 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 06:20:17 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 06:20:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 06:20:24 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 06:20:25 GMT
USER 1001
# Wed, 06 Apr 2022 06:20:25 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 06:20:25 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 06:20:25 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 06:25:31 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:25:31 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 06:29:02 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 06:29:03 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 06:29:38 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:2de664fdc03716f9363ceadd4dd17d7e1b14e86037b9096951d5742bcba8b7a7`  
		Last Modified: Tue, 05 Apr 2022 23:39:15 GMT  
		Size: 47.7 MB (47658316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73ebbc826a0dbf1766cf9d2329ac833ae344d2d462f4ad82159b63d7b58e41b`  
		Last Modified: Tue, 05 Apr 2022 23:39:09 GMT  
		Size: 4.3 MB (4333203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91eb4cbcd6cb1e1defd11ad3951f072fb4928bc4505b2db35743633bd432b189`  
		Last Modified: Wed, 06 Apr 2022 06:36:47 GMT  
		Size: 14.3 MB (14286112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fb8942e0ad9e5e5d5fb0218fb65f840412a41eb027ae4b6da78f2200299c38`  
		Last Modified: Wed, 06 Apr 2022 06:36:43 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d85d86c24a2eb627239ca5a3ecd1ed4906f32a7133f119b884adc80c87eb4ec`  
		Last Modified: Wed, 06 Apr 2022 06:36:43 GMT  
		Size: 9.7 KB (9671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2556593ce8079a404f0d13a1ecf151a84543a6f5d7caa05591913034d6f34915`  
		Last Modified: Wed, 06 Apr 2022 06:36:43 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67176bf95080c16e7a23f1dc539d4d7cbcaa91cd2bf623ced0faf7b905f4caa`  
		Last Modified: Wed, 06 Apr 2022 06:36:43 GMT  
		Size: 10.6 KB (10647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff997c265e4d85242d4280d12a7fdd1ec810c73d5e75cbf157fbd7e0d475dd60`  
		Last Modified: Wed, 06 Apr 2022 06:36:44 GMT  
		Size: 2.5 MB (2478923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e06d1082c1b16fe1234c9a68b1f8da627bcd79c31fc6d6cd417f5eba351463b`  
		Last Modified: Wed, 06 Apr 2022 06:37:44 GMT  
		Size: 264.6 MB (264634426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f941ceb62fa1b0f84aebcde67c507c83bc0e90efb8ddc79b81d331501cd7f3c`  
		Last Modified: Wed, 06 Apr 2022 06:37:25 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0221ce4e29da13e90a1a42fad8f84aeadfa4657d1e122fe7547d25ea3ee1ec`  
		Last Modified: Wed, 06 Apr 2022 06:37:28 GMT  
		Size: 14.4 MB (14360813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:832d9329ba2d6436c6b76e7a23ac97086b28dc92ebc9d7ece074d09f3a769975
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.2 MB (396182782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21a00ac8502d41994f04b04f79a3c4ced9e9f58c34077830d7803b1376bba8c9`
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
# Wed, 06 Apr 2022 05:25:20 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Wed, 06 Apr 2022 05:28:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 06 Apr 2022 05:28:29 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 05:28:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 06 Apr 2022 05:29:30 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 06 Apr 2022 11:03:56 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:04:03 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:35:42 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 06 Apr 2022 11:35:46 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 06 Apr 2022 11:35:50 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 06 Apr 2022 11:35:52 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl211220211117-1256 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 11:35:55 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 06 Apr 2022 11:35:58 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 11:36:01 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 11:36:42 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 11:36:47 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 11:36:50 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl211220211117-1256
# Wed, 06 Apr 2022 11:36:52 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:37:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 11:37:05 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 11:37:07 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 11:37:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 11:37:45 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 11:37:48 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 11:37:51 GMT
USER 1001
# Wed, 06 Apr 2022 11:37:53 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 11:37:57 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 11:38:02 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 11:46:44 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:46:50 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 11:51:26 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 11:51:32 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 11:52:37 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:b6584e4eaf032ab0a077066aaf7fed665eb2a8f3602e32470a2876ef90b88061`  
		Last Modified: Wed, 06 Apr 2022 05:42:06 GMT  
		Size: 48.4 MB (48356007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b610dbba5e90b2e3952904cb87b4c157a9a5130c86608dcbb6c497386be16e`  
		Last Modified: Wed, 06 Apr 2022 05:41:59 GMT  
		Size: 3.3 MB (3346135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e4e3baf72a75779c49d48aed68107566fa408d50eccb0fa42d80c07500a4b2`  
		Last Modified: Wed, 06 Apr 2022 12:03:28 GMT  
		Size: 14.3 MB (14286550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9ff29844be662148376f3df846f8ef9d00244baae577b3711a987643801685`  
		Last Modified: Wed, 06 Apr 2022 12:03:23 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6ef456aed7d8df42f3adf82914b95344b7bf620b7ba38cd96334f024cb9254`  
		Last Modified: Wed, 06 Apr 2022 12:03:23 GMT  
		Size: 9.7 KB (9672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac23b02ced8ff8ae9ad98549503dab067a8a109cef257cee1ec116802de26a34`  
		Last Modified: Wed, 06 Apr 2022 12:03:23 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46929683bd0c5840f64f0509450f6e98a3ae4960d7e94eab946ed75f68fc812`  
		Last Modified: Wed, 06 Apr 2022 12:03:23 GMT  
		Size: 10.7 KB (10655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2908c0bdd0d752e345a1d51eed0c4cf36e3196de3129f89bdcd9c2b3520434ad`  
		Last Modified: Wed, 06 Apr 2022 12:03:24 GMT  
		Size: 2.5 MB (2476404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59388089b65f752d6b45554fa58ccf69caf3e9d2b25ba8a711ed46666e3f5888`  
		Last Modified: Wed, 06 Apr 2022 12:04:48 GMT  
		Size: 264.6 MB (264634840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540c598ccbb2d14ab72c7e70041cec13c7f4910b2f943fedc2fd124ec95a9538`  
		Last Modified: Wed, 06 Apr 2022 12:04:24 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d8d2e4f3c6080b85aba52ac1483cb5d3240a04b3a8a3b36615078aa7fc101a`  
		Last Modified: Wed, 06 Apr 2022 12:04:27 GMT  
		Size: 12.6 MB (12564555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:932e671a772a80a36bfdfaaef69bf26b2146469de7296399f74da030da84f84c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **389.7 MB (389700213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f887cc07b2e18f5d2f05f162754bae1651fe6d06e8320e07eaf7e93ccadbbf3b`
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
# Tue, 05 Apr 2022 23:37:27 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Tue, 05 Apr 2022 23:38:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 05 Apr 2022 23:38:30 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 23:38:30 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 05 Apr 2022 23:39:03 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 06 Apr 2022 00:22:26 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:22:27 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:40:26 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 06 Apr 2022 00:40:26 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 06 Apr 2022 00:40:26 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 06 Apr 2022 00:40:26 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl211220211117-1256 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 00:40:26 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 06 Apr 2022 00:40:26 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 00:40:26 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 00:40:36 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:40:36 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 00:40:36 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl211220211117-1256
# Wed, 06 Apr 2022 00:40:37 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:40:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 00:40:37 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 00:40:37 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 00:40:38 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 00:40:43 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 00:40:43 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 00:40:43 GMT
USER 1001
# Wed, 06 Apr 2022 00:40:43 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 00:40:43 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 00:40:44 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 00:46:38 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:46:38 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 00:51:42 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 00:51:59 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 00:52:30 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:0efef42000170e3bcdd94a2519a9339d346b977d75a0129e443ce90e974708ce`  
		Last Modified: Tue, 05 Apr 2022 23:44:45 GMT  
		Size: 46.7 MB (46692257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b82868a62b6c97ba5baae49e8f092d01163d3296a2447501f70129c2eb3277`  
		Last Modified: Tue, 05 Apr 2022 23:44:40 GMT  
		Size: 4.3 MB (4308425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5218e0ace36c6b934b171b73fe6d193266c18fa8051d2394c63674b0f0fb5cb`  
		Last Modified: Wed, 06 Apr 2022 01:01:19 GMT  
		Size: 14.3 MB (14286290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b6cab245a02b15b0ee6394e7e1b4dd2f02272e7620e2189f8f3ac248cf1253`  
		Last Modified: Wed, 06 Apr 2022 01:01:16 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8a7ec7157605e19da186f624cefdfe517f042e16d27b7bd628dcb40c429ca4`  
		Last Modified: Wed, 06 Apr 2022 01:01:16 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e1469f6197226a02d621304a62bdc55e3341200de9fb9ebe2636b06bc09c7b`  
		Last Modified: Wed, 06 Apr 2022 01:01:16 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fca30cb6df73f571c62d0a109ab5108b0a74338dca6eb10c586170d2f82c90`  
		Last Modified: Wed, 06 Apr 2022 01:01:16 GMT  
		Size: 10.7 KB (10652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3692dd277a02ec2b29a449acb23dc87ce8787707a8374cd52252ae8a7e0d280`  
		Last Modified: Wed, 06 Apr 2022 01:01:17 GMT  
		Size: 2.5 MB (2518818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f39d3741d71b2718c17a2c98f9bc73f16f18ad1b992d3ef5369e284b2a7a692`  
		Last Modified: Wed, 06 Apr 2022 01:02:06 GMT  
		Size: 264.6 MB (264635139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ce0c8780cd76853c96e4f3426440a9d9c70f315e83ae26916ac3f9a10f4089`  
		Last Modified: Wed, 06 Apr 2022 01:01:55 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b0912c1ca61648f83405bfbffaea7c43afcb6fca457a896eef4d0204451b3c`  
		Last Modified: Wed, 06 Apr 2022 01:01:56 GMT  
		Size: 14.4 MB (14413822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.12-full-java17-openj9`

```console
$ docker pull websphere-liberty@sha256:e60ead357162bacebb9df051638c6ce04375afac81cc34fa67242f4198cbbd8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.12-full-java17-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:ec7e2865e5f287f3c7fef838f029f0a5bbcef6ab6526099743c01774b5cb58a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.3 MB (393279182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37031b26c9b65a54ae03502efdb75a829d62bf2c9a205e458cf1de3e5e25c22`
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
# Wed, 06 Apr 2022 06:20:30 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 06 Apr 2022 06:20:30 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 06 Apr 2022 06:20:30 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 06 Apr 2022 06:20:30 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl211220211117-1256 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 06:20:31 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 06 Apr 2022 06:20:31 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 06:20:31 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 06:20:38 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 06:20:39 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 06:20:39 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl211220211117-1256
# Wed, 06 Apr 2022 06:20:39 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:20:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 06:20:40 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 06:20:40 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 06:20:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 06:20:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 06:20:48 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 06:20:49 GMT
USER 1001
# Wed, 06 Apr 2022 06:20:49 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 06:20:49 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 06:20:49 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 06:29:54 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:29:54 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 06:33:30 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 06:33:30 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 06:34:06 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:dba1be02760b6993079603a4444cb9198933a1473d24eac2fae6a989511d6613`  
		Last Modified: Wed, 06 Apr 2022 06:36:58 GMT  
		Size: 14.3 MB (14286095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6122a2c2dcbe5f4a7d9432eaea28aa442500f6c5456ace0210ba4af79c938e3e`  
		Last Modified: Wed, 06 Apr 2022 06:36:53 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea659dc6a27d052bae33b2680b5faf7a296581c9e356bc499e72112129791f8`  
		Last Modified: Wed, 06 Apr 2022 06:36:54 GMT  
		Size: 9.7 KB (9672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d8bf1a13868d09adb8251174d4ef5df1abe58b5b64bcfeb52974db7bd1fd39`  
		Last Modified: Wed, 06 Apr 2022 06:36:54 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5014c8d6c2e51bbd9dee17493bf941723854ef015b61dac85c31c7c5428f6e`  
		Last Modified: Wed, 06 Apr 2022 06:36:53 GMT  
		Size: 10.6 KB (10643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb85f48ef5bb116b11a36bb2f63ac2040b4089526422f2f7c2a343f974438b5`  
		Last Modified: Wed, 06 Apr 2022 06:36:54 GMT  
		Size: 2.6 MB (2612353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1894f5a9533ef5e838fdf323b5eddb8cbae0df947d92fc75c495f4a88274f684`  
		Last Modified: Wed, 06 Apr 2022 06:38:08 GMT  
		Size: 264.6 MB (264634451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852dbc9485f0d6a62028c10e32e7af10dce755e1c06725f70bda92c2d2eab8cf`  
		Last Modified: Wed, 06 Apr 2022 06:37:54 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd99dbf23b9282ce6813228f80c8988f269387e462c053c038d48c102773ee1`  
		Last Modified: Wed, 06 Apr 2022 06:37:57 GMT  
		Size: 14.5 MB (14494856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-full-java17-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:0504d7a04ed93f53b0e347f0bf947262279c180e36adcd4b17deda58b753517c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.9 MB (396905270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca87173fca3d19e1a5c861aaf50cb8450d87922c7ef722f856dda760558f64f5`
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
# Wed, 06 Apr 2022 11:38:21 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 06 Apr 2022 11:38:23 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 06 Apr 2022 11:38:25 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 06 Apr 2022 11:38:27 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl211220211117-1256 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 11:38:28 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 06 Apr 2022 11:38:30 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 11:38:32 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 11:39:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 11:39:05 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 11:39:07 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl211220211117-1256
# Wed, 06 Apr 2022 11:39:09 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:39:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 11:39:17 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 11:39:18 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 11:39:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 11:39:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 11:39:48 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 11:39:51 GMT
USER 1001
# Wed, 06 Apr 2022 11:39:54 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 11:39:56 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 11:39:58 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 11:52:57 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:53:02 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 11:57:42 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 11:57:50 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 11:58:58 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:41ae0599a0ba71049c3a888cfffa7effd75838e65acb7fc5f58d01795753b3f4`  
		Last Modified: Wed, 06 Apr 2022 12:03:42 GMT  
		Size: 14.3 MB (14286549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62022870185dfb597ed88bfec0cd3337bc0146a9c5ecc1c0eff1e88721b0cbab`  
		Last Modified: Wed, 06 Apr 2022 12:03:38 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7ad7778f51a40546aaa44d12f4d8c7c47f8b1eaec5416cd5218ddde7e0342c`  
		Last Modified: Wed, 06 Apr 2022 12:03:37 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4fcab062f620d0ff8a3266fb85753bb053aabc4d61d5b4af6f019d2489c298`  
		Last Modified: Wed, 06 Apr 2022 12:03:38 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b27ba4a75d1b93903747ebbb57a6eee87015f159eac3dff1e18426e22702f56`  
		Last Modified: Wed, 06 Apr 2022 12:03:37 GMT  
		Size: 10.7 KB (10654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72828bdfee35fc6120f9ac6a8125101b9a440fdd8ddbbb256f5fea6693a85c37`  
		Last Modified: Wed, 06 Apr 2022 12:03:38 GMT  
		Size: 2.5 MB (2457034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b6b16c2849e829d454645fa18d869d480bce36a65549d3b8179cd013b00580`  
		Last Modified: Wed, 06 Apr 2022 12:05:21 GMT  
		Size: 264.6 MB (264635344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53fb84001077af15f78ab1a9be18cf11831d1787c9c5c022d612d070e5d51e3`  
		Last Modified: Wed, 06 Apr 2022 12:04:57 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d031c30ab22787a65dfa56936ce9bc4b53c01f9773d9add6db13bc7af07a204`  
		Last Modified: Wed, 06 Apr 2022 12:05:01 GMT  
		Size: 13.2 MB (13211453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-full-java17-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:5d00e6a30700d83fbc690d3dd463bb6b7d02671c5cf6ff00eb4cad37d6f3ff5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.2 MB (390178429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25b7a8074dc1f38f9a251a156bc1d52d8be697d50a7d095ce688689c1f63dcef`
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
# Wed, 06 Apr 2022 00:40:49 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 06 Apr 2022 00:40:49 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 06 Apr 2022 00:40:50 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 06 Apr 2022 00:40:50 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl211220211117-1256 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 00:40:50 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 06 Apr 2022 00:40:50 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 00:40:50 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 00:41:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:41:00 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 00:41:00 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl211220211117-1256
# Wed, 06 Apr 2022 00:41:00 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:41:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 00:41:01 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 00:41:01 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 00:41:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 00:41:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 00:41:07 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 00:41:07 GMT
USER 1001
# Wed, 06 Apr 2022 00:41:07 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 00:41:07 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 00:41:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 00:52:49 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:52:50 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 00:57:47 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 00:58:03 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 00:58:36 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:83bb27727b0d14675a72c14c933ac2b8a699fb949237205ef3b379d4bf33160f`  
		Last Modified: Wed, 06 Apr 2022 01:01:27 GMT  
		Size: 14.3 MB (14286280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d485423436c33574695ed9203bf48f0cc1242e1bd828ceba52753cf4c8563d45`  
		Last Modified: Wed, 06 Apr 2022 01:01:25 GMT  
		Size: 682.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a8600d8e5c5f2df925ab09a86c6f7f09684ee82973f3546a0548be1fa3e331`  
		Last Modified: Wed, 06 Apr 2022 01:01:25 GMT  
		Size: 9.7 KB (9668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919003a8426794f1cde05f3f60fc96413a390531a874d9288e425cce14bee96e`  
		Last Modified: Wed, 06 Apr 2022 01:01:25 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ee8c99d6f63f185b387768edef65f55d8f618e268e5892c1d7f02c38d30cc1`  
		Last Modified: Wed, 06 Apr 2022 01:01:25 GMT  
		Size: 10.6 KB (10643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138dccb86975e3c3c125ddd51c6758caea35b3f419be8ffb136f7801ade84d32`  
		Last Modified: Wed, 06 Apr 2022 01:01:25 GMT  
		Size: 2.5 MB (2510165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cb836cd139303ff8f1c818d9e974a93ab1bb54bc30b3a082227f673030cfe1`  
		Last Modified: Wed, 06 Apr 2022 01:02:24 GMT  
		Size: 264.6 MB (264635232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35626144f6ec29867d3678a0e38920f5af2e1e6da0e7ffb90b3a6a9e3f5d5150`  
		Last Modified: Wed, 06 Apr 2022 01:02:12 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07b15520663fb724202fb24198cf3899b3881b92f8e8880781b1bed3ac85467`  
		Last Modified: Wed, 06 Apr 2022 01:02:14 GMT  
		Size: 14.7 MB (14731807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.12-full-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:2cb6c1f92fdb7a534fdc2916c38a10199ddda5391141da4770bd29ad96ddbf86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.12-full-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:94e88c37179659d9f9d57bd311147bd21e21ef9eb4404c484cf490056cf36c3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **459.2 MB (459160015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdd0e57d007f71d6ca097ea4d250bb1f8eafe6842be7b3ffe098ea51ed61a4c9`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:42 GMT
ADD file:8a4ddbd462c1dd2016c64bd71ea6b5dba2ac4934bfd235a04d55b364666b67d1 in / 
# Tue, 05 Apr 2022 22:20:43 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 04:11:03 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Apr 2022 04:11:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:11:10 GMT
ENV JAVA_VERSION=8.0.7.5
# Wed, 06 Apr 2022 04:11:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Apr 2022 04:11:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 06:04:50 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:04:50 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:19:39 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 06 Apr 2022 06:19:39 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 06 Apr 2022 06:19:39 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 06 Apr 2022 06:19:39 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl211220211117-1256 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 06:19:39 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 06 Apr 2022 06:19:39 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 06:19:39 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 06:19:49 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 06:19:49 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 06:19:49 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl211220211117-1256
# Wed, 06 Apr 2022 06:19:49 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:19:50 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 06:19:50 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 06:19:50 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 06:19:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 06:20:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 06:20:00 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 06:20:00 GMT
USER 1001
# Wed, 06 Apr 2022 06:20:00 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 06:20:00 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 06:20:01 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 06:20:53 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:20:53 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 06:24:43 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 06:24:44 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 06:25:21 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:08a6abff89437fab99b52abbefed82ea907f12845c30eeb94f6b93c69be93166`  
		Last Modified: Tue, 05 Apr 2022 13:10:59 GMT  
		Size: 26.7 MB (26708938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfba7ea970cb1c55200b82df4d841cb3aeceb410b11a8979aa633a92e7d236b`  
		Last Modified: Wed, 06 Apr 2022 04:13:29 GMT  
		Size: 3.0 MB (2959903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7928eec80454bb70ea4d40960304e706827316397e2721ec34143d7e471d489`  
		Last Modified: Wed, 06 Apr 2022 04:13:39 GMT  
		Size: 128.8 MB (128801744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141942e76973a48faee7266c88d19a8ff74fed97759accfa50e4378d6bf09ac6`  
		Last Modified: Wed, 06 Apr 2022 06:36:36 GMT  
		Size: 14.2 MB (14187118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b043134d523dd6b6fb6f2ecf14dafd9c4e24325c7cfea0187fd7dfb0a25d42d4`  
		Last Modified: Wed, 06 Apr 2022 06:36:33 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc393cb897cee11d22d9ecd895d3978f729589b322b3fd417a50aaef99951c8`  
		Last Modified: Wed, 06 Apr 2022 06:36:32 GMT  
		Size: 9.7 KB (9674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b2804d700f0f71bce45e4aec74fa44e07c591a0866875a2018926e40344ad9`  
		Last Modified: Wed, 06 Apr 2022 06:36:32 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3827ed872068a11c457bea618344b2d7c845b246d916844aa0c15afc402a4b94`  
		Last Modified: Wed, 06 Apr 2022 06:36:32 GMT  
		Size: 10.7 KB (10657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc50b2787af5357baf2eaeb4b78b6c388307d596b4ef1153c81dfe93bae0fc05`  
		Last Modified: Wed, 06 Apr 2022 06:36:33 GMT  
		Size: 5.7 MB (5662962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd7b03e313ebab85345ea4abb588c1e11a32abef4c6467e04d5019e3905b8a9`  
		Last Modified: Wed, 06 Apr 2022 06:37:18 GMT  
		Size: 264.6 MB (264634869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3982b96755c908e7f5f625ca5310340736da04f3e4b33b94bcb74f79ce1ee539`  
		Last Modified: Wed, 06 Apr 2022 06:37:04 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c4d77f321e10a65a9afc25e5e70dfd48ddfdcee55e8268c6d7e6efe1007c4`  
		Last Modified: Wed, 06 Apr 2022 06:37:07 GMT  
		Size: 16.2 MB (16182221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-full-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:1af20998bf336d5c0a5a8475f3cea7fc119946b3ec23d762e82628a77f1ab746
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **459.6 MB (459571608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3306a12e528d1f33bc2fd0c211131a4ef7da587bb1b077a6f920c05f21389bd8`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 06 Apr 2022 03:35:14 GMT
ADD file:1dc494089c70f6414b0a1f5e2e09605266508bf5ec19e1e2fb17028253f8953d in / 
# Wed, 06 Apr 2022 03:35:17 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 05:13:40 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Apr 2022 05:14:24 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 05:14:31 GMT
ENV JAVA_VERSION=8.0.7.5
# Wed, 06 Apr 2022 05:15:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Apr 2022 05:15:55 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 11:00:44 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:00:46 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:32:48 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 06 Apr 2022 11:32:52 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 06 Apr 2022 11:32:57 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 06 Apr 2022 11:33:00 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl211220211117-1256 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 11:33:03 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 06 Apr 2022 11:33:04 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 11:33:09 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 11:33:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 11:34:00 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 11:34:02 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl211220211117-1256
# Wed, 06 Apr 2022 11:34:10 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:34:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 11:34:30 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 11:34:32 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 11:34:38 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 11:35:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 11:35:04 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 11:35:07 GMT
USER 1001
# Wed, 06 Apr 2022 11:35:09 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 11:35:16 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 11:35:22 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 11:40:17 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:40:20 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 11:45:07 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 11:45:17 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 11:46:22 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:74c6ac89233d470993bd9d67b39dc7ccb63096b55dc274e26eb50345bbecdcd8`  
		Last Modified: Tue, 05 Apr 2022 13:13:08 GMT  
		Size: 30.4 MB (30438429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdbaeb83a31ef16299d247a8ff263c6635af307374780bb9be69adac828283a`  
		Last Modified: Wed, 06 Apr 2022 05:19:24 GMT  
		Size: 3.1 MB (3082224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c2b3b642229c677b19f97c99ecf42203b8d144e161b096bac2c2f2423096b3`  
		Last Modified: Wed, 06 Apr 2022 05:19:37 GMT  
		Size: 128.3 MB (128315500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e1034f4699a85dfc9ab86899f0f36ba6e0a4208d690749c27fbcd2075b094e`  
		Last Modified: Wed, 06 Apr 2022 12:03:14 GMT  
		Size: 14.2 MB (14187826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73e8d44a0e5c029a0b4af5fc2eb48b615aaaef6776554d869bc3cbb227d153c`  
		Last Modified: Wed, 06 Apr 2022 12:03:09 GMT  
		Size: 709.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086df77cd750d64127e0b8fbb75937113d9e67896c90fa78f04e125b82eb109f`  
		Last Modified: Wed, 06 Apr 2022 12:03:09 GMT  
		Size: 9.7 KB (9673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b563fb35ad6e862d8746faa2a9b7051effbf9d29a91da955839d1efdf52125`  
		Last Modified: Wed, 06 Apr 2022 12:03:09 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deafe9f8b8afca0cbec5a63878a488c95dd4bf958a578e679aff9a8d96ee71c5`  
		Last Modified: Wed, 06 Apr 2022 12:03:09 GMT  
		Size: 10.7 KB (10664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c5c5b5b6ee215f8d1e487ef2754b8fd54d2b182d379e46bf769b6a95e50848`  
		Last Modified: Wed, 06 Apr 2022 12:03:10 GMT  
		Size: 5.3 MB (5291237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cbb79e2194b040d51dbd8ffdf69269771b7720d4ddbf4c8548c4bb872ca71c`  
		Last Modified: Wed, 06 Apr 2022 12:04:15 GMT  
		Size: 264.6 MB (264635068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ac887fcf65402b165d90e30983f805a64b39aa90616aee79d8834eac0e1ec1`  
		Last Modified: Wed, 06 Apr 2022 12:03:51 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fb37e5105aea8b260460b2b181cf99364217a11eb1e474c6000e84f33932ba`  
		Last Modified: Wed, 06 Apr 2022 12:03:54 GMT  
		Size: 13.6 MB (13599060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-full-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:5df69e1792e98923c3fa2a0cd3aa5420af3c2e66c065712f78217f7ece5e0f4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **454.3 MB (454258489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14b6143a429815382ebcff1fe115b1b6f768705e0b84e0d798b1579a307d2327`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Apr 2022 22:41:55 GMT
ADD file:7da6edcff7f600bf3a5d740cd585065c6b3748ff587c0627def91686d1bfe54d in / 
# Tue, 05 Apr 2022 22:41:57 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:04:20 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 05 Apr 2022 23:04:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:04:27 GMT
ENV JAVA_VERSION=8.0.7.5
# Tue, 05 Apr 2022 23:05:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 05 Apr 2022 23:05:10 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 00:21:45 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:21:45 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:39:58 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 06 Apr 2022 00:39:58 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 06 Apr 2022 00:39:58 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 06 Apr 2022 00:39:58 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl211220211117-1256 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 00:39:58 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 06 Apr 2022 00:39:59 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 00:39:59 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 00:40:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:40:10 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 00:40:10 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl211220211117-1256
# Wed, 06 Apr 2022 00:40:11 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:40:11 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 00:40:11 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 00:40:11 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 00:40:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 00:40:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 00:40:20 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 00:40:20 GMT
USER 1001
# Wed, 06 Apr 2022 00:40:20 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 00:40:20 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 00:40:20 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 00:41:14 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:41:14 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 00:45:47 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 00:45:57 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 00:46:27 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:4b0f8a5e4614be4866f08e8772b57664127164f512df03d05a52607176caa02f`  
		Last Modified: Tue, 05 Apr 2022 13:13:37 GMT  
		Size: 25.4 MB (25365860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1df112729db94ceb85cc2f4f1a8a29c4c17240f3414e928932240687367857b`  
		Last Modified: Tue, 05 Apr 2022 23:07:59 GMT  
		Size: 2.7 MB (2676913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7842fa8c2deed61ffe9a36afd3c1544e042b88e440ab57c28e1732e356ea75df`  
		Last Modified: Tue, 05 Apr 2022 23:08:07 GMT  
		Size: 125.8 MB (125807378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61e95eb02ce8e9f3944a356b2ce907c4bedb5b0b30c325e20e2da4e188092b9`  
		Last Modified: Wed, 06 Apr 2022 01:01:11 GMT  
		Size: 14.2 MB (14187232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db79a50be91abf5721fa260a799d7ce050f306d25f494b9197ef1e580b2fa01`  
		Last Modified: Wed, 06 Apr 2022 01:01:08 GMT  
		Size: 698.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f0587e03834f06b3da7bea6fcbd04bdf5321dfd85dd0e4a7203222ae974a2a`  
		Last Modified: Wed, 06 Apr 2022 01:01:09 GMT  
		Size: 9.7 KB (9673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d7e4bb1fd14954c1c93848d24985be894a65846dca7d265d8efc57261e6433`  
		Last Modified: Wed, 06 Apr 2022 01:01:08 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190a2732cba5766775499e667ea43547bad977b9af177ecb86ee011ac3d67fb0`  
		Last Modified: Wed, 06 Apr 2022 01:01:09 GMT  
		Size: 10.7 KB (10654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2816e47d3c334fe2cf3350f18bdbd54ce3550de8de4dc4da076b6e0ac6c46025`  
		Last Modified: Wed, 06 Apr 2022 01:01:09 GMT  
		Size: 5.8 MB (5805446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a46a959fa9215322121e1700cfc688413a014e8be23ad02238ba126bdc84373`  
		Last Modified: Wed, 06 Apr 2022 01:01:46 GMT  
		Size: 264.6 MB (264635442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d9060bb6abe09dea26984434052acdbdff1ae5729c8ef10853cfd9f2135a3e`  
		Last Modified: Wed, 06 Apr 2022 01:01:35 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4205c4d9727821717d835eb6580f40f7d8d56f592484f8c96055f168b683a8a8`  
		Last Modified: Wed, 06 Apr 2022 01:01:37 GMT  
		Size: 15.8 MB (15757972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.12-kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:592030acebfd315b23b4fe571154e23f2210ed9c7c1e3a1593ab77c82d95edeb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.12-kernel-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:b7998842a8174a752a2262b055415667a7b1a776b3322d074ccc72385d2b5388
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.4 MB (113374198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65a148fa88b561341d0f825422682c6d1830153aa283f522ca312e58ecfe6330`
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
# Tue, 05 Apr 2022 23:31:52 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Tue, 05 Apr 2022 23:32:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 05 Apr 2022 23:32:58 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 23:32:58 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 05 Apr 2022 23:33:33 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 06 Apr 2022 06:05:18 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:05:18 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:20:07 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 06 Apr 2022 06:20:07 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 06 Apr 2022 06:20:07 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 06 Apr 2022 06:20:07 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl211220211117-1256 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 06:20:07 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 06 Apr 2022 06:20:07 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 06:20:07 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 06:20:15 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 06:20:15 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 06:20:16 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl211220211117-1256
# Wed, 06 Apr 2022 06:20:16 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:20:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 06:20:17 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 06:20:17 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 06:20:17 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 06:20:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 06:20:24 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 06:20:25 GMT
USER 1001
# Wed, 06 Apr 2022 06:20:25 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 06:20:25 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 06:20:25 GMT
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
	-	`sha256:2de664fdc03716f9363ceadd4dd17d7e1b14e86037b9096951d5742bcba8b7a7`  
		Last Modified: Tue, 05 Apr 2022 23:39:15 GMT  
		Size: 47.7 MB (47658316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73ebbc826a0dbf1766cf9d2329ac833ae344d2d462f4ad82159b63d7b58e41b`  
		Last Modified: Tue, 05 Apr 2022 23:39:09 GMT  
		Size: 4.3 MB (4333203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91eb4cbcd6cb1e1defd11ad3951f072fb4928bc4505b2db35743633bd432b189`  
		Last Modified: Wed, 06 Apr 2022 06:36:47 GMT  
		Size: 14.3 MB (14286112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fb8942e0ad9e5e5d5fb0218fb65f840412a41eb027ae4b6da78f2200299c38`  
		Last Modified: Wed, 06 Apr 2022 06:36:43 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d85d86c24a2eb627239ca5a3ecd1ed4906f32a7133f119b884adc80c87eb4ec`  
		Last Modified: Wed, 06 Apr 2022 06:36:43 GMT  
		Size: 9.7 KB (9671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2556593ce8079a404f0d13a1ecf151a84543a6f5d7caa05591913034d6f34915`  
		Last Modified: Wed, 06 Apr 2022 06:36:43 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67176bf95080c16e7a23f1dc539d4d7cbcaa91cd2bf623ced0faf7b905f4caa`  
		Last Modified: Wed, 06 Apr 2022 06:36:43 GMT  
		Size: 10.6 KB (10647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff997c265e4d85242d4280d12a7fdd1ec810c73d5e75cbf157fbd7e0d475dd60`  
		Last Modified: Wed, 06 Apr 2022 06:36:44 GMT  
		Size: 2.5 MB (2478923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-kernel-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:8d59f71966540aa6291204fb6b8d7d0a18c50a841d13d2e6ec387a66bc477f00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118982440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ba17b6762f1f4a823e194f689462150cd5dbebe963d9317d4812347a76b7b20`
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
# Wed, 06 Apr 2022 05:25:20 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Wed, 06 Apr 2022 05:28:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 06 Apr 2022 05:28:29 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 05:28:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 06 Apr 2022 05:29:30 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 06 Apr 2022 11:03:56 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:04:03 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:35:42 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 06 Apr 2022 11:35:46 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 06 Apr 2022 11:35:50 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 06 Apr 2022 11:35:52 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl211220211117-1256 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 11:35:55 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 06 Apr 2022 11:35:58 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 11:36:01 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 11:36:42 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 11:36:47 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 11:36:50 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl211220211117-1256
# Wed, 06 Apr 2022 11:36:52 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:37:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 11:37:05 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 11:37:07 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 11:37:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 11:37:45 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 11:37:48 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 11:37:51 GMT
USER 1001
# Wed, 06 Apr 2022 11:37:53 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 11:37:57 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 11:38:02 GMT
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
	-	`sha256:b6584e4eaf032ab0a077066aaf7fed665eb2a8f3602e32470a2876ef90b88061`  
		Last Modified: Wed, 06 Apr 2022 05:42:06 GMT  
		Size: 48.4 MB (48356007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b610dbba5e90b2e3952904cb87b4c157a9a5130c86608dcbb6c497386be16e`  
		Last Modified: Wed, 06 Apr 2022 05:41:59 GMT  
		Size: 3.3 MB (3346135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e4e3baf72a75779c49d48aed68107566fa408d50eccb0fa42d80c07500a4b2`  
		Last Modified: Wed, 06 Apr 2022 12:03:28 GMT  
		Size: 14.3 MB (14286550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9ff29844be662148376f3df846f8ef9d00244baae577b3711a987643801685`  
		Last Modified: Wed, 06 Apr 2022 12:03:23 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6ef456aed7d8df42f3adf82914b95344b7bf620b7ba38cd96334f024cb9254`  
		Last Modified: Wed, 06 Apr 2022 12:03:23 GMT  
		Size: 9.7 KB (9672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac23b02ced8ff8ae9ad98549503dab067a8a109cef257cee1ec116802de26a34`  
		Last Modified: Wed, 06 Apr 2022 12:03:23 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46929683bd0c5840f64f0509450f6e98a3ae4960d7e94eab946ed75f68fc812`  
		Last Modified: Wed, 06 Apr 2022 12:03:23 GMT  
		Size: 10.7 KB (10655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2908c0bdd0d752e345a1d51eed0c4cf36e3196de3129f89bdcd9c2b3520434ad`  
		Last Modified: Wed, 06 Apr 2022 12:03:24 GMT  
		Size: 2.5 MB (2476404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:cc49a8138e6811d32509379e46950125b5678493828ed59f54b3e51a2fbfead6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110650307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98eb7ebdc5ad655f1db9ccb0dbcc462da0a782b21a8d0f034284e387f7701f4c`
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
# Tue, 05 Apr 2022 23:37:27 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Tue, 05 Apr 2022 23:38:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 05 Apr 2022 23:38:30 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 23:38:30 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 05 Apr 2022 23:39:03 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 06 Apr 2022 00:22:26 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:22:27 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:40:26 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 06 Apr 2022 00:40:26 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 06 Apr 2022 00:40:26 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 06 Apr 2022 00:40:26 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl211220211117-1256 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 00:40:26 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 06 Apr 2022 00:40:26 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 00:40:26 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 00:40:36 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:40:36 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 00:40:36 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl211220211117-1256
# Wed, 06 Apr 2022 00:40:37 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:40:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 00:40:37 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 00:40:37 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 00:40:38 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 00:40:43 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 00:40:43 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 00:40:43 GMT
USER 1001
# Wed, 06 Apr 2022 00:40:43 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 00:40:43 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 00:40:44 GMT
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
	-	`sha256:0efef42000170e3bcdd94a2519a9339d346b977d75a0129e443ce90e974708ce`  
		Last Modified: Tue, 05 Apr 2022 23:44:45 GMT  
		Size: 46.7 MB (46692257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b82868a62b6c97ba5baae49e8f092d01163d3296a2447501f70129c2eb3277`  
		Last Modified: Tue, 05 Apr 2022 23:44:40 GMT  
		Size: 4.3 MB (4308425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5218e0ace36c6b934b171b73fe6d193266c18fa8051d2394c63674b0f0fb5cb`  
		Last Modified: Wed, 06 Apr 2022 01:01:19 GMT  
		Size: 14.3 MB (14286290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b6cab245a02b15b0ee6394e7e1b4dd2f02272e7620e2189f8f3ac248cf1253`  
		Last Modified: Wed, 06 Apr 2022 01:01:16 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8a7ec7157605e19da186f624cefdfe517f042e16d27b7bd628dcb40c429ca4`  
		Last Modified: Wed, 06 Apr 2022 01:01:16 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e1469f6197226a02d621304a62bdc55e3341200de9fb9ebe2636b06bc09c7b`  
		Last Modified: Wed, 06 Apr 2022 01:01:16 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fca30cb6df73f571c62d0a109ab5108b0a74338dca6eb10c586170d2f82c90`  
		Last Modified: Wed, 06 Apr 2022 01:01:16 GMT  
		Size: 10.7 KB (10652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3692dd277a02ec2b29a449acb23dc87ce8787707a8374cd52252ae8a7e0d280`  
		Last Modified: Wed, 06 Apr 2022 01:01:17 GMT  
		Size: 2.5 MB (2518818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.12-kernel-java17-openj9`

```console
$ docker pull websphere-liberty@sha256:6637d835cfbb1010e24e29698907939fbf59d15d39adba43335fd2093c801c15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.12-kernel-java17-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:5ba12ae5da0c38e486dc2ef520892daa6e7ac07206af5330de9f90016c67fb8c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.1 MB (114148927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:405f3180ca33a57083edc0597d416855d09a4ad0f2080b0ea90012c0ed4a1423`
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
# Wed, 06 Apr 2022 06:20:30 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 06 Apr 2022 06:20:30 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 06 Apr 2022 06:20:30 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 06 Apr 2022 06:20:30 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl211220211117-1256 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 06:20:31 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 06 Apr 2022 06:20:31 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 06:20:31 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 06:20:38 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 06:20:39 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 06:20:39 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl211220211117-1256
# Wed, 06 Apr 2022 06:20:39 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:20:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 06:20:40 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 06:20:40 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 06:20:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 06:20:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 06:20:48 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 06:20:49 GMT
USER 1001
# Wed, 06 Apr 2022 06:20:49 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 06:20:49 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 06:20:49 GMT
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
	-	`sha256:dba1be02760b6993079603a4444cb9198933a1473d24eac2fae6a989511d6613`  
		Last Modified: Wed, 06 Apr 2022 06:36:58 GMT  
		Size: 14.3 MB (14286095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6122a2c2dcbe5f4a7d9432eaea28aa442500f6c5456ace0210ba4af79c938e3e`  
		Last Modified: Wed, 06 Apr 2022 06:36:53 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea659dc6a27d052bae33b2680b5faf7a296581c9e356bc499e72112129791f8`  
		Last Modified: Wed, 06 Apr 2022 06:36:54 GMT  
		Size: 9.7 KB (9672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d8bf1a13868d09adb8251174d4ef5df1abe58b5b64bcfeb52974db7bd1fd39`  
		Last Modified: Wed, 06 Apr 2022 06:36:54 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5014c8d6c2e51bbd9dee17493bf941723854ef015b61dac85c31c7c5428f6e`  
		Last Modified: Wed, 06 Apr 2022 06:36:53 GMT  
		Size: 10.6 KB (10643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb85f48ef5bb116b11a36bb2f63ac2040b4089526422f2f7c2a343f974438b5`  
		Last Modified: Wed, 06 Apr 2022 06:36:54 GMT  
		Size: 2.6 MB (2612353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-kernel-java17-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:cd63ad68dabf18fdcdb567b1e0dff17ec2170eaa32ffae736c3217b068a459f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.1 MB (119057524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da92ef9eac4d6b57bc49e67bdd602c8974d79975025257e0d494af38951fa9cd`
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
# Wed, 06 Apr 2022 11:38:21 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 06 Apr 2022 11:38:23 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 06 Apr 2022 11:38:25 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 06 Apr 2022 11:38:27 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl211220211117-1256 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 11:38:28 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 06 Apr 2022 11:38:30 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 11:38:32 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 11:39:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 11:39:05 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 11:39:07 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl211220211117-1256
# Wed, 06 Apr 2022 11:39:09 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:39:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 11:39:17 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 11:39:18 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 11:39:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 11:39:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 11:39:48 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 11:39:51 GMT
USER 1001
# Wed, 06 Apr 2022 11:39:54 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 11:39:56 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 11:39:58 GMT
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
	-	`sha256:41ae0599a0ba71049c3a888cfffa7effd75838e65acb7fc5f58d01795753b3f4`  
		Last Modified: Wed, 06 Apr 2022 12:03:42 GMT  
		Size: 14.3 MB (14286549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62022870185dfb597ed88bfec0cd3337bc0146a9c5ecc1c0eff1e88721b0cbab`  
		Last Modified: Wed, 06 Apr 2022 12:03:38 GMT  
		Size: 693.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7ad7778f51a40546aaa44d12f4d8c7c47f8b1eaec5416cd5218ddde7e0342c`  
		Last Modified: Wed, 06 Apr 2022 12:03:37 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4fcab062f620d0ff8a3266fb85753bb053aabc4d61d5b4af6f019d2489c298`  
		Last Modified: Wed, 06 Apr 2022 12:03:38 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b27ba4a75d1b93903747ebbb57a6eee87015f159eac3dff1e18426e22702f56`  
		Last Modified: Wed, 06 Apr 2022 12:03:37 GMT  
		Size: 10.7 KB (10654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72828bdfee35fc6120f9ac6a8125101b9a440fdd8ddbbb256f5fea6693a85c37`  
		Last Modified: Wed, 06 Apr 2022 12:03:38 GMT  
		Size: 2.5 MB (2457034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-kernel-java17-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:417ec8fe5623e23600f238cd35466fd05c2a3903f262aceed96f9e124c5c3ef9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110810447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c48b8c97423e733e5aa8c3d63bfa7b683a46d61f64603b8fac60ded90a0ea308`
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
# Wed, 06 Apr 2022 00:40:49 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 06 Apr 2022 00:40:49 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 06 Apr 2022 00:40:50 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 06 Apr 2022 00:40:50 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl211220211117-1256 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 00:40:50 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 06 Apr 2022 00:40:50 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 00:40:50 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 00:41:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:41:00 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 00:41:00 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl211220211117-1256
# Wed, 06 Apr 2022 00:41:00 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:41:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 00:41:01 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 00:41:01 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 00:41:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 00:41:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 00:41:07 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 00:41:07 GMT
USER 1001
# Wed, 06 Apr 2022 00:41:07 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 00:41:07 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 00:41:07 GMT
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
	-	`sha256:83bb27727b0d14675a72c14c933ac2b8a699fb949237205ef3b379d4bf33160f`  
		Last Modified: Wed, 06 Apr 2022 01:01:27 GMT  
		Size: 14.3 MB (14286280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d485423436c33574695ed9203bf48f0cc1242e1bd828ceba52753cf4c8563d45`  
		Last Modified: Wed, 06 Apr 2022 01:01:25 GMT  
		Size: 682.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a8600d8e5c5f2df925ab09a86c6f7f09684ee82973f3546a0548be1fa3e331`  
		Last Modified: Wed, 06 Apr 2022 01:01:25 GMT  
		Size: 9.7 KB (9668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919003a8426794f1cde05f3f60fc96413a390531a874d9288e425cce14bee96e`  
		Last Modified: Wed, 06 Apr 2022 01:01:25 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ee8c99d6f63f185b387768edef65f55d8f618e268e5892c1d7f02c38d30cc1`  
		Last Modified: Wed, 06 Apr 2022 01:01:25 GMT  
		Size: 10.6 KB (10643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138dccb86975e3c3c125ddd51c6758caea35b3f419be8ffb136f7801ade84d32`  
		Last Modified: Wed, 06 Apr 2022 01:01:25 GMT  
		Size: 2.5 MB (2510165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:21.0.0.12-kernel-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:b5b6b24cef5222268d4124784eba50d1e9e65c1dc9cb0c6196cc0d555fb9bf7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:21.0.0.12-kernel-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:f5b1666bd5fd8505f93971757050e11e51717de23efcc9261a32df6e62f286e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.3 MB (178341976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baf5876dd3b82e47a8fa26b1caaaae788d6a92b0853a26b018d8b3565e5724aa`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:42 GMT
ADD file:8a4ddbd462c1dd2016c64bd71ea6b5dba2ac4934bfd235a04d55b364666b67d1 in / 
# Tue, 05 Apr 2022 22:20:43 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 04:11:03 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Apr 2022 04:11:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:11:10 GMT
ENV JAVA_VERSION=8.0.7.5
# Wed, 06 Apr 2022 04:11:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Apr 2022 04:11:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 06:04:50 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:04:50 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:19:39 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 06 Apr 2022 06:19:39 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 06 Apr 2022 06:19:39 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 06 Apr 2022 06:19:39 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl211220211117-1256 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 06:19:39 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 06 Apr 2022 06:19:39 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 06:19:39 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 06:19:49 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 06:19:49 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 06:19:49 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl211220211117-1256
# Wed, 06 Apr 2022 06:19:49 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:19:50 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 06:19:50 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 06:19:50 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 06:19:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 06:20:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 06:20:00 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 06:20:00 GMT
USER 1001
# Wed, 06 Apr 2022 06:20:00 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 06:20:00 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 06:20:01 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:08a6abff89437fab99b52abbefed82ea907f12845c30eeb94f6b93c69be93166`  
		Last Modified: Tue, 05 Apr 2022 13:10:59 GMT  
		Size: 26.7 MB (26708938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfba7ea970cb1c55200b82df4d841cb3aeceb410b11a8979aa633a92e7d236b`  
		Last Modified: Wed, 06 Apr 2022 04:13:29 GMT  
		Size: 3.0 MB (2959903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7928eec80454bb70ea4d40960304e706827316397e2721ec34143d7e471d489`  
		Last Modified: Wed, 06 Apr 2022 04:13:39 GMT  
		Size: 128.8 MB (128801744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141942e76973a48faee7266c88d19a8ff74fed97759accfa50e4378d6bf09ac6`  
		Last Modified: Wed, 06 Apr 2022 06:36:36 GMT  
		Size: 14.2 MB (14187118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b043134d523dd6b6fb6f2ecf14dafd9c4e24325c7cfea0187fd7dfb0a25d42d4`  
		Last Modified: Wed, 06 Apr 2022 06:36:33 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc393cb897cee11d22d9ecd895d3978f729589b322b3fd417a50aaef99951c8`  
		Last Modified: Wed, 06 Apr 2022 06:36:32 GMT  
		Size: 9.7 KB (9674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b2804d700f0f71bce45e4aec74fa44e07c591a0866875a2018926e40344ad9`  
		Last Modified: Wed, 06 Apr 2022 06:36:32 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3827ed872068a11c457bea618344b2d7c845b246d916844aa0c15afc402a4b94`  
		Last Modified: Wed, 06 Apr 2022 06:36:32 GMT  
		Size: 10.7 KB (10657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc50b2787af5357baf2eaeb4b78b6c388307d596b4ef1153c81dfe93bae0fc05`  
		Last Modified: Wed, 06 Apr 2022 06:36:33 GMT  
		Size: 5.7 MB (5662962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-kernel-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:8ff93e9586ad8d40f9f1aacd2d95d9af354e107e12076755aa04fd19f34eb4a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.3 MB (181336534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5912cbefc2ccff4be55bc78f797ae52e75ffa89bdf64f31e5182f58cc5103d19`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 06 Apr 2022 03:35:14 GMT
ADD file:1dc494089c70f6414b0a1f5e2e09605266508bf5ec19e1e2fb17028253f8953d in / 
# Wed, 06 Apr 2022 03:35:17 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 05:13:40 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Apr 2022 05:14:24 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 05:14:31 GMT
ENV JAVA_VERSION=8.0.7.5
# Wed, 06 Apr 2022 05:15:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Apr 2022 05:15:55 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 11:00:44 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:00:46 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:32:48 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 06 Apr 2022 11:32:52 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 06 Apr 2022 11:32:57 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 06 Apr 2022 11:33:00 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl211220211117-1256 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 11:33:03 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 06 Apr 2022 11:33:04 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 11:33:09 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 11:33:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 11:34:00 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 11:34:02 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl211220211117-1256
# Wed, 06 Apr 2022 11:34:10 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:34:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 11:34:30 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 11:34:32 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 11:34:38 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 11:35:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 11:35:04 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 11:35:07 GMT
USER 1001
# Wed, 06 Apr 2022 11:35:09 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 11:35:16 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 11:35:22 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:74c6ac89233d470993bd9d67b39dc7ccb63096b55dc274e26eb50345bbecdcd8`  
		Last Modified: Tue, 05 Apr 2022 13:13:08 GMT  
		Size: 30.4 MB (30438429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdbaeb83a31ef16299d247a8ff263c6635af307374780bb9be69adac828283a`  
		Last Modified: Wed, 06 Apr 2022 05:19:24 GMT  
		Size: 3.1 MB (3082224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c2b3b642229c677b19f97c99ecf42203b8d144e161b096bac2c2f2423096b3`  
		Last Modified: Wed, 06 Apr 2022 05:19:37 GMT  
		Size: 128.3 MB (128315500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e1034f4699a85dfc9ab86899f0f36ba6e0a4208d690749c27fbcd2075b094e`  
		Last Modified: Wed, 06 Apr 2022 12:03:14 GMT  
		Size: 14.2 MB (14187826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73e8d44a0e5c029a0b4af5fc2eb48b615aaaef6776554d869bc3cbb227d153c`  
		Last Modified: Wed, 06 Apr 2022 12:03:09 GMT  
		Size: 709.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086df77cd750d64127e0b8fbb75937113d9e67896c90fa78f04e125b82eb109f`  
		Last Modified: Wed, 06 Apr 2022 12:03:09 GMT  
		Size: 9.7 KB (9673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b563fb35ad6e862d8746faa2a9b7051effbf9d29a91da955839d1efdf52125`  
		Last Modified: Wed, 06 Apr 2022 12:03:09 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deafe9f8b8afca0cbec5a63878a488c95dd4bf958a578e679aff9a8d96ee71c5`  
		Last Modified: Wed, 06 Apr 2022 12:03:09 GMT  
		Size: 10.7 KB (10664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c5c5b5b6ee215f8d1e487ef2754b8fd54d2b182d379e46bf769b6a95e50848`  
		Last Modified: Wed, 06 Apr 2022 12:03:10 GMT  
		Size: 5.3 MB (5291237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:21.0.0.12-kernel-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:9dcd03a3a43ef2f5ff29fc30d9609a27f837953a8e42657f3305786665d9471f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.9 MB (173864129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c19ac33458788bf42337753f0252ef606c6cb4ec0601321b6d6febab7840c30c`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Apr 2022 22:41:55 GMT
ADD file:7da6edcff7f600bf3a5d740cd585065c6b3748ff587c0627def91686d1bfe54d in / 
# Tue, 05 Apr 2022 22:41:57 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:04:20 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 05 Apr 2022 23:04:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:04:27 GMT
ENV JAVA_VERSION=8.0.7.5
# Tue, 05 Apr 2022 23:05:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 05 Apr 2022 23:05:10 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 00:21:45 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:21:45 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:39:58 GMT
ARG EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078
# Wed, 06 Apr 2022 00:39:58 GMT
ARG NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2
# Wed, 06 Apr 2022 00:39:58 GMT
ARG NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54
# Wed, 06 Apr 2022 00:39:58 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.12 org.opencontainers.image.revision=cl211220211117-1256 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 00:39:58 GMT
ENV LIBERTY_VERSION=21.0.0_12
# Wed, 06 Apr 2022 00:39:59 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 00:39:59 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 00:40:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:40:10 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 00:40:10 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.12 BuildLabel=cl211220211117-1256
# Wed, 06 Apr 2022 00:40:11 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:40:11 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 00:40:11 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 00:40:11 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 00:40:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 00:40:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=3e0b8b39a5c8000b0ad1458943454d8ad2e4b4712030cd0f96846a0aa1090078 NON_IBM_SHA=66d73b0d3e0cb314134e9fee966dbda6c388bf33645583921f63e00851242ff2 NOTICES_SHA=30a37bfd567f61c63daf4726d95ee3bf6d1c5f2b885678af4d52e44fa2f93e54 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 00:40:20 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 00:40:20 GMT
USER 1001
# Wed, 06 Apr 2022 00:40:20 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 00:40:20 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 00:40:20 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:4b0f8a5e4614be4866f08e8772b57664127164f512df03d05a52607176caa02f`  
		Last Modified: Tue, 05 Apr 2022 13:13:37 GMT  
		Size: 25.4 MB (25365860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1df112729db94ceb85cc2f4f1a8a29c4c17240f3414e928932240687367857b`  
		Last Modified: Tue, 05 Apr 2022 23:07:59 GMT  
		Size: 2.7 MB (2676913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7842fa8c2deed61ffe9a36afd3c1544e042b88e440ab57c28e1732e356ea75df`  
		Last Modified: Tue, 05 Apr 2022 23:08:07 GMT  
		Size: 125.8 MB (125807378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61e95eb02ce8e9f3944a356b2ce907c4bedb5b0b30c325e20e2da4e188092b9`  
		Last Modified: Wed, 06 Apr 2022 01:01:11 GMT  
		Size: 14.2 MB (14187232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db79a50be91abf5721fa260a799d7ce050f306d25f494b9197ef1e580b2fa01`  
		Last Modified: Wed, 06 Apr 2022 01:01:08 GMT  
		Size: 698.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f0587e03834f06b3da7bea6fcbd04bdf5321dfd85dd0e4a7203222ae974a2a`  
		Last Modified: Wed, 06 Apr 2022 01:01:09 GMT  
		Size: 9.7 KB (9673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d7e4bb1fd14954c1c93848d24985be894a65846dca7d265d8efc57261e6433`  
		Last Modified: Wed, 06 Apr 2022 01:01:08 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190a2732cba5766775499e667ea43547bad977b9af177ecb86ee011ac3d67fb0`  
		Last Modified: Wed, 06 Apr 2022 01:01:09 GMT  
		Size: 10.7 KB (10654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2816e47d3c334fe2cf3350f18bdbd54ce3550de8de4dc4da076b6e0ac6c46025`  
		Last Modified: Wed, 06 Apr 2022 01:01:09 GMT  
		Size: 5.8 MB (5805446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.3-full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:271c814dc860192c177b3159e377a0cb854cff53852b21f55468abe1805ebffd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:22.0.0.3-full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:9797600f2aea0ebdb8aed586ea0a80f7176bab06427609089b927974c406127b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.1 MB (392082245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a1412f68bc777621f23788740606e12ab92313a8021bf33b1d76fde065868ec`
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
# Tue, 05 Apr 2022 23:31:52 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Tue, 05 Apr 2022 23:32:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 05 Apr 2022 23:32:58 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 23:32:58 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 05 Apr 2022 23:33:33 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 06 Apr 2022 06:05:18 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:05:18 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:05:18 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 06:05:18 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 06:05:18 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 06:05:18 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 06:05:18 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 06:05:18 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 06:05:19 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 06:05:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 06:05:27 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 06:05:27 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 06:05:27 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:05:28 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 06:05:28 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 06:05:28 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 06:05:29 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 06:05:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 06:05:37 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 06:05:37 GMT
USER 1001
# Wed, 06 Apr 2022 06:05:37 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 06:05:37 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 06:05:37 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 06:10:42 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:10:42 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 06:14:23 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 06:14:24 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 06:14:58 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:2de664fdc03716f9363ceadd4dd17d7e1b14e86037b9096951d5742bcba8b7a7`  
		Last Modified: Tue, 05 Apr 2022 23:39:15 GMT  
		Size: 47.7 MB (47658316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73ebbc826a0dbf1766cf9d2329ac833ae344d2d462f4ad82159b63d7b58e41b`  
		Last Modified: Tue, 05 Apr 2022 23:39:09 GMT  
		Size: 4.3 MB (4333203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6132a1e30ebb061befc1dc524bec1dd16d89400628c2898a924654e48fe2fea0`  
		Last Modified: Wed, 06 Apr 2022 06:34:52 GMT  
		Size: 14.2 MB (14176948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f87590a8053062ea031a350fabd17c38798cf922f91301bcec7562cbca5c990`  
		Last Modified: Wed, 06 Apr 2022 06:34:48 GMT  
		Size: 688.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abedd88d5657c41d189250b3464751eb245af279284318677984c98dd1a92fa`  
		Last Modified: Wed, 06 Apr 2022 06:34:48 GMT  
		Size: 9.7 KB (9675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf381e38f8a29f5f63826328fbb4127a1c9a5c62f9a87b7a9c9229f30f0d84a`  
		Last Modified: Wed, 06 Apr 2022 06:34:48 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5ed086f03616c21833af3573ed3ebc2a7be3ca035cbff4ac0539b3cafcfd17`  
		Last Modified: Wed, 06 Apr 2022 06:34:48 GMT  
		Size: 10.7 KB (10651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a868e8fe31784701d1a577402dc0ca1c8414d996e92ea9562de4906604154089`  
		Last Modified: Wed, 06 Apr 2022 06:34:49 GMT  
		Size: 2.6 MB (2563936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20985f63df3a4adc843b7a4e0d223bba988fd56baa9f2639a234a3bf6c2da369`  
		Last Modified: Wed, 06 Apr 2022 06:35:46 GMT  
		Size: 264.0 MB (263977804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca66295c5b316ec0deb734ad793c6ccc3ac8754f319ebce0928e93cf80222fa`  
		Last Modified: Wed, 06 Apr 2022 06:35:33 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdc0db0f88390acf85409ce8b9e5b67f7e6720aad16a73b79f1f111a968ad4c`  
		Last Modified: Wed, 06 Apr 2022 06:35:35 GMT  
		Size: 14.8 MB (14753445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.3-full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:ace0e86e8e2660a4fadae29b799f3e25072d21d2db140a29d078114c64e51924
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.5 MB (395527289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7da5b44a87bd4293e3ae41575322dfa6f4d1ca0253d30fc0afeb10503a08701b`
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
# Wed, 06 Apr 2022 05:25:20 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Wed, 06 Apr 2022 05:28:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 06 Apr 2022 05:28:29 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 05:28:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 06 Apr 2022 05:29:30 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 06 Apr 2022 11:03:56 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:04:03 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:04:08 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 11:04:10 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 11:04:12 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 11:04:15 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 11:04:18 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 11:04:21 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 11:04:24 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 11:05:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 11:05:07 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 11:05:12 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 11:05:16 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:05:29 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 11:05:32 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 11:05:35 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 11:05:45 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 11:06:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 11:06:14 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 11:06:18 GMT
USER 1001
# Wed, 06 Apr 2022 11:06:21 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 11:06:27 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 11:06:29 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 11:19:27 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:19:31 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 11:24:24 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 11:24:30 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 11:25:33 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:b6584e4eaf032ab0a077066aaf7fed665eb2a8f3602e32470a2876ef90b88061`  
		Last Modified: Wed, 06 Apr 2022 05:42:06 GMT  
		Size: 48.4 MB (48356007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b610dbba5e90b2e3952904cb87b4c157a9a5130c86608dcbb6c497386be16e`  
		Last Modified: Wed, 06 Apr 2022 05:41:59 GMT  
		Size: 3.3 MB (3346135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95ae83fb73bece18f1fa8f40c395ae30eef41eebf1e48a38b2b9dbcd8e1d49c`  
		Last Modified: Wed, 06 Apr 2022 12:00:32 GMT  
		Size: 14.2 MB (14177015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86f956bcffb8404cc6684e7a66edb75965ee0f8b0f3a604f6c32425db347929`  
		Last Modified: Wed, 06 Apr 2022 12:00:27 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08016258ef4a64fde96e9d147484fe3e65a08cb41cee929bd1884553993ff80`  
		Last Modified: Wed, 06 Apr 2022 12:00:26 GMT  
		Size: 9.7 KB (9675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00695331e2e0491cc7528ef72c22343d7efdf0dd9805979574730aedaca08306`  
		Last Modified: Wed, 06 Apr 2022 12:00:26 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbcd96946f527cfb1cd5e6f585ec054d814e2a3896889a637d4e4a39cde58f5`  
		Last Modified: Wed, 06 Apr 2022 12:00:27 GMT  
		Size: 10.7 KB (10666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fc0431eea1ff91d5ec2ea2499d23b1b529f2e20e12ada3774a61b58c504fe4`  
		Last Modified: Wed, 06 Apr 2022 12:00:27 GMT  
		Size: 2.5 MB (2498053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4769339e764d724355c2701c937c017208a84bf442513b37fffc9a0565b4c47e`  
		Last Modified: Wed, 06 Apr 2022 12:01:59 GMT  
		Size: 264.0 MB (263980230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de22bb02b2b14b4da0dbddb55ec62288106a4b909a5714ee066809dd45ff4ea6`  
		Last Modified: Wed, 06 Apr 2022 12:01:35 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a22db6e2d685b28fb7c4225daac663469a0b034a02d3a4b64a02bd8086444e`  
		Last Modified: Wed, 06 Apr 2022 12:01:41 GMT  
		Size: 12.7 MB (12651538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.3-full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:1ffa26ba4ed12d7607b3f043784a1b8375b8b08a02c8acfe02b8d4dec7d96d73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **388.9 MB (388893052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ffacf41e1cc0b8ee433ae1a73ed72f2866712dea3024b1a084e1f0239ba5703`
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
# Tue, 05 Apr 2022 23:37:27 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Tue, 05 Apr 2022 23:38:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 05 Apr 2022 23:38:30 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 23:38:30 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 05 Apr 2022 23:39:03 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 06 Apr 2022 00:22:26 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:22:27 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:22:27 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 00:22:27 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 00:22:27 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 00:22:27 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 00:22:27 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 00:22:28 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 00:22:28 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 00:22:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:22:39 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 00:22:39 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 00:22:40 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:22:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 00:22:41 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 00:22:41 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 00:22:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 00:22:47 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 00:22:47 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 00:22:48 GMT
USER 1001
# Wed, 06 Apr 2022 00:22:48 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 00:22:48 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 00:22:48 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 00:28:51 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:28:51 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 00:33:21 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 00:33:26 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 00:33:52 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:0efef42000170e3bcdd94a2519a9339d346b977d75a0129e443ce90e974708ce`  
		Last Modified: Tue, 05 Apr 2022 23:44:45 GMT  
		Size: 46.7 MB (46692257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b82868a62b6c97ba5baae49e8f092d01163d3296a2447501f70129c2eb3277`  
		Last Modified: Tue, 05 Apr 2022 23:44:40 GMT  
		Size: 4.3 MB (4308425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058f842793768c6a4228763d95efeb7ddfaea1518fbeef298795d623064b8c04`  
		Last Modified: Wed, 06 Apr 2022 00:59:42 GMT  
		Size: 14.2 MB (14176985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a088cccd826c8de31e45c82202f3d0fd45572b7fd81409696fd14665fa7cde`  
		Last Modified: Wed, 06 Apr 2022 00:59:40 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f047879900349daf331d78bca6b10df39e0e6c83a732d77bffb4af8c34e26ef3`  
		Last Modified: Wed, 06 Apr 2022 00:59:40 GMT  
		Size: 9.7 KB (9676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a79c5873bc6c06caf02c6cd195ad6a736a03dabf60d71edacaeeedc1bca46a`  
		Last Modified: Wed, 06 Apr 2022 00:59:40 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26f79dcfee7280c24a869c0861196eda62e7a7db5e2571b47b72a9cc3f9e188`  
		Last Modified: Wed, 06 Apr 2022 00:59:40 GMT  
		Size: 10.7 KB (10655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b66e645849a3ac3034c982f9902b4477df8359237dc14e4b782a929ffeeea05`  
		Last Modified: Wed, 06 Apr 2022 00:59:40 GMT  
		Size: 2.6 MB (2556370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a251890d9a5809c5c1ac9a554925afed3b7b0fb47baf9dd2e56ecf4d2c1cb51`  
		Last Modified: Wed, 06 Apr 2022 01:00:28 GMT  
		Size: 264.0 MB (263979732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a02373f0608ae3251a9470df381d9f73bd0b0a869777fe0b906a644cce53ee`  
		Last Modified: Wed, 06 Apr 2022 01:00:16 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b675630eee794075b80d2bc070552a388f2b2462ca66cfb1675fa58b30fb5a7a`  
		Last Modified: Wed, 06 Apr 2022 01:00:18 GMT  
		Size: 14.3 MB (14333812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.3-full-java17-openj9`

```console
$ docker pull websphere-liberty@sha256:7bbe668c7134fef50c686219dbeb57f4a1ee5daa39c1d98a07ba288cb9984bbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:22.0.0.3-full-java17-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:a1f224fb2b02fe1abcc7ef2f69ad3074debf530e19b079bf40a24d3d3488de90
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.9 MB (392888570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7addf32e4ac1f24f011bad464204a44016e8982458ec38060731e87739be2cf2`
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
# Wed, 06 Apr 2022 06:15:05 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:15:05 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 06:18:49 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 06:18:50 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 06:19:26 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:46f79396957baf2dbd1896fa475541cb5f4812ade98e99b9fa96890156c7930e`  
		Last Modified: Wed, 06 Apr 2022 06:36:08 GMT  
		Size: 264.0 MB (263977221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4288ba967a1b39f55f94b7b0f114abb2bb52b4a830d73cbae02cb57d3edcfda4`  
		Last Modified: Wed, 06 Apr 2022 06:35:54 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a25a3e4180aa053251898ee4164c137669da61a217d942de833f8222521138`  
		Last Modified: Wed, 06 Apr 2022 06:35:56 GMT  
		Size: 14.9 MB (14902322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.3-full-java17-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:ecda3b2de80bfa580a08e73d1168ffa4a5b45ca2b6bc88bc7700df3222bab9d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.2 MB (396236120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5201d33f7c97805a986f71401c9f8427c827fa16eb465cfd01b6d80920439593`
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
# Wed, 06 Apr 2022 11:25:53 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:25:57 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 11:30:55 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 11:30:59 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 11:32:06 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:e25d61c85edc197b103a017fc7f613affcf103a0f46c39442245b0f02276be7f`  
		Last Modified: Wed, 06 Apr 2022 12:02:33 GMT  
		Size: 264.0 MB (263979505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b309a2a80174dffd819f9fbff3ed68ba27aaad395295105172978611ed1d922`  
		Last Modified: Wed, 06 Apr 2022 12:02:09 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37432f78ffcb85dbcc85751152b01ff2e19e3e0a077a2be6e2da9ca70b89e55`  
		Last Modified: Wed, 06 Apr 2022 12:02:13 GMT  
		Size: 13.3 MB (13269063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.3-full-java17-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:217ba82fef2ad2de05e542110e7dcb8411d15e88a10da6400b37e425d4bae63c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **389.3 MB (389324009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e4ee585f25815c703fc836a7be581346c17146aa110d145bad15acebafc205e`
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
# Wed, 06 Apr 2022 00:34:14 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:34:14 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 00:38:41 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 00:38:46 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 00:39:10 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:ca35b4ac395d9d8742983ea27fd9ecd988ed12a5d4ebe7527618ce33897c131a`  
		Last Modified: Wed, 06 Apr 2022 01:00:48 GMT  
		Size: 264.0 MB (263979666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452d4cc5b4a3b6c1dd13b16fef1f730e76fca9f0ef8715c8fb90d06326dff62c`  
		Last Modified: Wed, 06 Apr 2022 01:00:37 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7963455bc01e7b072abde32795f8086fe33cbf0e9c6ffdfb1b610f50cdc7d0c1`  
		Last Modified: Wed, 06 Apr 2022 01:00:38 GMT  
		Size: 14.5 MB (14521744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.3-full-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:8de0b824af28b3746a3c6125fedbb83a9280b825b1e923403306e79f722c376f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:22.0.0.3-full-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:cda65fcc714caba7e3c36f5b7435e9bdfc3ac25a35a1d19d6a4131202eb2db7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **458.4 MB (458358013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5ac205b973d5c45f76f1d8f62de7d9666fa8edc73a87e83caf63db1a09b0df9`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:42 GMT
ADD file:8a4ddbd462c1dd2016c64bd71ea6b5dba2ac4934bfd235a04d55b364666b67d1 in / 
# Tue, 05 Apr 2022 22:20:43 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 04:11:03 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Apr 2022 04:11:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:11:10 GMT
ENV JAVA_VERSION=8.0.7.5
# Wed, 06 Apr 2022 04:11:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Apr 2022 04:11:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 06:04:50 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:04:50 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:04:50 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 06:04:50 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 06:04:50 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 06:04:50 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 06:04:51 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 06:04:51 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 06:04:51 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 06:05:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 06:05:01 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 06:05:01 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 06:05:02 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:05:03 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 06:05:03 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 06:05:03 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 06:05:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 06:05:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 06:05:13 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 06:05:13 GMT
USER 1001
# Wed, 06 Apr 2022 06:05:14 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 06:05:14 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 06:05:14 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 06:06:04 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:06:04 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 06:09:55 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 06:09:56 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 06:10:33 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:08a6abff89437fab99b52abbefed82ea907f12845c30eeb94f6b93c69be93166`  
		Last Modified: Tue, 05 Apr 2022 13:10:59 GMT  
		Size: 26.7 MB (26708938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfba7ea970cb1c55200b82df4d841cb3aeceb410b11a8979aa633a92e7d236b`  
		Last Modified: Wed, 06 Apr 2022 04:13:29 GMT  
		Size: 3.0 MB (2959903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7928eec80454bb70ea4d40960304e706827316397e2721ec34143d7e471d489`  
		Last Modified: Wed, 06 Apr 2022 04:13:39 GMT  
		Size: 128.8 MB (128801744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e8321e19197f2773b582a498e2c352f378d117442244e67ab76160b26c151`  
		Last Modified: Wed, 06 Apr 2022 06:34:41 GMT  
		Size: 14.1 MB (14079475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f525ec02b7acf591d7d8eec0bc9312b4d67404d39b2fe6b867cbdd75cda5957`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24de75b5ad0e32a1538636e8cf2db791b896dda43206f4b53cd75447dcdd9d69`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 9.7 KB (9680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17671817a6482e1aab160a13024a37aa3725d833b5e1fe872e40c965b3e60c2`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd49fec10585cc3bbdc3a0fb3580e26135a7b7910e8fef1cc1cded362c8d33c`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 10.7 KB (10652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5821dc03875268203466d1599daa966b4ca91b58ed9b5391b9d3274d649c7efa`  
		Last Modified: Wed, 06 Apr 2022 06:34:38 GMT  
		Size: 5.7 MB (5698843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c243f60957de1ee44d01c6baaae691fe8078ff83354adf037360a605c61e29f0`  
		Last Modified: Wed, 06 Apr 2022 06:35:23 GMT  
		Size: 264.0 MB (263977874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bea240e7db6ec28462ead5dea5d2b49793e7ca3048380006748d9551ae47aca`  
		Last Modified: Wed, 06 Apr 2022 06:35:09 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf55c107ae9a8dec5f029da6a473b1e6a1de8413e84cbabacf8ee2932c9c6eb5`  
		Last Modified: Wed, 06 Apr 2022 06:35:12 GMT  
		Size: 16.1 MB (16108990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.3-full-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:c97b5678d350c594cbcbd9036c7bb6eb551c40d1fc684f6deba01863d86c196c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **459.4 MB (459380904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92453735197d834aebbc804122ab90fd2bca3463f14bdd638c9a611e89ee0f6c`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 06 Apr 2022 03:35:14 GMT
ADD file:1dc494089c70f6414b0a1f5e2e09605266508bf5ec19e1e2fb17028253f8953d in / 
# Wed, 06 Apr 2022 03:35:17 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 05:13:40 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Apr 2022 05:14:24 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 05:14:31 GMT
ENV JAVA_VERSION=8.0.7.5
# Wed, 06 Apr 2022 05:15:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Apr 2022 05:15:55 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 11:00:44 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:00:46 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:00:50 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 11:00:53 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 11:00:56 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 11:00:59 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 11:01:01 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 11:01:03 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 11:01:07 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 11:01:47 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 11:01:52 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 11:01:57 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 11:02:02 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:02:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 11:02:29 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 11:02:31 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 11:02:43 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 11:03:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 11:03:16 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 11:03:22 GMT
USER 1001
# Wed, 06 Apr 2022 11:03:28 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 11:03:32 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 11:03:34 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 11:12:16 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:12:20 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 11:17:19 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 11:17:36 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 11:19:12 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:74c6ac89233d470993bd9d67b39dc7ccb63096b55dc274e26eb50345bbecdcd8`  
		Last Modified: Tue, 05 Apr 2022 13:13:08 GMT  
		Size: 30.4 MB (30438429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdbaeb83a31ef16299d247a8ff263c6635af307374780bb9be69adac828283a`  
		Last Modified: Wed, 06 Apr 2022 05:19:24 GMT  
		Size: 3.1 MB (3082224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c2b3b642229c677b19f97c99ecf42203b8d144e161b096bac2c2f2423096b3`  
		Last Modified: Wed, 06 Apr 2022 05:19:37 GMT  
		Size: 128.3 MB (128315500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607319fec708d071582f7068356a9b783452155ba745e3ae2a1ee5ff70006816`  
		Last Modified: Wed, 06 Apr 2022 12:00:17 GMT  
		Size: 14.1 MB (14080204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db26f8d06474b6cdae2a54e5b37464ae2d95059cad5bf4f189066796933a20b`  
		Last Modified: Wed, 06 Apr 2022 12:00:12 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c1989f41a81f220c80b3443f5b96a49f0372f9d53626c1551cdb7c72835b58`  
		Last Modified: Wed, 06 Apr 2022 12:00:12 GMT  
		Size: 9.7 KB (9677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3bfd5a575c436bbb31c349cb945f2f841da5996f2fe41fe71c3a5c1c9cc2fd`  
		Last Modified: Wed, 06 Apr 2022 12:00:12 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96179275284d5d42953fdbb04b7c28b376c018e18dc4e7fa6acadebcd137663a`  
		Last Modified: Wed, 06 Apr 2022 12:00:13 GMT  
		Size: 10.7 KB (10670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df489a3f9e1f8998afa4e608455726d81d3a58818050d61fd27c6c7b77244af`  
		Last Modified: Wed, 06 Apr 2022 12:00:13 GMT  
		Size: 5.3 MB (5336752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b042d816e5dae6c615a67e99c9c146f9361cb053c7191a28453ee4bac700dd`  
		Last Modified: Wed, 06 Apr 2022 12:01:20 GMT  
		Size: 264.0 MB (263979859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27a22ff3e3a47f2f395eea6bcdf51b5900894b8bc4088f6bb5a568e5faa585e`  
		Last Modified: Wed, 06 Apr 2022 12:00:57 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395acfb1d10392c0b8bd138f86cd3d941e8ed4e3df73d3dddc2d25c5e1cd20ba`  
		Last Modified: Wed, 06 Apr 2022 12:01:00 GMT  
		Size: 14.1 MB (14125664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.3-full-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:17a16ee52bccd25691b4511b3a476c3b9e8b89db8bb57e2cad48f1a27f1325bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **453.8 MB (453776780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f6c02bef0033fdf780cd7e119e505dd2cc3448e877dacc650f05f9ab493896b`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Apr 2022 22:41:55 GMT
ADD file:7da6edcff7f600bf3a5d740cd585065c6b3748ff587c0627def91686d1bfe54d in / 
# Tue, 05 Apr 2022 22:41:57 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:04:20 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 05 Apr 2022 23:04:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:04:27 GMT
ENV JAVA_VERSION=8.0.7.5
# Tue, 05 Apr 2022 23:05:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 05 Apr 2022 23:05:10 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 00:21:45 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:21:45 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:21:45 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 00:21:45 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 00:21:45 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 00:21:46 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 00:21:46 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 00:21:46 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 00:21:46 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 00:22:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:22:00 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 00:22:00 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 00:22:01 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:22:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 00:22:03 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 00:22:03 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 00:22:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 00:22:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 00:22:13 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 00:22:13 GMT
USER 1001
# Wed, 06 Apr 2022 00:22:13 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 00:22:14 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 00:22:14 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 00:23:26 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:23:27 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 00:28:01 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 00:28:10 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 00:28:39 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:4b0f8a5e4614be4866f08e8772b57664127164f512df03d05a52607176caa02f`  
		Last Modified: Tue, 05 Apr 2022 13:13:37 GMT  
		Size: 25.4 MB (25365860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1df112729db94ceb85cc2f4f1a8a29c4c17240f3414e928932240687367857b`  
		Last Modified: Tue, 05 Apr 2022 23:07:59 GMT  
		Size: 2.7 MB (2676913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7842fa8c2deed61ffe9a36afd3c1544e042b88e440ab57c28e1732e356ea75df`  
		Last Modified: Tue, 05 Apr 2022 23:08:07 GMT  
		Size: 125.8 MB (125807378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404f68c2321c29cbc1068910410523410cf5f547bd14a1a39d22a191b7af2f2c`  
		Last Modified: Wed, 06 Apr 2022 00:59:35 GMT  
		Size: 14.1 MB (14079579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae1055a4b0be252bcf172f8c6844707d527fcef2a35187c9569bef098a77c18`  
		Last Modified: Wed, 06 Apr 2022 00:59:32 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc478f125deb368d73eb16801b69efb288cb07b229ff40ef29a31cd1fec805c`  
		Last Modified: Wed, 06 Apr 2022 00:59:32 GMT  
		Size: 9.7 KB (9682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90d9b68d251175efb44f7e467b8bc09edacfc0fbf0d138d33684cfd78d72d9f`  
		Last Modified: Wed, 06 Apr 2022 00:59:32 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d346a08c2d95ddc678ee0d514318700fdbbc867edbdc372f52a1d50792cf92af`  
		Last Modified: Wed, 06 Apr 2022 00:59:33 GMT  
		Size: 10.7 KB (10657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79772bc444250adebe9820159101675bd0b319704a1298e7b58cc96a2fc91830`  
		Last Modified: Wed, 06 Apr 2022 00:59:33 GMT  
		Size: 5.8 MB (5840724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af3906793f5b93df770a0e9c8ab76701e7a7462c459753b23abeb8927f0be8f`  
		Last Modified: Wed, 06 Apr 2022 01:00:07 GMT  
		Size: 264.0 MB (263980552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc4cd25be3f31eced3efee7946ca0b82fb018fd5d8a2ca3ef863f738de062ae`  
		Last Modified: Wed, 06 Apr 2022 00:59:55 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4ee76efe1d5ce46952511f6eabd0cc40ccf205b07c26582d2504d6d50a868c`  
		Last Modified: Wed, 06 Apr 2022 00:59:57 GMT  
		Size: 16.0 MB (16003518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.3-kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:2004177a4e7200445aca1ba0270f9490fa23de84f6d610f98693cb918d34a7dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:22.0.0.3-kernel-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:8ce41452f4500cd47ad92e6805c35f5918273c14b929cfd2e174a2e294563fba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.4 MB (113350052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d77be323eea3d650decb6f7130da21769792ab442e397d990775fdd96699fda8`
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
# Tue, 05 Apr 2022 23:31:52 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Tue, 05 Apr 2022 23:32:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 05 Apr 2022 23:32:58 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 23:32:58 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 05 Apr 2022 23:33:33 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 06 Apr 2022 06:05:18 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:05:18 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:05:18 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 06:05:18 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 06:05:18 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 06:05:18 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 06:05:18 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 06:05:18 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 06:05:19 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 06:05:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 06:05:27 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 06:05:27 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 06:05:27 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:05:28 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 06:05:28 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 06:05:28 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 06:05:29 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 06:05:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 06:05:37 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 06:05:37 GMT
USER 1001
# Wed, 06 Apr 2022 06:05:37 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 06:05:37 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 06:05:37 GMT
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
	-	`sha256:2de664fdc03716f9363ceadd4dd17d7e1b14e86037b9096951d5742bcba8b7a7`  
		Last Modified: Tue, 05 Apr 2022 23:39:15 GMT  
		Size: 47.7 MB (47658316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73ebbc826a0dbf1766cf9d2329ac833ae344d2d462f4ad82159b63d7b58e41b`  
		Last Modified: Tue, 05 Apr 2022 23:39:09 GMT  
		Size: 4.3 MB (4333203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6132a1e30ebb061befc1dc524bec1dd16d89400628c2898a924654e48fe2fea0`  
		Last Modified: Wed, 06 Apr 2022 06:34:52 GMT  
		Size: 14.2 MB (14176948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f87590a8053062ea031a350fabd17c38798cf922f91301bcec7562cbca5c990`  
		Last Modified: Wed, 06 Apr 2022 06:34:48 GMT  
		Size: 688.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abedd88d5657c41d189250b3464751eb245af279284318677984c98dd1a92fa`  
		Last Modified: Wed, 06 Apr 2022 06:34:48 GMT  
		Size: 9.7 KB (9675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf381e38f8a29f5f63826328fbb4127a1c9a5c62f9a87b7a9c9229f30f0d84a`  
		Last Modified: Wed, 06 Apr 2022 06:34:48 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5ed086f03616c21833af3573ed3ebc2a7be3ca035cbff4ac0539b3cafcfd17`  
		Last Modified: Wed, 06 Apr 2022 06:34:48 GMT  
		Size: 10.7 KB (10651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a868e8fe31784701d1a577402dc0ca1c8414d996e92ea9562de4906604154089`  
		Last Modified: Wed, 06 Apr 2022 06:34:49 GMT  
		Size: 2.6 MB (2563936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.3-kernel-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:0181e3a088fbed78f05be0c5c664db7aae2ec526e5784e52411292fbe24fc2ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118894573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a42b286e66f0e555edc25ed96a891d292ed41695d877db432119bf4ee852c495`
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
# Wed, 06 Apr 2022 05:25:20 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Wed, 06 Apr 2022 05:28:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 06 Apr 2022 05:28:29 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 05:28:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 06 Apr 2022 05:29:30 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 06 Apr 2022 11:03:56 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:04:03 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:04:08 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 11:04:10 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 11:04:12 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 11:04:15 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 11:04:18 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 11:04:21 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 11:04:24 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 11:05:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 11:05:07 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 11:05:12 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 11:05:16 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:05:29 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 11:05:32 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 11:05:35 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 11:05:45 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 11:06:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 11:06:14 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 11:06:18 GMT
USER 1001
# Wed, 06 Apr 2022 11:06:21 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 11:06:27 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 11:06:29 GMT
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
	-	`sha256:b6584e4eaf032ab0a077066aaf7fed665eb2a8f3602e32470a2876ef90b88061`  
		Last Modified: Wed, 06 Apr 2022 05:42:06 GMT  
		Size: 48.4 MB (48356007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b610dbba5e90b2e3952904cb87b4c157a9a5130c86608dcbb6c497386be16e`  
		Last Modified: Wed, 06 Apr 2022 05:41:59 GMT  
		Size: 3.3 MB (3346135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95ae83fb73bece18f1fa8f40c395ae30eef41eebf1e48a38b2b9dbcd8e1d49c`  
		Last Modified: Wed, 06 Apr 2022 12:00:32 GMT  
		Size: 14.2 MB (14177015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86f956bcffb8404cc6684e7a66edb75965ee0f8b0f3a604f6c32425db347929`  
		Last Modified: Wed, 06 Apr 2022 12:00:27 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08016258ef4a64fde96e9d147484fe3e65a08cb41cee929bd1884553993ff80`  
		Last Modified: Wed, 06 Apr 2022 12:00:26 GMT  
		Size: 9.7 KB (9675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00695331e2e0491cc7528ef72c22343d7efdf0dd9805979574730aedaca08306`  
		Last Modified: Wed, 06 Apr 2022 12:00:26 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbcd96946f527cfb1cd5e6f585ec054d814e2a3896889a637d4e4a39cde58f5`  
		Last Modified: Wed, 06 Apr 2022 12:00:27 GMT  
		Size: 10.7 KB (10666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fc0431eea1ff91d5ec2ea2499d23b1b529f2e20e12ada3774a61b58c504fe4`  
		Last Modified: Wed, 06 Apr 2022 12:00:27 GMT  
		Size: 2.5 MB (2498053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.3-kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:d7155eac65555d6fbef3279d48d1b15f44c0bc5788b56889187901d07734a8aa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110578561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:182d330bce80f26c52deb1c7070bbdcbf23a2b23357d1ad02d453e1d9b38875e`
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
# Tue, 05 Apr 2022 23:37:27 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Tue, 05 Apr 2022 23:38:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 05 Apr 2022 23:38:30 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 23:38:30 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 05 Apr 2022 23:39:03 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 06 Apr 2022 00:22:26 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:22:27 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:22:27 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 00:22:27 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 00:22:27 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 00:22:27 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 00:22:27 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 00:22:28 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 00:22:28 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 00:22:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:22:39 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 00:22:39 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 00:22:40 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:22:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 00:22:41 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 00:22:41 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 00:22:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 00:22:47 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 00:22:47 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 00:22:48 GMT
USER 1001
# Wed, 06 Apr 2022 00:22:48 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 00:22:48 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 00:22:48 GMT
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
	-	`sha256:0efef42000170e3bcdd94a2519a9339d346b977d75a0129e443ce90e974708ce`  
		Last Modified: Tue, 05 Apr 2022 23:44:45 GMT  
		Size: 46.7 MB (46692257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b82868a62b6c97ba5baae49e8f092d01163d3296a2447501f70129c2eb3277`  
		Last Modified: Tue, 05 Apr 2022 23:44:40 GMT  
		Size: 4.3 MB (4308425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058f842793768c6a4228763d95efeb7ddfaea1518fbeef298795d623064b8c04`  
		Last Modified: Wed, 06 Apr 2022 00:59:42 GMT  
		Size: 14.2 MB (14176985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a088cccd826c8de31e45c82202f3d0fd45572b7fd81409696fd14665fa7cde`  
		Last Modified: Wed, 06 Apr 2022 00:59:40 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f047879900349daf331d78bca6b10df39e0e6c83a732d77bffb4af8c34e26ef3`  
		Last Modified: Wed, 06 Apr 2022 00:59:40 GMT  
		Size: 9.7 KB (9676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a79c5873bc6c06caf02c6cd195ad6a736a03dabf60d71edacaeeedc1bca46a`  
		Last Modified: Wed, 06 Apr 2022 00:59:40 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26f79dcfee7280c24a869c0861196eda62e7a7db5e2571b47b72a9cc3f9e188`  
		Last Modified: Wed, 06 Apr 2022 00:59:40 GMT  
		Size: 10.7 KB (10655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b66e645849a3ac3034c982f9902b4477df8359237dc14e4b782a929ffeeea05`  
		Last Modified: Wed, 06 Apr 2022 00:59:40 GMT  
		Size: 2.6 MB (2556370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:22.0.0.3-kernel-java17-openj9`

```console
$ docker pull websphere-liberty@sha256:2483ee1237a1c69fe21a4f023ead2402d4a46baff9423e496360abeb8cc6d540
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:22.0.0.3-kernel-java17-openj9` - linux; amd64

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

### `websphere-liberty:22.0.0.3-kernel-java17-openj9` - linux; ppc64le

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

### `websphere-liberty:22.0.0.3-kernel-java17-openj9` - linux; s390x

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

## `websphere-liberty:22.0.0.3-kernel-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:c49f2ec5c5a1a18b6417755bcb8e51bb167210c07d94578a08c2232f71418a29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:22.0.0.3-kernel-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:9e3edcb74de734f3cc5a6ba6c2b7e512bae73e107bf0e55323bc4136e9c64eb3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.3 MB (178270202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ba3ec0b3bf0b3fa6b9b4319be274cfbde67785b8f210f79e3b8e5382550b10a`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:42 GMT
ADD file:8a4ddbd462c1dd2016c64bd71ea6b5dba2ac4934bfd235a04d55b364666b67d1 in / 
# Tue, 05 Apr 2022 22:20:43 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 04:11:03 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Apr 2022 04:11:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:11:10 GMT
ENV JAVA_VERSION=8.0.7.5
# Wed, 06 Apr 2022 04:11:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Apr 2022 04:11:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 06:04:50 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:04:50 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:04:50 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 06:04:50 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 06:04:50 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 06:04:50 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 06:04:51 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 06:04:51 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 06:04:51 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 06:05:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 06:05:01 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 06:05:01 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 06:05:02 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:05:03 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 06:05:03 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 06:05:03 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 06:05:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 06:05:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 06:05:13 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 06:05:13 GMT
USER 1001
# Wed, 06 Apr 2022 06:05:14 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 06:05:14 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 06:05:14 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:08a6abff89437fab99b52abbefed82ea907f12845c30eeb94f6b93c69be93166`  
		Last Modified: Tue, 05 Apr 2022 13:10:59 GMT  
		Size: 26.7 MB (26708938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfba7ea970cb1c55200b82df4d841cb3aeceb410b11a8979aa633a92e7d236b`  
		Last Modified: Wed, 06 Apr 2022 04:13:29 GMT  
		Size: 3.0 MB (2959903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7928eec80454bb70ea4d40960304e706827316397e2721ec34143d7e471d489`  
		Last Modified: Wed, 06 Apr 2022 04:13:39 GMT  
		Size: 128.8 MB (128801744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e8321e19197f2773b582a498e2c352f378d117442244e67ab76160b26c151`  
		Last Modified: Wed, 06 Apr 2022 06:34:41 GMT  
		Size: 14.1 MB (14079475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f525ec02b7acf591d7d8eec0bc9312b4d67404d39b2fe6b867cbdd75cda5957`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24de75b5ad0e32a1538636e8cf2db791b896dda43206f4b53cd75447dcdd9d69`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 9.7 KB (9680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17671817a6482e1aab160a13024a37aa3725d833b5e1fe872e40c965b3e60c2`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd49fec10585cc3bbdc3a0fb3580e26135a7b7910e8fef1cc1cded362c8d33c`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 10.7 KB (10652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5821dc03875268203466d1599daa966b4ca91b58ed9b5391b9d3274d649c7efa`  
		Last Modified: Wed, 06 Apr 2022 06:34:38 GMT  
		Size: 5.7 MB (5698843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.3-kernel-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:dad922668d5e602332f9061eece1f0c4d46a79ea4d45086948e381b3708d4813
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.3 MB (181274433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a699b2b3aa112b11608f8c6e08565c02239c284fa3c309424ee1731fc850f935`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 06 Apr 2022 03:35:14 GMT
ADD file:1dc494089c70f6414b0a1f5e2e09605266508bf5ec19e1e2fb17028253f8953d in / 
# Wed, 06 Apr 2022 03:35:17 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 05:13:40 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Apr 2022 05:14:24 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 05:14:31 GMT
ENV JAVA_VERSION=8.0.7.5
# Wed, 06 Apr 2022 05:15:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Apr 2022 05:15:55 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 11:00:44 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:00:46 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:00:50 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 11:00:53 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 11:00:56 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 11:00:59 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 11:01:01 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 11:01:03 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 11:01:07 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 11:01:47 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 11:01:52 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 11:01:57 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 11:02:02 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:02:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 11:02:29 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 11:02:31 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 11:02:43 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 11:03:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 11:03:16 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 11:03:22 GMT
USER 1001
# Wed, 06 Apr 2022 11:03:28 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 11:03:32 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 11:03:34 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:74c6ac89233d470993bd9d67b39dc7ccb63096b55dc274e26eb50345bbecdcd8`  
		Last Modified: Tue, 05 Apr 2022 13:13:08 GMT  
		Size: 30.4 MB (30438429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdbaeb83a31ef16299d247a8ff263c6635af307374780bb9be69adac828283a`  
		Last Modified: Wed, 06 Apr 2022 05:19:24 GMT  
		Size: 3.1 MB (3082224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c2b3b642229c677b19f97c99ecf42203b8d144e161b096bac2c2f2423096b3`  
		Last Modified: Wed, 06 Apr 2022 05:19:37 GMT  
		Size: 128.3 MB (128315500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607319fec708d071582f7068356a9b783452155ba745e3ae2a1ee5ff70006816`  
		Last Modified: Wed, 06 Apr 2022 12:00:17 GMT  
		Size: 14.1 MB (14080204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db26f8d06474b6cdae2a54e5b37464ae2d95059cad5bf4f189066796933a20b`  
		Last Modified: Wed, 06 Apr 2022 12:00:12 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c1989f41a81f220c80b3443f5b96a49f0372f9d53626c1551cdb7c72835b58`  
		Last Modified: Wed, 06 Apr 2022 12:00:12 GMT  
		Size: 9.7 KB (9677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3bfd5a575c436bbb31c349cb945f2f841da5996f2fe41fe71c3a5c1c9cc2fd`  
		Last Modified: Wed, 06 Apr 2022 12:00:12 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96179275284d5d42953fdbb04b7c28b376c018e18dc4e7fa6acadebcd137663a`  
		Last Modified: Wed, 06 Apr 2022 12:00:13 GMT  
		Size: 10.7 KB (10670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df489a3f9e1f8998afa4e608455726d81d3a58818050d61fd27c6c7b77244af`  
		Last Modified: Wed, 06 Apr 2022 12:00:13 GMT  
		Size: 5.3 MB (5336752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:22.0.0.3-kernel-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:0a8dab18f831e1dc83abcb79ce0d73103ef4032d33212a93f56c8ba371202aca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.8 MB (173791762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a554922d9f557cd093c15daaaeb857d95d49d423933d9535fb70bd85e16b9822`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Apr 2022 22:41:55 GMT
ADD file:7da6edcff7f600bf3a5d740cd585065c6b3748ff587c0627def91686d1bfe54d in / 
# Tue, 05 Apr 2022 22:41:57 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:04:20 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 05 Apr 2022 23:04:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:04:27 GMT
ENV JAVA_VERSION=8.0.7.5
# Tue, 05 Apr 2022 23:05:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 05 Apr 2022 23:05:10 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 00:21:45 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:21:45 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:21:45 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 00:21:45 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 00:21:45 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 00:21:46 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 00:21:46 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 00:21:46 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 00:21:46 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 00:22:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:22:00 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 00:22:00 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 00:22:01 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:22:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 00:22:03 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 00:22:03 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 00:22:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 00:22:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 00:22:13 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 00:22:13 GMT
USER 1001
# Wed, 06 Apr 2022 00:22:13 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 00:22:14 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 00:22:14 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:4b0f8a5e4614be4866f08e8772b57664127164f512df03d05a52607176caa02f`  
		Last Modified: Tue, 05 Apr 2022 13:13:37 GMT  
		Size: 25.4 MB (25365860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1df112729db94ceb85cc2f4f1a8a29c4c17240f3414e928932240687367857b`  
		Last Modified: Tue, 05 Apr 2022 23:07:59 GMT  
		Size: 2.7 MB (2676913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7842fa8c2deed61ffe9a36afd3c1544e042b88e440ab57c28e1732e356ea75df`  
		Last Modified: Tue, 05 Apr 2022 23:08:07 GMT  
		Size: 125.8 MB (125807378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404f68c2321c29cbc1068910410523410cf5f547bd14a1a39d22a191b7af2f2c`  
		Last Modified: Wed, 06 Apr 2022 00:59:35 GMT  
		Size: 14.1 MB (14079579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae1055a4b0be252bcf172f8c6844707d527fcef2a35187c9569bef098a77c18`  
		Last Modified: Wed, 06 Apr 2022 00:59:32 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc478f125deb368d73eb16801b69efb288cb07b229ff40ef29a31cd1fec805c`  
		Last Modified: Wed, 06 Apr 2022 00:59:32 GMT  
		Size: 9.7 KB (9682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90d9b68d251175efb44f7e467b8bc09edacfc0fbf0d138d33684cfd78d72d9f`  
		Last Modified: Wed, 06 Apr 2022 00:59:32 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d346a08c2d95ddc678ee0d514318700fdbbc867edbdc372f52a1d50792cf92af`  
		Last Modified: Wed, 06 Apr 2022 00:59:33 GMT  
		Size: 10.7 KB (10657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79772bc444250adebe9820159101675bd0b319704a1298e7b58cc96a2fc91830`  
		Last Modified: Wed, 06 Apr 2022 00:59:33 GMT  
		Size: 5.8 MB (5840724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:full`

```console
$ docker pull websphere-liberty@sha256:8de0b824af28b3746a3c6125fedbb83a9280b825b1e923403306e79f722c376f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:cda65fcc714caba7e3c36f5b7435e9bdfc3ac25a35a1d19d6a4131202eb2db7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **458.4 MB (458358013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5ac205b973d5c45f76f1d8f62de7d9666fa8edc73a87e83caf63db1a09b0df9`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:42 GMT
ADD file:8a4ddbd462c1dd2016c64bd71ea6b5dba2ac4934bfd235a04d55b364666b67d1 in / 
# Tue, 05 Apr 2022 22:20:43 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 04:11:03 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Apr 2022 04:11:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:11:10 GMT
ENV JAVA_VERSION=8.0.7.5
# Wed, 06 Apr 2022 04:11:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Apr 2022 04:11:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 06:04:50 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:04:50 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:04:50 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 06:04:50 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 06:04:50 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 06:04:50 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 06:04:51 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 06:04:51 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 06:04:51 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 06:05:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 06:05:01 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 06:05:01 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 06:05:02 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:05:03 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 06:05:03 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 06:05:03 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 06:05:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 06:05:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 06:05:13 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 06:05:13 GMT
USER 1001
# Wed, 06 Apr 2022 06:05:14 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 06:05:14 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 06:05:14 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 06:06:04 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:06:04 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 06:09:55 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 06:09:56 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 06:10:33 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:08a6abff89437fab99b52abbefed82ea907f12845c30eeb94f6b93c69be93166`  
		Last Modified: Tue, 05 Apr 2022 13:10:59 GMT  
		Size: 26.7 MB (26708938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfba7ea970cb1c55200b82df4d841cb3aeceb410b11a8979aa633a92e7d236b`  
		Last Modified: Wed, 06 Apr 2022 04:13:29 GMT  
		Size: 3.0 MB (2959903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7928eec80454bb70ea4d40960304e706827316397e2721ec34143d7e471d489`  
		Last Modified: Wed, 06 Apr 2022 04:13:39 GMT  
		Size: 128.8 MB (128801744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e8321e19197f2773b582a498e2c352f378d117442244e67ab76160b26c151`  
		Last Modified: Wed, 06 Apr 2022 06:34:41 GMT  
		Size: 14.1 MB (14079475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f525ec02b7acf591d7d8eec0bc9312b4d67404d39b2fe6b867cbdd75cda5957`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24de75b5ad0e32a1538636e8cf2db791b896dda43206f4b53cd75447dcdd9d69`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 9.7 KB (9680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17671817a6482e1aab160a13024a37aa3725d833b5e1fe872e40c965b3e60c2`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd49fec10585cc3bbdc3a0fb3580e26135a7b7910e8fef1cc1cded362c8d33c`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 10.7 KB (10652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5821dc03875268203466d1599daa966b4ca91b58ed9b5391b9d3274d649c7efa`  
		Last Modified: Wed, 06 Apr 2022 06:34:38 GMT  
		Size: 5.7 MB (5698843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c243f60957de1ee44d01c6baaae691fe8078ff83354adf037360a605c61e29f0`  
		Last Modified: Wed, 06 Apr 2022 06:35:23 GMT  
		Size: 264.0 MB (263977874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bea240e7db6ec28462ead5dea5d2b49793e7ca3048380006748d9551ae47aca`  
		Last Modified: Wed, 06 Apr 2022 06:35:09 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf55c107ae9a8dec5f029da6a473b1e6a1de8413e84cbabacf8ee2932c9c6eb5`  
		Last Modified: Wed, 06 Apr 2022 06:35:12 GMT  
		Size: 16.1 MB (16108990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:c97b5678d350c594cbcbd9036c7bb6eb551c40d1fc684f6deba01863d86c196c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **459.4 MB (459380904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92453735197d834aebbc804122ab90fd2bca3463f14bdd638c9a611e89ee0f6c`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 06 Apr 2022 03:35:14 GMT
ADD file:1dc494089c70f6414b0a1f5e2e09605266508bf5ec19e1e2fb17028253f8953d in / 
# Wed, 06 Apr 2022 03:35:17 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 05:13:40 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Apr 2022 05:14:24 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 05:14:31 GMT
ENV JAVA_VERSION=8.0.7.5
# Wed, 06 Apr 2022 05:15:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Apr 2022 05:15:55 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 11:00:44 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:00:46 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:00:50 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 11:00:53 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 11:00:56 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 11:00:59 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 11:01:01 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 11:01:03 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 11:01:07 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 11:01:47 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 11:01:52 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 11:01:57 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 11:02:02 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:02:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 11:02:29 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 11:02:31 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 11:02:43 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 11:03:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 11:03:16 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 11:03:22 GMT
USER 1001
# Wed, 06 Apr 2022 11:03:28 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 11:03:32 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 11:03:34 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 11:12:16 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:12:20 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 11:17:19 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 11:17:36 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 11:19:12 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:74c6ac89233d470993bd9d67b39dc7ccb63096b55dc274e26eb50345bbecdcd8`  
		Last Modified: Tue, 05 Apr 2022 13:13:08 GMT  
		Size: 30.4 MB (30438429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdbaeb83a31ef16299d247a8ff263c6635af307374780bb9be69adac828283a`  
		Last Modified: Wed, 06 Apr 2022 05:19:24 GMT  
		Size: 3.1 MB (3082224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c2b3b642229c677b19f97c99ecf42203b8d144e161b096bac2c2f2423096b3`  
		Last Modified: Wed, 06 Apr 2022 05:19:37 GMT  
		Size: 128.3 MB (128315500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607319fec708d071582f7068356a9b783452155ba745e3ae2a1ee5ff70006816`  
		Last Modified: Wed, 06 Apr 2022 12:00:17 GMT  
		Size: 14.1 MB (14080204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db26f8d06474b6cdae2a54e5b37464ae2d95059cad5bf4f189066796933a20b`  
		Last Modified: Wed, 06 Apr 2022 12:00:12 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c1989f41a81f220c80b3443f5b96a49f0372f9d53626c1551cdb7c72835b58`  
		Last Modified: Wed, 06 Apr 2022 12:00:12 GMT  
		Size: 9.7 KB (9677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3bfd5a575c436bbb31c349cb945f2f841da5996f2fe41fe71c3a5c1c9cc2fd`  
		Last Modified: Wed, 06 Apr 2022 12:00:12 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96179275284d5d42953fdbb04b7c28b376c018e18dc4e7fa6acadebcd137663a`  
		Last Modified: Wed, 06 Apr 2022 12:00:13 GMT  
		Size: 10.7 KB (10670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df489a3f9e1f8998afa4e608455726d81d3a58818050d61fd27c6c7b77244af`  
		Last Modified: Wed, 06 Apr 2022 12:00:13 GMT  
		Size: 5.3 MB (5336752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b042d816e5dae6c615a67e99c9c146f9361cb053c7191a28453ee4bac700dd`  
		Last Modified: Wed, 06 Apr 2022 12:01:20 GMT  
		Size: 264.0 MB (263979859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27a22ff3e3a47f2f395eea6bcdf51b5900894b8bc4088f6bb5a568e5faa585e`  
		Last Modified: Wed, 06 Apr 2022 12:00:57 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395acfb1d10392c0b8bd138f86cd3d941e8ed4e3df73d3dddc2d25c5e1cd20ba`  
		Last Modified: Wed, 06 Apr 2022 12:01:00 GMT  
		Size: 14.1 MB (14125664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:17a16ee52bccd25691b4511b3a476c3b9e8b89db8bb57e2cad48f1a27f1325bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **453.8 MB (453776780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f6c02bef0033fdf780cd7e119e505dd2cc3448e877dacc650f05f9ab493896b`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Apr 2022 22:41:55 GMT
ADD file:7da6edcff7f600bf3a5d740cd585065c6b3748ff587c0627def91686d1bfe54d in / 
# Tue, 05 Apr 2022 22:41:57 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:04:20 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 05 Apr 2022 23:04:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:04:27 GMT
ENV JAVA_VERSION=8.0.7.5
# Tue, 05 Apr 2022 23:05:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 05 Apr 2022 23:05:10 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 00:21:45 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:21:45 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:21:45 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 00:21:45 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 00:21:45 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 00:21:46 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 00:21:46 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 00:21:46 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 00:21:46 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 00:22:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:22:00 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 00:22:00 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 00:22:01 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:22:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 00:22:03 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 00:22:03 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 00:22:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 00:22:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 00:22:13 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 00:22:13 GMT
USER 1001
# Wed, 06 Apr 2022 00:22:13 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 00:22:14 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 00:22:14 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 00:23:26 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:23:27 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 00:28:01 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 00:28:10 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 00:28:39 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:4b0f8a5e4614be4866f08e8772b57664127164f512df03d05a52607176caa02f`  
		Last Modified: Tue, 05 Apr 2022 13:13:37 GMT  
		Size: 25.4 MB (25365860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1df112729db94ceb85cc2f4f1a8a29c4c17240f3414e928932240687367857b`  
		Last Modified: Tue, 05 Apr 2022 23:07:59 GMT  
		Size: 2.7 MB (2676913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7842fa8c2deed61ffe9a36afd3c1544e042b88e440ab57c28e1732e356ea75df`  
		Last Modified: Tue, 05 Apr 2022 23:08:07 GMT  
		Size: 125.8 MB (125807378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404f68c2321c29cbc1068910410523410cf5f547bd14a1a39d22a191b7af2f2c`  
		Last Modified: Wed, 06 Apr 2022 00:59:35 GMT  
		Size: 14.1 MB (14079579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae1055a4b0be252bcf172f8c6844707d527fcef2a35187c9569bef098a77c18`  
		Last Modified: Wed, 06 Apr 2022 00:59:32 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc478f125deb368d73eb16801b69efb288cb07b229ff40ef29a31cd1fec805c`  
		Last Modified: Wed, 06 Apr 2022 00:59:32 GMT  
		Size: 9.7 KB (9682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90d9b68d251175efb44f7e467b8bc09edacfc0fbf0d138d33684cfd78d72d9f`  
		Last Modified: Wed, 06 Apr 2022 00:59:32 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d346a08c2d95ddc678ee0d514318700fdbbc867edbdc372f52a1d50792cf92af`  
		Last Modified: Wed, 06 Apr 2022 00:59:33 GMT  
		Size: 10.7 KB (10657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79772bc444250adebe9820159101675bd0b319704a1298e7b58cc96a2fc91830`  
		Last Modified: Wed, 06 Apr 2022 00:59:33 GMT  
		Size: 5.8 MB (5840724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af3906793f5b93df770a0e9c8ab76701e7a7462c459753b23abeb8927f0be8f`  
		Last Modified: Wed, 06 Apr 2022 01:00:07 GMT  
		Size: 264.0 MB (263980552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc4cd25be3f31eced3efee7946ca0b82fb018fd5d8a2ca3ef863f738de062ae`  
		Last Modified: Wed, 06 Apr 2022 00:59:55 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4ee76efe1d5ce46952511f6eabd0cc40ccf205b07c26582d2504d6d50a868c`  
		Last Modified: Wed, 06 Apr 2022 00:59:57 GMT  
		Size: 16.0 MB (16003518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:271c814dc860192c177b3159e377a0cb854cff53852b21f55468abe1805ebffd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:9797600f2aea0ebdb8aed586ea0a80f7176bab06427609089b927974c406127b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.1 MB (392082245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a1412f68bc777621f23788740606e12ab92313a8021bf33b1d76fde065868ec`
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
# Tue, 05 Apr 2022 23:31:52 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Tue, 05 Apr 2022 23:32:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 05 Apr 2022 23:32:58 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 23:32:58 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 05 Apr 2022 23:33:33 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 06 Apr 2022 06:05:18 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:05:18 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:05:18 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 06:05:18 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 06:05:18 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 06:05:18 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 06:05:18 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 06:05:18 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 06:05:19 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 06:05:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 06:05:27 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 06:05:27 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 06:05:27 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:05:28 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 06:05:28 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 06:05:28 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 06:05:29 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 06:05:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 06:05:37 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 06:05:37 GMT
USER 1001
# Wed, 06 Apr 2022 06:05:37 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 06:05:37 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 06:05:37 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 06:10:42 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:10:42 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 06:14:23 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 06:14:24 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 06:14:58 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:2de664fdc03716f9363ceadd4dd17d7e1b14e86037b9096951d5742bcba8b7a7`  
		Last Modified: Tue, 05 Apr 2022 23:39:15 GMT  
		Size: 47.7 MB (47658316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73ebbc826a0dbf1766cf9d2329ac833ae344d2d462f4ad82159b63d7b58e41b`  
		Last Modified: Tue, 05 Apr 2022 23:39:09 GMT  
		Size: 4.3 MB (4333203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6132a1e30ebb061befc1dc524bec1dd16d89400628c2898a924654e48fe2fea0`  
		Last Modified: Wed, 06 Apr 2022 06:34:52 GMT  
		Size: 14.2 MB (14176948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f87590a8053062ea031a350fabd17c38798cf922f91301bcec7562cbca5c990`  
		Last Modified: Wed, 06 Apr 2022 06:34:48 GMT  
		Size: 688.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abedd88d5657c41d189250b3464751eb245af279284318677984c98dd1a92fa`  
		Last Modified: Wed, 06 Apr 2022 06:34:48 GMT  
		Size: 9.7 KB (9675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf381e38f8a29f5f63826328fbb4127a1c9a5c62f9a87b7a9c9229f30f0d84a`  
		Last Modified: Wed, 06 Apr 2022 06:34:48 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5ed086f03616c21833af3573ed3ebc2a7be3ca035cbff4ac0539b3cafcfd17`  
		Last Modified: Wed, 06 Apr 2022 06:34:48 GMT  
		Size: 10.7 KB (10651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a868e8fe31784701d1a577402dc0ca1c8414d996e92ea9562de4906604154089`  
		Last Modified: Wed, 06 Apr 2022 06:34:49 GMT  
		Size: 2.6 MB (2563936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20985f63df3a4adc843b7a4e0d223bba988fd56baa9f2639a234a3bf6c2da369`  
		Last Modified: Wed, 06 Apr 2022 06:35:46 GMT  
		Size: 264.0 MB (263977804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca66295c5b316ec0deb734ad793c6ccc3ac8754f319ebce0928e93cf80222fa`  
		Last Modified: Wed, 06 Apr 2022 06:35:33 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdc0db0f88390acf85409ce8b9e5b67f7e6720aad16a73b79f1f111a968ad4c`  
		Last Modified: Wed, 06 Apr 2022 06:35:35 GMT  
		Size: 14.8 MB (14753445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:ace0e86e8e2660a4fadae29b799f3e25072d21d2db140a29d078114c64e51924
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.5 MB (395527289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7da5b44a87bd4293e3ae41575322dfa6f4d1ca0253d30fc0afeb10503a08701b`
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
# Wed, 06 Apr 2022 05:25:20 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Wed, 06 Apr 2022 05:28:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 06 Apr 2022 05:28:29 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 05:28:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 06 Apr 2022 05:29:30 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 06 Apr 2022 11:03:56 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:04:03 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:04:08 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 11:04:10 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 11:04:12 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 11:04:15 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 11:04:18 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 11:04:21 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 11:04:24 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 11:05:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 11:05:07 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 11:05:12 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 11:05:16 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:05:29 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 11:05:32 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 11:05:35 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 11:05:45 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 11:06:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 11:06:14 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 11:06:18 GMT
USER 1001
# Wed, 06 Apr 2022 11:06:21 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 11:06:27 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 11:06:29 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 11:19:27 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:19:31 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 11:24:24 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 11:24:30 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 11:25:33 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:b6584e4eaf032ab0a077066aaf7fed665eb2a8f3602e32470a2876ef90b88061`  
		Last Modified: Wed, 06 Apr 2022 05:42:06 GMT  
		Size: 48.4 MB (48356007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b610dbba5e90b2e3952904cb87b4c157a9a5130c86608dcbb6c497386be16e`  
		Last Modified: Wed, 06 Apr 2022 05:41:59 GMT  
		Size: 3.3 MB (3346135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95ae83fb73bece18f1fa8f40c395ae30eef41eebf1e48a38b2b9dbcd8e1d49c`  
		Last Modified: Wed, 06 Apr 2022 12:00:32 GMT  
		Size: 14.2 MB (14177015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86f956bcffb8404cc6684e7a66edb75965ee0f8b0f3a604f6c32425db347929`  
		Last Modified: Wed, 06 Apr 2022 12:00:27 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08016258ef4a64fde96e9d147484fe3e65a08cb41cee929bd1884553993ff80`  
		Last Modified: Wed, 06 Apr 2022 12:00:26 GMT  
		Size: 9.7 KB (9675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00695331e2e0491cc7528ef72c22343d7efdf0dd9805979574730aedaca08306`  
		Last Modified: Wed, 06 Apr 2022 12:00:26 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbcd96946f527cfb1cd5e6f585ec054d814e2a3896889a637d4e4a39cde58f5`  
		Last Modified: Wed, 06 Apr 2022 12:00:27 GMT  
		Size: 10.7 KB (10666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fc0431eea1ff91d5ec2ea2499d23b1b529f2e20e12ada3774a61b58c504fe4`  
		Last Modified: Wed, 06 Apr 2022 12:00:27 GMT  
		Size: 2.5 MB (2498053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4769339e764d724355c2701c937c017208a84bf442513b37fffc9a0565b4c47e`  
		Last Modified: Wed, 06 Apr 2022 12:01:59 GMT  
		Size: 264.0 MB (263980230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de22bb02b2b14b4da0dbddb55ec62288106a4b909a5714ee066809dd45ff4ea6`  
		Last Modified: Wed, 06 Apr 2022 12:01:35 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a22db6e2d685b28fb7c4225daac663469a0b034a02d3a4b64a02bd8086444e`  
		Last Modified: Wed, 06 Apr 2022 12:01:41 GMT  
		Size: 12.7 MB (12651538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:1ffa26ba4ed12d7607b3f043784a1b8375b8b08a02c8acfe02b8d4dec7d96d73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **388.9 MB (388893052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ffacf41e1cc0b8ee433ae1a73ed72f2866712dea3024b1a084e1f0239ba5703`
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
# Tue, 05 Apr 2022 23:37:27 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Tue, 05 Apr 2022 23:38:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 05 Apr 2022 23:38:30 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 23:38:30 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 05 Apr 2022 23:39:03 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 06 Apr 2022 00:22:26 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:22:27 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:22:27 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 00:22:27 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 00:22:27 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 00:22:27 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 00:22:27 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 00:22:28 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 00:22:28 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 00:22:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:22:39 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 00:22:39 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 00:22:40 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:22:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 00:22:41 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 00:22:41 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 00:22:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 00:22:47 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 00:22:47 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 00:22:48 GMT
USER 1001
# Wed, 06 Apr 2022 00:22:48 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 00:22:48 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 00:22:48 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 00:28:51 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:28:51 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 00:33:21 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 00:33:26 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 00:33:52 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:0efef42000170e3bcdd94a2519a9339d346b977d75a0129e443ce90e974708ce`  
		Last Modified: Tue, 05 Apr 2022 23:44:45 GMT  
		Size: 46.7 MB (46692257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b82868a62b6c97ba5baae49e8f092d01163d3296a2447501f70129c2eb3277`  
		Last Modified: Tue, 05 Apr 2022 23:44:40 GMT  
		Size: 4.3 MB (4308425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058f842793768c6a4228763d95efeb7ddfaea1518fbeef298795d623064b8c04`  
		Last Modified: Wed, 06 Apr 2022 00:59:42 GMT  
		Size: 14.2 MB (14176985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a088cccd826c8de31e45c82202f3d0fd45572b7fd81409696fd14665fa7cde`  
		Last Modified: Wed, 06 Apr 2022 00:59:40 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f047879900349daf331d78bca6b10df39e0e6c83a732d77bffb4af8c34e26ef3`  
		Last Modified: Wed, 06 Apr 2022 00:59:40 GMT  
		Size: 9.7 KB (9676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a79c5873bc6c06caf02c6cd195ad6a736a03dabf60d71edacaeeedc1bca46a`  
		Last Modified: Wed, 06 Apr 2022 00:59:40 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26f79dcfee7280c24a869c0861196eda62e7a7db5e2571b47b72a9cc3f9e188`  
		Last Modified: Wed, 06 Apr 2022 00:59:40 GMT  
		Size: 10.7 KB (10655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b66e645849a3ac3034c982f9902b4477df8359237dc14e4b782a929ffeeea05`  
		Last Modified: Wed, 06 Apr 2022 00:59:40 GMT  
		Size: 2.6 MB (2556370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a251890d9a5809c5c1ac9a554925afed3b7b0fb47baf9dd2e56ecf4d2c1cb51`  
		Last Modified: Wed, 06 Apr 2022 01:00:28 GMT  
		Size: 264.0 MB (263979732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a02373f0608ae3251a9470df381d9f73bd0b0a869777fe0b906a644cce53ee`  
		Last Modified: Wed, 06 Apr 2022 01:00:16 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b675630eee794075b80d2bc070552a388f2b2462ca66cfb1675fa58b30fb5a7a`  
		Last Modified: Wed, 06 Apr 2022 01:00:18 GMT  
		Size: 14.3 MB (14333812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:full-java17-openj9`

```console
$ docker pull websphere-liberty@sha256:7bbe668c7134fef50c686219dbeb57f4a1ee5daa39c1d98a07ba288cb9984bbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full-java17-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:a1f224fb2b02fe1abcc7ef2f69ad3074debf530e19b079bf40a24d3d3488de90
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.9 MB (392888570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7addf32e4ac1f24f011bad464204a44016e8982458ec38060731e87739be2cf2`
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
# Wed, 06 Apr 2022 06:15:05 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:15:05 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 06:18:49 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 06:18:50 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 06:19:26 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:46f79396957baf2dbd1896fa475541cb5f4812ade98e99b9fa96890156c7930e`  
		Last Modified: Wed, 06 Apr 2022 06:36:08 GMT  
		Size: 264.0 MB (263977221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4288ba967a1b39f55f94b7b0f114abb2bb52b4a830d73cbae02cb57d3edcfda4`  
		Last Modified: Wed, 06 Apr 2022 06:35:54 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a25a3e4180aa053251898ee4164c137669da61a217d942de833f8222521138`  
		Last Modified: Wed, 06 Apr 2022 06:35:56 GMT  
		Size: 14.9 MB (14902322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java17-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:ecda3b2de80bfa580a08e73d1168ffa4a5b45ca2b6bc88bc7700df3222bab9d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.2 MB (396236120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5201d33f7c97805a986f71401c9f8427c827fa16eb465cfd01b6d80920439593`
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
# Wed, 06 Apr 2022 11:25:53 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:25:57 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 11:30:55 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 11:30:59 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 11:32:06 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:e25d61c85edc197b103a017fc7f613affcf103a0f46c39442245b0f02276be7f`  
		Last Modified: Wed, 06 Apr 2022 12:02:33 GMT  
		Size: 264.0 MB (263979505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b309a2a80174dffd819f9fbff3ed68ba27aaad395295105172978611ed1d922`  
		Last Modified: Wed, 06 Apr 2022 12:02:09 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37432f78ffcb85dbcc85751152b01ff2e19e3e0a077a2be6e2da9ca70b89e55`  
		Last Modified: Wed, 06 Apr 2022 12:02:13 GMT  
		Size: 13.3 MB (13269063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java17-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:217ba82fef2ad2de05e542110e7dcb8411d15e88a10da6400b37e425d4bae63c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **389.3 MB (389324009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e4ee585f25815c703fc836a7be581346c17146aa110d145bad15acebafc205e`
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
# Wed, 06 Apr 2022 00:34:14 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:34:14 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 00:38:41 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 00:38:46 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 00:39:10 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:ca35b4ac395d9d8742983ea27fd9ecd988ed12a5d4ebe7527618ce33897c131a`  
		Last Modified: Wed, 06 Apr 2022 01:00:48 GMT  
		Size: 264.0 MB (263979666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452d4cc5b4a3b6c1dd13b16fef1f730e76fca9f0ef8715c8fb90d06326dff62c`  
		Last Modified: Wed, 06 Apr 2022 01:00:37 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7963455bc01e7b072abde32795f8086fe33cbf0e9c6ffdfb1b610f50cdc7d0c1`  
		Last Modified: Wed, 06 Apr 2022 01:00:38 GMT  
		Size: 14.5 MB (14521744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:kernel`

```console
$ docker pull websphere-liberty@sha256:c49f2ec5c5a1a18b6417755bcb8e51bb167210c07d94578a08c2232f71418a29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:kernel` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:9e3edcb74de734f3cc5a6ba6c2b7e512bae73e107bf0e55323bc4136e9c64eb3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.3 MB (178270202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ba3ec0b3bf0b3fa6b9b4319be274cfbde67785b8f210f79e3b8e5382550b10a`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:42 GMT
ADD file:8a4ddbd462c1dd2016c64bd71ea6b5dba2ac4934bfd235a04d55b364666b67d1 in / 
# Tue, 05 Apr 2022 22:20:43 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 04:11:03 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Apr 2022 04:11:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:11:10 GMT
ENV JAVA_VERSION=8.0.7.5
# Wed, 06 Apr 2022 04:11:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Apr 2022 04:11:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 06:04:50 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:04:50 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:04:50 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 06:04:50 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 06:04:50 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 06:04:50 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 06:04:51 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 06:04:51 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 06:04:51 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 06:05:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 06:05:01 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 06:05:01 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 06:05:02 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:05:03 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 06:05:03 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 06:05:03 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 06:05:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 06:05:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 06:05:13 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 06:05:13 GMT
USER 1001
# Wed, 06 Apr 2022 06:05:14 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 06:05:14 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 06:05:14 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:08a6abff89437fab99b52abbefed82ea907f12845c30eeb94f6b93c69be93166`  
		Last Modified: Tue, 05 Apr 2022 13:10:59 GMT  
		Size: 26.7 MB (26708938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfba7ea970cb1c55200b82df4d841cb3aeceb410b11a8979aa633a92e7d236b`  
		Last Modified: Wed, 06 Apr 2022 04:13:29 GMT  
		Size: 3.0 MB (2959903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7928eec80454bb70ea4d40960304e706827316397e2721ec34143d7e471d489`  
		Last Modified: Wed, 06 Apr 2022 04:13:39 GMT  
		Size: 128.8 MB (128801744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e8321e19197f2773b582a498e2c352f378d117442244e67ab76160b26c151`  
		Last Modified: Wed, 06 Apr 2022 06:34:41 GMT  
		Size: 14.1 MB (14079475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f525ec02b7acf591d7d8eec0bc9312b4d67404d39b2fe6b867cbdd75cda5957`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24de75b5ad0e32a1538636e8cf2db791b896dda43206f4b53cd75447dcdd9d69`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 9.7 KB (9680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17671817a6482e1aab160a13024a37aa3725d833b5e1fe872e40c965b3e60c2`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd49fec10585cc3bbdc3a0fb3580e26135a7b7910e8fef1cc1cded362c8d33c`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 10.7 KB (10652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5821dc03875268203466d1599daa966b4ca91b58ed9b5391b9d3274d649c7efa`  
		Last Modified: Wed, 06 Apr 2022 06:34:38 GMT  
		Size: 5.7 MB (5698843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:dad922668d5e602332f9061eece1f0c4d46a79ea4d45086948e381b3708d4813
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.3 MB (181274433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a699b2b3aa112b11608f8c6e08565c02239c284fa3c309424ee1731fc850f935`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 06 Apr 2022 03:35:14 GMT
ADD file:1dc494089c70f6414b0a1f5e2e09605266508bf5ec19e1e2fb17028253f8953d in / 
# Wed, 06 Apr 2022 03:35:17 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 05:13:40 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Apr 2022 05:14:24 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 05:14:31 GMT
ENV JAVA_VERSION=8.0.7.5
# Wed, 06 Apr 2022 05:15:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Apr 2022 05:15:55 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 11:00:44 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:00:46 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:00:50 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 11:00:53 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 11:00:56 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 11:00:59 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 11:01:01 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 11:01:03 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 11:01:07 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 11:01:47 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 11:01:52 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 11:01:57 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 11:02:02 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:02:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 11:02:29 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 11:02:31 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 11:02:43 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 11:03:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 11:03:16 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 11:03:22 GMT
USER 1001
# Wed, 06 Apr 2022 11:03:28 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 11:03:32 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 11:03:34 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:74c6ac89233d470993bd9d67b39dc7ccb63096b55dc274e26eb50345bbecdcd8`  
		Last Modified: Tue, 05 Apr 2022 13:13:08 GMT  
		Size: 30.4 MB (30438429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdbaeb83a31ef16299d247a8ff263c6635af307374780bb9be69adac828283a`  
		Last Modified: Wed, 06 Apr 2022 05:19:24 GMT  
		Size: 3.1 MB (3082224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c2b3b642229c677b19f97c99ecf42203b8d144e161b096bac2c2f2423096b3`  
		Last Modified: Wed, 06 Apr 2022 05:19:37 GMT  
		Size: 128.3 MB (128315500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607319fec708d071582f7068356a9b783452155ba745e3ae2a1ee5ff70006816`  
		Last Modified: Wed, 06 Apr 2022 12:00:17 GMT  
		Size: 14.1 MB (14080204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db26f8d06474b6cdae2a54e5b37464ae2d95059cad5bf4f189066796933a20b`  
		Last Modified: Wed, 06 Apr 2022 12:00:12 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c1989f41a81f220c80b3443f5b96a49f0372f9d53626c1551cdb7c72835b58`  
		Last Modified: Wed, 06 Apr 2022 12:00:12 GMT  
		Size: 9.7 KB (9677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3bfd5a575c436bbb31c349cb945f2f841da5996f2fe41fe71c3a5c1c9cc2fd`  
		Last Modified: Wed, 06 Apr 2022 12:00:12 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96179275284d5d42953fdbb04b7c28b376c018e18dc4e7fa6acadebcd137663a`  
		Last Modified: Wed, 06 Apr 2022 12:00:13 GMT  
		Size: 10.7 KB (10670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df489a3f9e1f8998afa4e608455726d81d3a58818050d61fd27c6c7b77244af`  
		Last Modified: Wed, 06 Apr 2022 12:00:13 GMT  
		Size: 5.3 MB (5336752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:0a8dab18f831e1dc83abcb79ce0d73103ef4032d33212a93f56c8ba371202aca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.8 MB (173791762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a554922d9f557cd093c15daaaeb857d95d49d423933d9535fb70bd85e16b9822`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Apr 2022 22:41:55 GMT
ADD file:7da6edcff7f600bf3a5d740cd585065c6b3748ff587c0627def91686d1bfe54d in / 
# Tue, 05 Apr 2022 22:41:57 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:04:20 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 05 Apr 2022 23:04:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:04:27 GMT
ENV JAVA_VERSION=8.0.7.5
# Tue, 05 Apr 2022 23:05:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 05 Apr 2022 23:05:10 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 00:21:45 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:21:45 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:21:45 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 00:21:45 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 00:21:45 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 00:21:46 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 00:21:46 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 00:21:46 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 00:21:46 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 00:22:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:22:00 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 00:22:00 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 00:22:01 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:22:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 00:22:03 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 00:22:03 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 00:22:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 00:22:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 00:22:13 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 00:22:13 GMT
USER 1001
# Wed, 06 Apr 2022 00:22:13 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 00:22:14 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 00:22:14 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:4b0f8a5e4614be4866f08e8772b57664127164f512df03d05a52607176caa02f`  
		Last Modified: Tue, 05 Apr 2022 13:13:37 GMT  
		Size: 25.4 MB (25365860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1df112729db94ceb85cc2f4f1a8a29c4c17240f3414e928932240687367857b`  
		Last Modified: Tue, 05 Apr 2022 23:07:59 GMT  
		Size: 2.7 MB (2676913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7842fa8c2deed61ffe9a36afd3c1544e042b88e440ab57c28e1732e356ea75df`  
		Last Modified: Tue, 05 Apr 2022 23:08:07 GMT  
		Size: 125.8 MB (125807378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404f68c2321c29cbc1068910410523410cf5f547bd14a1a39d22a191b7af2f2c`  
		Last Modified: Wed, 06 Apr 2022 00:59:35 GMT  
		Size: 14.1 MB (14079579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae1055a4b0be252bcf172f8c6844707d527fcef2a35187c9569bef098a77c18`  
		Last Modified: Wed, 06 Apr 2022 00:59:32 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc478f125deb368d73eb16801b69efb288cb07b229ff40ef29a31cd1fec805c`  
		Last Modified: Wed, 06 Apr 2022 00:59:32 GMT  
		Size: 9.7 KB (9682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90d9b68d251175efb44f7e467b8bc09edacfc0fbf0d138d33684cfd78d72d9f`  
		Last Modified: Wed, 06 Apr 2022 00:59:32 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d346a08c2d95ddc678ee0d514318700fdbbc867edbdc372f52a1d50792cf92af`  
		Last Modified: Wed, 06 Apr 2022 00:59:33 GMT  
		Size: 10.7 KB (10657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79772bc444250adebe9820159101675bd0b319704a1298e7b58cc96a2fc91830`  
		Last Modified: Wed, 06 Apr 2022 00:59:33 GMT  
		Size: 5.8 MB (5840724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:2004177a4e7200445aca1ba0270f9490fa23de84f6d610f98693cb918d34a7dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:kernel-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:8ce41452f4500cd47ad92e6805c35f5918273c14b929cfd2e174a2e294563fba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.4 MB (113350052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d77be323eea3d650decb6f7130da21769792ab442e397d990775fdd96699fda8`
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
# Tue, 05 Apr 2022 23:31:52 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Tue, 05 Apr 2022 23:32:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 05 Apr 2022 23:32:58 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 23:32:58 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 05 Apr 2022 23:33:33 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 06 Apr 2022 06:05:18 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:05:18 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:05:18 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 06:05:18 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 06:05:18 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 06:05:18 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 06:05:18 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 06:05:18 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 06:05:19 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 06:05:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 06:05:27 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 06:05:27 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 06:05:27 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:05:28 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 06:05:28 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 06:05:28 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 06:05:29 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 06:05:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 06:05:37 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 06:05:37 GMT
USER 1001
# Wed, 06 Apr 2022 06:05:37 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 06:05:37 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 06:05:37 GMT
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
	-	`sha256:2de664fdc03716f9363ceadd4dd17d7e1b14e86037b9096951d5742bcba8b7a7`  
		Last Modified: Tue, 05 Apr 2022 23:39:15 GMT  
		Size: 47.7 MB (47658316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73ebbc826a0dbf1766cf9d2329ac833ae344d2d462f4ad82159b63d7b58e41b`  
		Last Modified: Tue, 05 Apr 2022 23:39:09 GMT  
		Size: 4.3 MB (4333203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6132a1e30ebb061befc1dc524bec1dd16d89400628c2898a924654e48fe2fea0`  
		Last Modified: Wed, 06 Apr 2022 06:34:52 GMT  
		Size: 14.2 MB (14176948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f87590a8053062ea031a350fabd17c38798cf922f91301bcec7562cbca5c990`  
		Last Modified: Wed, 06 Apr 2022 06:34:48 GMT  
		Size: 688.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abedd88d5657c41d189250b3464751eb245af279284318677984c98dd1a92fa`  
		Last Modified: Wed, 06 Apr 2022 06:34:48 GMT  
		Size: 9.7 KB (9675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf381e38f8a29f5f63826328fbb4127a1c9a5c62f9a87b7a9c9229f30f0d84a`  
		Last Modified: Wed, 06 Apr 2022 06:34:48 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5ed086f03616c21833af3573ed3ebc2a7be3ca035cbff4ac0539b3cafcfd17`  
		Last Modified: Wed, 06 Apr 2022 06:34:48 GMT  
		Size: 10.7 KB (10651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a868e8fe31784701d1a577402dc0ca1c8414d996e92ea9562de4906604154089`  
		Last Modified: Wed, 06 Apr 2022 06:34:49 GMT  
		Size: 2.6 MB (2563936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:0181e3a088fbed78f05be0c5c664db7aae2ec526e5784e52411292fbe24fc2ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118894573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a42b286e66f0e555edc25ed96a891d292ed41695d877db432119bf4ee852c495`
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
# Wed, 06 Apr 2022 05:25:20 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Wed, 06 Apr 2022 05:28:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 06 Apr 2022 05:28:29 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 05:28:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 06 Apr 2022 05:29:30 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 06 Apr 2022 11:03:56 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:04:03 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:04:08 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 11:04:10 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 11:04:12 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 11:04:15 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 11:04:18 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 11:04:21 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 11:04:24 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 11:05:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 11:05:07 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 11:05:12 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 11:05:16 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:05:29 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 11:05:32 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 11:05:35 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 11:05:45 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 11:06:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 11:06:14 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 11:06:18 GMT
USER 1001
# Wed, 06 Apr 2022 11:06:21 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 11:06:27 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 11:06:29 GMT
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
	-	`sha256:b6584e4eaf032ab0a077066aaf7fed665eb2a8f3602e32470a2876ef90b88061`  
		Last Modified: Wed, 06 Apr 2022 05:42:06 GMT  
		Size: 48.4 MB (48356007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b610dbba5e90b2e3952904cb87b4c157a9a5130c86608dcbb6c497386be16e`  
		Last Modified: Wed, 06 Apr 2022 05:41:59 GMT  
		Size: 3.3 MB (3346135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95ae83fb73bece18f1fa8f40c395ae30eef41eebf1e48a38b2b9dbcd8e1d49c`  
		Last Modified: Wed, 06 Apr 2022 12:00:32 GMT  
		Size: 14.2 MB (14177015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86f956bcffb8404cc6684e7a66edb75965ee0f8b0f3a604f6c32425db347929`  
		Last Modified: Wed, 06 Apr 2022 12:00:27 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08016258ef4a64fde96e9d147484fe3e65a08cb41cee929bd1884553993ff80`  
		Last Modified: Wed, 06 Apr 2022 12:00:26 GMT  
		Size: 9.7 KB (9675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00695331e2e0491cc7528ef72c22343d7efdf0dd9805979574730aedaca08306`  
		Last Modified: Wed, 06 Apr 2022 12:00:26 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbcd96946f527cfb1cd5e6f585ec054d814e2a3896889a637d4e4a39cde58f5`  
		Last Modified: Wed, 06 Apr 2022 12:00:27 GMT  
		Size: 10.7 KB (10666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fc0431eea1ff91d5ec2ea2499d23b1b529f2e20e12ada3774a61b58c504fe4`  
		Last Modified: Wed, 06 Apr 2022 12:00:27 GMT  
		Size: 2.5 MB (2498053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:d7155eac65555d6fbef3279d48d1b15f44c0bc5788b56889187901d07734a8aa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110578561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:182d330bce80f26c52deb1c7070bbdcbf23a2b23357d1ad02d453e1d9b38875e`
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
# Tue, 05 Apr 2022 23:37:27 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Tue, 05 Apr 2022 23:38:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 05 Apr 2022 23:38:30 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 23:38:30 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 05 Apr 2022 23:39:03 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 06 Apr 2022 00:22:26 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:22:27 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:22:27 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 00:22:27 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 00:22:27 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 00:22:27 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 00:22:27 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 00:22:28 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 00:22:28 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 00:22:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:22:39 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 00:22:39 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 00:22:40 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:22:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 00:22:41 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 00:22:41 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 00:22:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 00:22:47 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 00:22:47 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 06 Apr 2022 00:22:48 GMT
USER 1001
# Wed, 06 Apr 2022 00:22:48 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 00:22:48 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 00:22:48 GMT
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
	-	`sha256:0efef42000170e3bcdd94a2519a9339d346b977d75a0129e443ce90e974708ce`  
		Last Modified: Tue, 05 Apr 2022 23:44:45 GMT  
		Size: 46.7 MB (46692257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b82868a62b6c97ba5baae49e8f092d01163d3296a2447501f70129c2eb3277`  
		Last Modified: Tue, 05 Apr 2022 23:44:40 GMT  
		Size: 4.3 MB (4308425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058f842793768c6a4228763d95efeb7ddfaea1518fbeef298795d623064b8c04`  
		Last Modified: Wed, 06 Apr 2022 00:59:42 GMT  
		Size: 14.2 MB (14176985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a088cccd826c8de31e45c82202f3d0fd45572b7fd81409696fd14665fa7cde`  
		Last Modified: Wed, 06 Apr 2022 00:59:40 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f047879900349daf331d78bca6b10df39e0e6c83a732d77bffb4af8c34e26ef3`  
		Last Modified: Wed, 06 Apr 2022 00:59:40 GMT  
		Size: 9.7 KB (9676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a79c5873bc6c06caf02c6cd195ad6a736a03dabf60d71edacaeeedc1bca46a`  
		Last Modified: Wed, 06 Apr 2022 00:59:40 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26f79dcfee7280c24a869c0861196eda62e7a7db5e2571b47b72a9cc3f9e188`  
		Last Modified: Wed, 06 Apr 2022 00:59:40 GMT  
		Size: 10.7 KB (10655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b66e645849a3ac3034c982f9902b4477df8359237dc14e4b782a929ffeeea05`  
		Last Modified: Wed, 06 Apr 2022 00:59:40 GMT  
		Size: 2.6 MB (2556370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

## `websphere-liberty:latest`

```console
$ docker pull websphere-liberty@sha256:8de0b824af28b3746a3c6125fedbb83a9280b825b1e923403306e79f722c376f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:latest` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:cda65fcc714caba7e3c36f5b7435e9bdfc3ac25a35a1d19d6a4131202eb2db7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **458.4 MB (458358013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5ac205b973d5c45f76f1d8f62de7d9666fa8edc73a87e83caf63db1a09b0df9`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:42 GMT
ADD file:8a4ddbd462c1dd2016c64bd71ea6b5dba2ac4934bfd235a04d55b364666b67d1 in / 
# Tue, 05 Apr 2022 22:20:43 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 04:11:03 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Apr 2022 04:11:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:11:10 GMT
ENV JAVA_VERSION=8.0.7.5
# Wed, 06 Apr 2022 04:11:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Apr 2022 04:11:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 06:04:50 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:04:50 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:04:50 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 06:04:50 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 06:04:50 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 06:04:50 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 06:04:51 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 06:04:51 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 06:04:51 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 06:05:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 06:05:01 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 06:05:01 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 06:05:02 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 06:05:03 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 06:05:03 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 06:05:03 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 06:05:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 06:05:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 06:05:13 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 06:05:13 GMT
USER 1001
# Wed, 06 Apr 2022 06:05:14 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 06:05:14 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 06:05:14 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 06:06:04 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 06:06:04 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 06:09:55 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 06:09:56 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 06:10:33 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:08a6abff89437fab99b52abbefed82ea907f12845c30eeb94f6b93c69be93166`  
		Last Modified: Tue, 05 Apr 2022 13:10:59 GMT  
		Size: 26.7 MB (26708938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfba7ea970cb1c55200b82df4d841cb3aeceb410b11a8979aa633a92e7d236b`  
		Last Modified: Wed, 06 Apr 2022 04:13:29 GMT  
		Size: 3.0 MB (2959903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7928eec80454bb70ea4d40960304e706827316397e2721ec34143d7e471d489`  
		Last Modified: Wed, 06 Apr 2022 04:13:39 GMT  
		Size: 128.8 MB (128801744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e8321e19197f2773b582a498e2c352f378d117442244e67ab76160b26c151`  
		Last Modified: Wed, 06 Apr 2022 06:34:41 GMT  
		Size: 14.1 MB (14079475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f525ec02b7acf591d7d8eec0bc9312b4d67404d39b2fe6b867cbdd75cda5957`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24de75b5ad0e32a1538636e8cf2db791b896dda43206f4b53cd75447dcdd9d69`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 9.7 KB (9680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17671817a6482e1aab160a13024a37aa3725d833b5e1fe872e40c965b3e60c2`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd49fec10585cc3bbdc3a0fb3580e26135a7b7910e8fef1cc1cded362c8d33c`  
		Last Modified: Wed, 06 Apr 2022 06:34:37 GMT  
		Size: 10.7 KB (10652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5821dc03875268203466d1599daa966b4ca91b58ed9b5391b9d3274d649c7efa`  
		Last Modified: Wed, 06 Apr 2022 06:34:38 GMT  
		Size: 5.7 MB (5698843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c243f60957de1ee44d01c6baaae691fe8078ff83354adf037360a605c61e29f0`  
		Last Modified: Wed, 06 Apr 2022 06:35:23 GMT  
		Size: 264.0 MB (263977874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bea240e7db6ec28462ead5dea5d2b49793e7ca3048380006748d9551ae47aca`  
		Last Modified: Wed, 06 Apr 2022 06:35:09 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf55c107ae9a8dec5f029da6a473b1e6a1de8413e84cbabacf8ee2932c9c6eb5`  
		Last Modified: Wed, 06 Apr 2022 06:35:12 GMT  
		Size: 16.1 MB (16108990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:c97b5678d350c594cbcbd9036c7bb6eb551c40d1fc684f6deba01863d86c196c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **459.4 MB (459380904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92453735197d834aebbc804122ab90fd2bca3463f14bdd638c9a611e89ee0f6c`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 06 Apr 2022 03:35:14 GMT
ADD file:1dc494089c70f6414b0a1f5e2e09605266508bf5ec19e1e2fb17028253f8953d in / 
# Wed, 06 Apr 2022 03:35:17 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 05:13:40 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 06 Apr 2022 05:14:24 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 05:14:31 GMT
ENV JAVA_VERSION=8.0.7.5
# Wed, 06 Apr 2022 05:15:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 06 Apr 2022 05:15:55 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 11:00:44 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:00:46 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:00:50 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 11:00:53 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 11:00:56 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 11:00:59 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 11:01:01 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 11:01:03 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 11:01:07 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 11:01:47 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 11:01:52 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 11:01:57 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 11:02:02 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 11:02:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 11:02:29 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 11:02:31 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 11:02:43 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 11:03:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 11:03:16 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 11:03:22 GMT
USER 1001
# Wed, 06 Apr 2022 11:03:28 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 11:03:32 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 11:03:34 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 11:12:16 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 11:12:20 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 11:17:19 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 11:17:36 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 11:19:12 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:74c6ac89233d470993bd9d67b39dc7ccb63096b55dc274e26eb50345bbecdcd8`  
		Last Modified: Tue, 05 Apr 2022 13:13:08 GMT  
		Size: 30.4 MB (30438429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdbaeb83a31ef16299d247a8ff263c6635af307374780bb9be69adac828283a`  
		Last Modified: Wed, 06 Apr 2022 05:19:24 GMT  
		Size: 3.1 MB (3082224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c2b3b642229c677b19f97c99ecf42203b8d144e161b096bac2c2f2423096b3`  
		Last Modified: Wed, 06 Apr 2022 05:19:37 GMT  
		Size: 128.3 MB (128315500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607319fec708d071582f7068356a9b783452155ba745e3ae2a1ee5ff70006816`  
		Last Modified: Wed, 06 Apr 2022 12:00:17 GMT  
		Size: 14.1 MB (14080204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db26f8d06474b6cdae2a54e5b37464ae2d95059cad5bf4f189066796933a20b`  
		Last Modified: Wed, 06 Apr 2022 12:00:12 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c1989f41a81f220c80b3443f5b96a49f0372f9d53626c1551cdb7c72835b58`  
		Last Modified: Wed, 06 Apr 2022 12:00:12 GMT  
		Size: 9.7 KB (9677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3bfd5a575c436bbb31c349cb945f2f841da5996f2fe41fe71c3a5c1c9cc2fd`  
		Last Modified: Wed, 06 Apr 2022 12:00:12 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96179275284d5d42953fdbb04b7c28b376c018e18dc4e7fa6acadebcd137663a`  
		Last Modified: Wed, 06 Apr 2022 12:00:13 GMT  
		Size: 10.7 KB (10670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df489a3f9e1f8998afa4e608455726d81d3a58818050d61fd27c6c7b77244af`  
		Last Modified: Wed, 06 Apr 2022 12:00:13 GMT  
		Size: 5.3 MB (5336752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b042d816e5dae6c615a67e99c9c146f9361cb053c7191a28453ee4bac700dd`  
		Last Modified: Wed, 06 Apr 2022 12:01:20 GMT  
		Size: 264.0 MB (263979859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27a22ff3e3a47f2f395eea6bcdf51b5900894b8bc4088f6bb5a568e5faa585e`  
		Last Modified: Wed, 06 Apr 2022 12:00:57 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395acfb1d10392c0b8bd138f86cd3d941e8ed4e3df73d3dddc2d25c5e1cd20ba`  
		Last Modified: Wed, 06 Apr 2022 12:01:00 GMT  
		Size: 14.1 MB (14125664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:17a16ee52bccd25691b4511b3a476c3b9e8b89db8bb57e2cad48f1a27f1325bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **453.8 MB (453776780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f6c02bef0033fdf780cd7e119e505dd2cc3448e877dacc650f05f9ab493896b`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 05 Apr 2022 22:41:55 GMT
ADD file:7da6edcff7f600bf3a5d740cd585065c6b3748ff587c0627def91686d1bfe54d in / 
# Tue, 05 Apr 2022 22:41:57 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:04:20 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 05 Apr 2022 23:04:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:04:27 GMT
ENV JAVA_VERSION=8.0.7.5
# Tue, 05 Apr 2022 23:05:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2036ff825599773d0da7ca65e526ef4653e8060b787e5f9a4967fa73756cb56';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f4639c53ae366cda315db5f504bf7596a9757d7dccb4be66cce6e447613672cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='0961aedeaab4801cadb3d7a327344e66ef5d7f982f9269d5a0e447e4699feee7';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2469075243605203690306e9022150b86da5e9b5c563bba7ae1c3413c65b9cbf';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='71abbc456c06850a3f557465e988b73ecf66a22d9fd7d8a57a03dc56849f06a4';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 05 Apr 2022 23:05:10 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 06 Apr 2022 00:21:45 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:21:45 GMT
ARG OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:21:45 GMT
ARG EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6
# Wed, 06 Apr 2022 00:21:45 GMT
ARG NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64
# Wed, 06 Apr 2022 00:21:45 GMT
ARG NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74
# Wed, 06 Apr 2022 00:21:46 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.3 org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 06 Apr 2022 00:21:46 GMT
ENV LIBERTY_VERSION=22.0.0_03
# Wed, 06 Apr 2022 00:21:46 GMT
ARG LIBERTY_URL
# Wed, 06 Apr 2022 00:21:46 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 06 Apr 2022 00:22:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:22:00 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 00:22:00 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.3 BuildLabel=cl220320220302-1100
# Wed, 06 Apr 2022 00:22:01 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 06 Apr 2022 00:22:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 06 Apr 2022 00:22:03 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 06 Apr 2022 00:22:03 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 06 Apr 2022 00:22:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 06 Apr 2022 00:22:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=7acdc571668fc49854fb20faf9f178391395ae8d81a124eb792b694fe535fcf6 NON_IBM_SHA=1f28b264cab4c9ddba00122a875b6fbeed97f5a22b3574f415752bbacc1d2b64 NOTICES_SHA=4e83e7efe96dced32fef7686938abe012711c0cd643f458e2bac260f2c7dae74 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 06 Apr 2022 00:22:13 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 06 Apr 2022 00:22:13 GMT
USER 1001
# Wed, 06 Apr 2022 00:22:13 GMT
EXPOSE 9080 9443
# Wed, 06 Apr 2022 00:22:14 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 06 Apr 2022 00:22:14 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 06 Apr 2022 00:23:26 GMT
ARG VERBOSE=false
# Wed, 06 Apr 2022 00:23:27 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 06 Apr 2022 00:28:01 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 06 Apr 2022 00:28:10 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 06 Apr 2022 00:28:39 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:4b0f8a5e4614be4866f08e8772b57664127164f512df03d05a52607176caa02f`  
		Last Modified: Tue, 05 Apr 2022 13:13:37 GMT  
		Size: 25.4 MB (25365860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1df112729db94ceb85cc2f4f1a8a29c4c17240f3414e928932240687367857b`  
		Last Modified: Tue, 05 Apr 2022 23:07:59 GMT  
		Size: 2.7 MB (2676913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7842fa8c2deed61ffe9a36afd3c1544e042b88e440ab57c28e1732e356ea75df`  
		Last Modified: Tue, 05 Apr 2022 23:08:07 GMT  
		Size: 125.8 MB (125807378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404f68c2321c29cbc1068910410523410cf5f547bd14a1a39d22a191b7af2f2c`  
		Last Modified: Wed, 06 Apr 2022 00:59:35 GMT  
		Size: 14.1 MB (14079579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae1055a4b0be252bcf172f8c6844707d527fcef2a35187c9569bef098a77c18`  
		Last Modified: Wed, 06 Apr 2022 00:59:32 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc478f125deb368d73eb16801b69efb288cb07b229ff40ef29a31cd1fec805c`  
		Last Modified: Wed, 06 Apr 2022 00:59:32 GMT  
		Size: 9.7 KB (9682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90d9b68d251175efb44f7e467b8bc09edacfc0fbf0d138d33684cfd78d72d9f`  
		Last Modified: Wed, 06 Apr 2022 00:59:32 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d346a08c2d95ddc678ee0d514318700fdbbc867edbdc372f52a1d50792cf92af`  
		Last Modified: Wed, 06 Apr 2022 00:59:33 GMT  
		Size: 10.7 KB (10657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79772bc444250adebe9820159101675bd0b319704a1298e7b58cc96a2fc91830`  
		Last Modified: Wed, 06 Apr 2022 00:59:33 GMT  
		Size: 5.8 MB (5840724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af3906793f5b93df770a0e9c8ab76701e7a7462c459753b23abeb8927f0be8f`  
		Last Modified: Wed, 06 Apr 2022 01:00:07 GMT  
		Size: 264.0 MB (263980552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc4cd25be3f31eced3efee7946ca0b82fb018fd5d8a2ca3ef863f738de062ae`  
		Last Modified: Wed, 06 Apr 2022 00:59:55 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4ee76efe1d5ce46952511f6eabd0cc40ccf205b07c26582d2504d6d50a868c`  
		Last Modified: Wed, 06 Apr 2022 00:59:57 GMT  
		Size: 16.0 MB (16003518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
