## `websphere-liberty:full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:3f9acdbfbd823f43da2e08d4cd0751546659700b94f38ceb91a7de355a9dfcd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:1516040854650d814182c395a081da4d1db8668c4e7176c8909bbef8f4f01b59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.5 MB (413476737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59237d77159ddd72c1e2b0e7858bb380fd69b745fa6b275a9a9e14fbdf769f2b`
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
# Wed, 10 Aug 2022 22:45:19 GMT
ENV JAVA_VERSION=jdk-11.0.16+8_openj9-0.33.0
# Wed, 10 Aug 2022 22:47:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='49dc05a3e9f3f99c5f8fa466261aa3e33a753694c67cabfa7d3f682e5a2e3685';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16%2B8_openj9-0.33.0/ibm-semeru-open-jre_aarch64_linux_11.0.16_8_openj9-0.33.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='552da889577571881ac58eb06877ca2fdadc12397f433b553b319674ee10a02d';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16%2B8_openj9-0.33.0/ibm-semeru-open-jre_ppc64le_linux_11.0.16_8_openj9-0.33.0.tar.gz';          ;;        amd64|x86_64)          ESUM='ba09711193b8b8664478f3f949b5320232f65c1bdf61f32a885d84de73c02767';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16%2B8_openj9-0.33.0/ibm-semeru-open-jre_x64_linux_11.0.16_8_openj9-0.33.0.tar.gz';          ;;        s390x)          ESUM='edfccd071e4276c51884cd89522b3be21fd2e44612f98f7a7d3dceb0c339a391';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16%2B8_openj9-0.33.0/ibm-semeru-open-jre_s390x_linux_11.0.16_8_openj9-0.33.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 10 Aug 2022 22:47:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Aug 2022 22:47:11 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 10 Aug 2022 22:47:46 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 11 Aug 2022 00:24:36 GMT
ARG VERBOSE=false
# Thu, 11 Aug 2022 00:24:36 GMT
ARG OPENJ9_SCC=true
# Thu, 11 Aug 2022 00:24:36 GMT
ARG EN_SHA=1558244d39947a6f608f757be932356607a9f2be6c4d6ab7def29e54512d70d0
# Thu, 11 Aug 2022 00:24:36 GMT
ARG NON_IBM_SHA=c5edb6e93c6ac1f3ee6b74780a7b265efaaaaed625efccdd6f8597b844469a50
# Thu, 11 Aug 2022 00:24:36 GMT
ARG NOTICES_SHA=8f92b2e9c7dff626fb7f4cc360e29be26e3497bcc626aca216144589bf3f9715
# Thu, 11 Aug 2022 00:24:36 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.8 org.opencontainers.image.revision=cl220820220719-1056 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 11 Aug 2022 00:24:36 GMT
ENV LIBERTY_VERSION=22.0.0_08
# Thu, 11 Aug 2022 00:24:37 GMT
ARG LIBERTY_URL
# Thu, 11 Aug 2022 00:24:37 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 11 Aug 2022 00:24:52 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1558244d39947a6f608f757be932356607a9f2be6c4d6ab7def29e54512d70d0 NON_IBM_SHA=c5edb6e93c6ac1f3ee6b74780a7b265efaaaaed625efccdd6f8597b844469a50 NOTICES_SHA=8f92b2e9c7dff626fb7f4cc360e29be26e3497bcc626aca216144589bf3f9715 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 00:24:52 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 00:24:53 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.8 BuildLabel=cl220820220719-1056
# Thu, 11 Aug 2022 00:24:53 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 11 Aug 2022 00:24:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1558244d39947a6f608f757be932356607a9f2be6c4d6ab7def29e54512d70d0 NON_IBM_SHA=c5edb6e93c6ac1f3ee6b74780a7b265efaaaaed625efccdd6f8597b844469a50 NOTICES_SHA=8f92b2e9c7dff626fb7f4cc360e29be26e3497bcc626aca216144589bf3f9715 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 11 Aug 2022 00:24:54 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Thu, 11 Aug 2022 00:24:54 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 11 Aug 2022 00:24:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1558244d39947a6f608f757be932356607a9f2be6c4d6ab7def29e54512d70d0 NON_IBM_SHA=c5edb6e93c6ac1f3ee6b74780a7b265efaaaaed625efccdd6f8597b844469a50 NOTICES_SHA=8f92b2e9c7dff626fb7f4cc360e29be26e3497bcc626aca216144589bf3f9715 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 11 Aug 2022 00:25:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1558244d39947a6f608f757be932356607a9f2be6c4d6ab7def29e54512d70d0 NON_IBM_SHA=c5edb6e93c6ac1f3ee6b74780a7b265efaaaaed625efccdd6f8597b844469a50 NOTICES_SHA=8f92b2e9c7dff626fb7f4cc360e29be26e3497bcc626aca216144589bf3f9715 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 11 Aug 2022 00:25:01 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 11 Aug 2022 00:25:02 GMT
USER 1001
# Thu, 11 Aug 2022 00:25:02 GMT
EXPOSE 9080 9443
# Thu, 11 Aug 2022 00:25:02 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 11 Aug 2022 00:25:02 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 11 Aug 2022 00:25:34 GMT
ARG VERBOSE=false
# Thu, 11 Aug 2022 00:25:34 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 11 Aug 2022 00:33:01 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Thu, 11 Aug 2022 00:33:02 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 11 Aug 2022 00:33:31 GMT
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
	-	`sha256:dae1b8d04e3b180095582892e267b24b70e7d91e19764b8dc0f9d4445b894cbf`  
		Last Modified: Wed, 10 Aug 2022 22:59:11 GMT  
		Size: 48.0 MB (48030809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd248a0b366f0ee9b5c5a6a6d9a8d0a9d4f20213a539fc3a11117b3f103405e5`  
		Last Modified: Wed, 10 Aug 2022 22:59:05 GMT  
		Size: 4.2 MB (4225214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a9f72f8ae33563198933457a4d65dc3c4612a923955eee19059231677dae54`  
		Last Modified: Thu, 11 Aug 2022 01:16:53 GMT  
		Size: 14.2 MB (14201891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855b400afd5d7a0de6c51764b2bb50b54c661a63a4bcdd650a15a001980072fb`  
		Last Modified: Thu, 11 Aug 2022 01:16:49 GMT  
		Size: 674.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b10a80c18d9488baac6342656865bbeda4baa3ff1a9a5a2a3cf810ff894c96a`  
		Last Modified: Thu, 11 Aug 2022 01:16:49 GMT  
		Size: 9.8 KB (9755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918924d8c46a6639ed1d322c8cf5ddd5c87e9a1fb69892b7799dc143fc392404`  
		Last Modified: Thu, 11 Aug 2022 01:16:49 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d640c23bbe1460e47983b18ce405944be52f4ffac13bc6614d7a3fc86f461109`  
		Last Modified: Thu, 11 Aug 2022 01:16:49 GMT  
		Size: 10.7 KB (10731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5e8e86c34b131deec90cab93f81bfe025f06f93bf6f36dda340c4534524970`  
		Last Modified: Thu, 11 Aug 2022 01:16:49 GMT  
		Size: 2.5 MB (2540303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9458443e2d74beb834d66521aadeadcdb4349e897be3e78ac771ef2aa960e56c`  
		Last Modified: Thu, 11 Aug 2022 01:17:27 GMT  
		Size: 285.3 MB (285267382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33336ab4749669cbe996310b6d9bc79402257b88f47cec9592ddbba9b75dae20`  
		Last Modified: Thu, 11 Aug 2022 01:17:11 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f8f30df013b8b2d255a3905bac1b1ac134cdc8f438f250f4add161c3fddca6`  
		Last Modified: Thu, 11 Aug 2022 01:17:14 GMT  
		Size: 14.6 MB (14586230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:c94c131d9f66a074c7a8689469f434906d92f6a83afa519efbfdc8d7ab013514
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **417.5 MB (417452959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86bb377ad871a4c22a7555655446f7f05f8043960353391733c7a8c5752a308a`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:01 GMT
ADD file:75dd7889d4feb83b8504153b5ea6873e4ab0e616a4f4489ea81fd055b6ce9def in / 
# Tue, 02 Aug 2022 01:31:03 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 03:18:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 03 Aug 2022 03:20:22 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:38:25 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1_openj9-0.33.1
# Tue, 23 Aug 2022 22:40:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='843557b315464818b70e6814288618e2e9645455ee67faa18ada299e6fa7c50f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jre_aarch64_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='8121e6d0b6e33e2816ebca5f624f00f44a6dd1a797cc58afd6ebe5e49bf713ee';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jre_ppc64le_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        amd64|x86_64)          ESUM='038a44d5c81f14bce6458040f7b4eec48535dcbbdc59e3c536d6adc3326b64c7';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jre_x64_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        s390x)          ESUM='fd1e07b5bdc028b39d870f9807208c6b41bfec8002e88bd78a4661684cab575b';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jre_s390x_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 23 Aug 2022 22:40:58 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 22:40:58 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 23 Aug 2022 22:41:35 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 23 Aug 2022 23:25:47 GMT
ARG VERBOSE=false
# Tue, 23 Aug 2022 23:25:47 GMT
ARG OPENJ9_SCC=true
# Tue, 23 Aug 2022 23:25:48 GMT
ARG EN_SHA=1558244d39947a6f608f757be932356607a9f2be6c4d6ab7def29e54512d70d0
# Tue, 23 Aug 2022 23:25:48 GMT
ARG NON_IBM_SHA=c5edb6e93c6ac1f3ee6b74780a7b265efaaaaed625efccdd6f8597b844469a50
# Tue, 23 Aug 2022 23:25:48 GMT
ARG NOTICES_SHA=8f92b2e9c7dff626fb7f4cc360e29be26e3497bcc626aca216144589bf3f9715
# Tue, 23 Aug 2022 23:25:49 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.8 org.opencontainers.image.revision=cl220820220719-1056 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 23 Aug 2022 23:25:49 GMT
ENV LIBERTY_VERSION=22.0.0_08
# Tue, 23 Aug 2022 23:25:49 GMT
ARG LIBERTY_URL
# Tue, 23 Aug 2022 23:25:50 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 23 Aug 2022 23:26:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1558244d39947a6f608f757be932356607a9f2be6c4d6ab7def29e54512d70d0 NON_IBM_SHA=c5edb6e93c6ac1f3ee6b74780a7b265efaaaaed625efccdd6f8597b844469a50 NOTICES_SHA=8f92b2e9c7dff626fb7f4cc360e29be26e3497bcc626aca216144589bf3f9715 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 23:26:31 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 23:26:31 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.8 BuildLabel=cl220820220719-1056
# Tue, 23 Aug 2022 23:26:32 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 23 Aug 2022 23:26:33 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1558244d39947a6f608f757be932356607a9f2be6c4d6ab7def29e54512d70d0 NON_IBM_SHA=c5edb6e93c6ac1f3ee6b74780a7b265efaaaaed625efccdd6f8597b844469a50 NOTICES_SHA=8f92b2e9c7dff626fb7f4cc360e29be26e3497bcc626aca216144589bf3f9715 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 23 Aug 2022 23:26:34 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Tue, 23 Aug 2022 23:26:34 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 23 Aug 2022 23:26:36 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1558244d39947a6f608f757be932356607a9f2be6c4d6ab7def29e54512d70d0 NON_IBM_SHA=c5edb6e93c6ac1f3ee6b74780a7b265efaaaaed625efccdd6f8597b844469a50 NOTICES_SHA=8f92b2e9c7dff626fb7f4cc360e29be26e3497bcc626aca216144589bf3f9715 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 23 Aug 2022 23:26:47 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1558244d39947a6f608f757be932356607a9f2be6c4d6ab7def29e54512d70d0 NON_IBM_SHA=c5edb6e93c6ac1f3ee6b74780a7b265efaaaaed625efccdd6f8597b844469a50 NOTICES_SHA=8f92b2e9c7dff626fb7f4cc360e29be26e3497bcc626aca216144589bf3f9715 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 23 Aug 2022 23:26:47 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 23 Aug 2022 23:26:48 GMT
USER 1001
# Tue, 23 Aug 2022 23:26:48 GMT
EXPOSE 9080 9443
# Tue, 23 Aug 2022 23:26:49 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 23 Aug 2022 23:26:49 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 23 Aug 2022 23:28:13 GMT
ARG VERBOSE=false
# Tue, 23 Aug 2022 23:28:14 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 23 Aug 2022 23:42:48 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 23 Aug 2022 23:42:53 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 23 Aug 2022 23:43:37 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:bf47d2be67f1a301865e78e8f78cc69c55dcc389921b4ba187dc0d333cbfd63b`  
		Last Modified: Tue, 02 Aug 2022 01:33:30 GMT  
		Size: 33.3 MB (33295352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93d2375ba0032ebd673deba460fc14719ca1d2863b8d267e076565f71f6a0a6`  
		Last Modified: Wed, 03 Aug 2022 03:33:39 GMT  
		Size: 17.2 MB (17202740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca0161a7c7c5ed84e960b77242dd8114a300146f937a8594bf3a6c60d8083f8`  
		Last Modified: Tue, 23 Aug 2022 22:57:05 GMT  
		Size: 48.8 MB (48770332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c9799f461ae3ac3d4930f6cf121004eb0d61c9d832adc4237527e7f36c7e59`  
		Last Modified: Tue, 23 Aug 2022 22:56:54 GMT  
		Size: 3.4 MB (3400062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e91e3b8297d3713af3d766796fe7f1769b3715f858a1fc465198922cc64bccd`  
		Last Modified: Wed, 24 Aug 2022 01:04:47 GMT  
		Size: 14.2 MB (14202433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b476b891064c238432601e6520280d94a1673f9718909f3e0b974d6c0b794c`  
		Last Modified: Wed, 24 Aug 2022 01:04:43 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6fa1decbc95bf2c2df050bb2e9c28c1e6a196c2853c1c8a00e7fd21f21e11e`  
		Last Modified: Wed, 24 Aug 2022 01:04:43 GMT  
		Size: 9.8 KB (9755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a692da2258d805429dff06accecc329921e95de0171c5a53ecef91fd6d00f7`  
		Last Modified: Wed, 24 Aug 2022 01:04:43 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9d2a5338cf6b066ada792880ee65a5308eb67cca7136217fe555b117468515`  
		Last Modified: Wed, 24 Aug 2022 01:04:43 GMT  
		Size: 10.7 KB (10734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc5c3d44e362ff828c009efb01a13f72134683854214abe71178baefe9d0b3a`  
		Last Modified: Wed, 24 Aug 2022 01:04:43 GMT  
		Size: 2.5 MB (2519707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f85edd9512592bc184e79c519b6303de1deed6adf9864f86e4df7b055ab435`  
		Last Modified: Wed, 24 Aug 2022 01:05:35 GMT  
		Size: 285.3 MB (285268322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa121d2ca1521910f52155aac0dd52629f9fe0ed188e8fe6ce4eda0eb2100cce`  
		Last Modified: Wed, 24 Aug 2022 01:05:11 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c899bafbd676fa78c34a5b1c9c5aef212b4c6234deabc396bdcc6cef2196a21`  
		Last Modified: Wed, 24 Aug 2022 01:05:14 GMT  
		Size: 12.8 MB (12771632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:332ccfcb9d333ce392fc28aa6e7bb172e9bb269b9ad9891d60782e7b8debf997
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.2 MB (411224737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:351b2e89f3743e599c0df22b26902e6a43979c5db4986f1e4081b07090e666cb`
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
# Wed, 10 Aug 2022 21:44:03 GMT
ENV JAVA_VERSION=jdk-11.0.16+8_openj9-0.33.0
# Wed, 10 Aug 2022 21:45:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='49dc05a3e9f3f99c5f8fa466261aa3e33a753694c67cabfa7d3f682e5a2e3685';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16%2B8_openj9-0.33.0/ibm-semeru-open-jre_aarch64_linux_11.0.16_8_openj9-0.33.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='552da889577571881ac58eb06877ca2fdadc12397f433b553b319674ee10a02d';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16%2B8_openj9-0.33.0/ibm-semeru-open-jre_ppc64le_linux_11.0.16_8_openj9-0.33.0.tar.gz';          ;;        amd64|x86_64)          ESUM='ba09711193b8b8664478f3f949b5320232f65c1bdf61f32a885d84de73c02767';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16%2B8_openj9-0.33.0/ibm-semeru-open-jre_x64_linux_11.0.16_8_openj9-0.33.0.tar.gz';          ;;        s390x)          ESUM='edfccd071e4276c51884cd89522b3be21fd2e44612f98f7a7d3dceb0c339a391';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16%2B8_openj9-0.33.0/ibm-semeru-open-jre_s390x_linux_11.0.16_8_openj9-0.33.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 10 Aug 2022 21:45:21 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Aug 2022 21:45:21 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 10 Aug 2022 21:46:02 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 10 Aug 2022 22:53:56 GMT
ARG VERBOSE=false
# Wed, 10 Aug 2022 22:53:56 GMT
ARG OPENJ9_SCC=true
# Wed, 10 Aug 2022 22:53:56 GMT
ARG EN_SHA=1558244d39947a6f608f757be932356607a9f2be6c4d6ab7def29e54512d70d0
# Wed, 10 Aug 2022 22:53:56 GMT
ARG NON_IBM_SHA=c5edb6e93c6ac1f3ee6b74780a7b265efaaaaed625efccdd6f8597b844469a50
# Wed, 10 Aug 2022 22:53:56 GMT
ARG NOTICES_SHA=8f92b2e9c7dff626fb7f4cc360e29be26e3497bcc626aca216144589bf3f9715
# Wed, 10 Aug 2022 22:53:56 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.8 org.opencontainers.image.revision=cl220820220719-1056 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 10 Aug 2022 22:53:57 GMT
ENV LIBERTY_VERSION=22.0.0_08
# Wed, 10 Aug 2022 22:53:57 GMT
ARG LIBERTY_URL
# Wed, 10 Aug 2022 22:53:57 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 10 Aug 2022 22:54:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1558244d39947a6f608f757be932356607a9f2be6c4d6ab7def29e54512d70d0 NON_IBM_SHA=c5edb6e93c6ac1f3ee6b74780a7b265efaaaaed625efccdd6f8597b844469a50 NOTICES_SHA=8f92b2e9c7dff626fb7f4cc360e29be26e3497bcc626aca216144589bf3f9715 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 10 Aug 2022 22:54:09 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Aug 2022 22:54:09 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.8 BuildLabel=cl220820220719-1056
# Wed, 10 Aug 2022 22:54:09 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 10 Aug 2022 22:54:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1558244d39947a6f608f757be932356607a9f2be6c4d6ab7def29e54512d70d0 NON_IBM_SHA=c5edb6e93c6ac1f3ee6b74780a7b265efaaaaed625efccdd6f8597b844469a50 NOTICES_SHA=8f92b2e9c7dff626fb7f4cc360e29be26e3497bcc626aca216144589bf3f9715 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 10 Aug 2022 22:54:10 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 10 Aug 2022 22:54:11 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 10 Aug 2022 22:54:11 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1558244d39947a6f608f757be932356607a9f2be6c4d6ab7def29e54512d70d0 NON_IBM_SHA=c5edb6e93c6ac1f3ee6b74780a7b265efaaaaed625efccdd6f8597b844469a50 NOTICES_SHA=8f92b2e9c7dff626fb7f4cc360e29be26e3497bcc626aca216144589bf3f9715 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 10 Aug 2022 22:54:17 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1558244d39947a6f608f757be932356607a9f2be6c4d6ab7def29e54512d70d0 NON_IBM_SHA=c5edb6e93c6ac1f3ee6b74780a7b265efaaaaed625efccdd6f8597b844469a50 NOTICES_SHA=8f92b2e9c7dff626fb7f4cc360e29be26e3497bcc626aca216144589bf3f9715 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 10 Aug 2022 22:54:18 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 10 Aug 2022 22:54:18 GMT
USER 1001
# Wed, 10 Aug 2022 22:54:18 GMT
EXPOSE 9080 9443
# Wed, 10 Aug 2022 22:54:18 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 10 Aug 2022 22:54:18 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 10 Aug 2022 22:54:58 GMT
ARG VERBOSE=false
# Wed, 10 Aug 2022 22:54:58 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 10 Aug 2022 23:01:38 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 10 Aug 2022 23:01:50 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 10 Aug 2022 23:02:19 GMT
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
	-	`sha256:8789b0a8047984a2b7ccee4b3a6081deb0fe29bda6be096c6f02bea19fc78ba6`  
		Last Modified: Wed, 10 Aug 2022 21:57:01 GMT  
		Size: 47.6 MB (47591346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c373e87136408d5c44592bc0724a77c4a077d72029332252bbfc32bfee89ea4d`  
		Last Modified: Wed, 10 Aug 2022 21:56:55 GMT  
		Size: 4.3 MB (4347894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7842295bad3d1e1c5f84789db763c43fb2b867873a67d219ecdc1984ed3799a0`  
		Last Modified: Wed, 10 Aug 2022 23:42:30 GMT  
		Size: 14.2 MB (14202026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8137f5004cda7e007580f7c2a9499c05fd289bb53380a395dea978b519f59e4`  
		Last Modified: Wed, 10 Aug 2022 23:42:28 GMT  
		Size: 669.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228c913b0aa276b9e7449839ec772fb09a0d4f18a11f4e5025a5e42f82cc4ff2`  
		Last Modified: Wed, 10 Aug 2022 23:42:27 GMT  
		Size: 9.8 KB (9753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0c3fc62cb6b1b22992f24a16fe11c5621e836303d8fbc5404a65b9233cb84c`  
		Last Modified: Wed, 10 Aug 2022 23:42:27 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742505e7686477e000188c3efbf61d9a6f5c8890e8df00ffb6900397a5488de8`  
		Last Modified: Wed, 10 Aug 2022 23:42:27 GMT  
		Size: 10.7 KB (10729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff3d9955419aa83c434d24cb7b263488e0189e7d2f502aa321df990fc281469`  
		Last Modified: Wed, 10 Aug 2022 23:42:28 GMT  
		Size: 2.6 MB (2575303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197f22aa9f72593912ce43398435580e2f790f0a4099988aa0ff8c6e75e0cf50`  
		Last Modified: Wed, 10 Aug 2022 23:42:54 GMT  
		Size: 285.3 MB (285267428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5d09721f13b581307c2b3911c280ad3ef41ab5596977f33b5b2feff23de3a3`  
		Last Modified: Wed, 10 Aug 2022 23:42:42 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3aacf928ddfad20da88647496fe124e9e8b6d838149c3c130d29695189cd914`  
		Last Modified: Wed, 10 Aug 2022 23:42:43 GMT  
		Size: 14.4 MB (14442883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
