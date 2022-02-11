## `websphere-liberty:full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:e22bd59d95bcff00a765484ff3561d709957d0a0daf771d41ad4bf1c10fbf29f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:22ab2e4bb7ea4801f61ffa1dfa0712bd56b61cc8eb7d2697a959757fc0c4544f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.9 MB (398906406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f565ecf234b796a7e05d7e2fb1c9f28b0cc28f2d6104acb5433b7bd8c93ab31`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:57:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 07:42:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Feb 2022 19:22:44 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Fri, 11 Feb 2022 19:24:36 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 11 Feb 2022 19:24:36 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Feb 2022 19:24:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Fri, 11 Feb 2022 19:25:12 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Fri, 11 Feb 2022 20:29:12 GMT
ARG VERBOSE=false
# Fri, 11 Feb 2022 20:29:12 GMT
ARG OPENJ9_SCC=true
# Fri, 11 Feb 2022 20:29:12 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Fri, 11 Feb 2022 20:29:12 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Fri, 11 Feb 2022 20:29:13 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Fri, 11 Feb 2022 20:29:13 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 11 Feb 2022 20:29:13 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Fri, 11 Feb 2022 20:29:13 GMT
ARG LIBERTY_URL
# Fri, 11 Feb 2022 20:29:13 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 11 Feb 2022 20:29:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Feb 2022 20:29:24 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Feb 2022 20:29:24 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Fri, 11 Feb 2022 20:29:24 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 11 Feb 2022 20:29:25 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 11 Feb 2022 20:29:25 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Fri, 11 Feb 2022 20:29:26 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 11 Feb 2022 20:29:26 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 11 Feb 2022 20:29:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 11 Feb 2022 20:29:35 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Fri, 11 Feb 2022 20:29:35 GMT
USER 1001
# Fri, 11 Feb 2022 20:29:35 GMT
EXPOSE 9080 9443
# Fri, 11 Feb 2022 20:29:35 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 11 Feb 2022 20:29:35 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 11 Feb 2022 20:29:43 GMT
ARG VERBOSE=false
# Fri, 11 Feb 2022 20:29:44 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 11 Feb 2022 20:33:17 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Fri, 11 Feb 2022 20:33:19 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 11 Feb 2022 20:33:55 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a290702f639f2b2f25c1f64f9446f34bd91f353be52bb6c67b3575d304932c8d`  
		Last Modified: Wed, 02 Feb 2022 07:50:26 GMT  
		Size: 16.0 MB (16032322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbf5de6623326de34a7d2963e4ea9b5ea718e5720d7d201ebffb5695e25f06c`  
		Last Modified: Fri, 11 Feb 2022 19:28:09 GMT  
		Size: 47.7 MB (47658309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f6f1ed16cfa548caa1ac1132c8669b1349e2423bb126867e997822e8204bd8`  
		Last Modified: Fri, 11 Feb 2022 19:28:05 GMT  
		Size: 4.2 MB (4181401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d984f1dd333a22da161dc0ddbcf8dbe058e54ef973f30db7ceb12c5bb6dd0ca`  
		Last Modified: Fri, 11 Feb 2022 20:44:01 GMT  
		Size: 14.2 MB (14228754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0805c31e70d0f439ade4d0286bcee9fe78fe43a7ada73e3a875a8844a6da803`  
		Last Modified: Fri, 11 Feb 2022 20:43:57 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271e050833e94f710ec20eae9977ce1e6d2d8b74c4c76662f56719b40c16b254`  
		Last Modified: Fri, 11 Feb 2022 20:43:56 GMT  
		Size: 9.7 KB (9672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34691762aeab8921fcd0fbfed2da386938fa583929962e53ed66af01fb23954`  
		Last Modified: Fri, 11 Feb 2022 20:43:57 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a657fc58e999548467d273c7edbc2cbbdfd4d6c1cee515ddca52c99ed4904125`  
		Last Modified: Fri, 11 Feb 2022 20:43:57 GMT  
		Size: 10.6 KB (10646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fb55f2d1be034a597f1ce9ecd5f3350e9927dec764110548ecff0983565bfa`  
		Last Modified: Fri, 11 Feb 2022 20:43:57 GMT  
		Size: 2.5 MB (2509939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1596088aa7aae3ce578d1a2b53e5c5c060f8c78eea6cc265043b6452147060f`  
		Last Modified: Fri, 11 Feb 2022 20:44:28 GMT  
		Size: 271.1 MB (271128353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59cedff7e40f13d2209817bdac83f54d77db1338162ff67646487df90e3a9f72`  
		Last Modified: Fri, 11 Feb 2022 20:44:14 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ff297d893ede976b947791875305d38a77ad0f1281c013dd71761db628d426`  
		Last Modified: Fri, 11 Feb 2022 20:44:16 GMT  
		Size: 14.6 MB (14581007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:6ba1eb73e7adcd3bfb83469aab0b305a23206442cd519bbd722ce048615b6335
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.6 MB (402571013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f3e61a98f95ac70310982bcf7e71fa35fe5876cb1824848e4c6ab13075888ac`
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
# Fri, 11 Feb 2022 19:24:06 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Fri, 11 Feb 2022 19:27:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 11 Feb 2022 19:27:43 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Feb 2022 19:27:47 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Fri, 11 Feb 2022 19:28:31 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Fri, 11 Feb 2022 20:27:24 GMT
ARG VERBOSE=false
# Fri, 11 Feb 2022 20:27:27 GMT
ARG OPENJ9_SCC=true
# Fri, 11 Feb 2022 20:27:29 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Fri, 11 Feb 2022 20:27:31 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Fri, 11 Feb 2022 20:27:33 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Fri, 11 Feb 2022 20:27:34 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 11 Feb 2022 20:27:36 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Fri, 11 Feb 2022 20:27:40 GMT
ARG LIBERTY_URL
# Fri, 11 Feb 2022 20:27:43 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 11 Feb 2022 20:28:14 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Feb 2022 20:28:16 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Feb 2022 20:28:18 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Fri, 11 Feb 2022 20:28:19 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 11 Feb 2022 20:28:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 11 Feb 2022 20:28:24 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Fri, 11 Feb 2022 20:28:25 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 11 Feb 2022 20:28:30 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 11 Feb 2022 20:28:43 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 11 Feb 2022 20:28:46 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Fri, 11 Feb 2022 20:28:47 GMT
USER 1001
# Fri, 11 Feb 2022 20:28:49 GMT
EXPOSE 9080 9443
# Fri, 11 Feb 2022 20:28:51 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 11 Feb 2022 20:28:53 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 11 Feb 2022 20:29:11 GMT
ARG VERBOSE=false
# Fri, 11 Feb 2022 20:29:13 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 11 Feb 2022 20:33:32 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Fri, 11 Feb 2022 20:33:39 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 11 Feb 2022 20:34:31 GMT
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
	-	`sha256:fe4bd076876faf2f0233df3e5062e9079ea0e65d66b1a00b6546775ccf35a16f`  
		Last Modified: Fri, 11 Feb 2022 19:33:28 GMT  
		Size: 48.4 MB (48356013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8862a35e96ccf63d16c503c7d9874834dce679147273f8634d02e4cc45804df5`  
		Last Modified: Fri, 11 Feb 2022 19:33:20 GMT  
		Size: 3.3 MB (3340086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38062b7cef9e9c2dc36c9e99e44feb1c879bcfb683b952dba62daee713b5c749`  
		Last Modified: Fri, 11 Feb 2022 20:53:27 GMT  
		Size: 14.2 MB (14229426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d473ac4a5659ffe2edde9534b92f9000707caa66169729aa337894229f34f1`  
		Last Modified: Fri, 11 Feb 2022 20:53:23 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6401cdf7f6987375189f6309e3d6d44736dabb5b8e7927812b9dcc85842e604`  
		Last Modified: Fri, 11 Feb 2022 20:53:23 GMT  
		Size: 9.7 KB (9667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd617d4033b2f6ff52854c01fd11d7e14f43bec4907710e98a39f66394802fb1`  
		Last Modified: Fri, 11 Feb 2022 20:53:23 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8ceec147b4be950dc4118348e7a2bdd7d7bb538fd45a4ea5f816e8012bbbf0`  
		Last Modified: Fri, 11 Feb 2022 20:53:23 GMT  
		Size: 10.7 KB (10667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b188c4bd1cb50f30e4283491b96b9e8ca028b286af170f4e3931684dd0a63e3c`  
		Last Modified: Fri, 11 Feb 2022 20:53:24 GMT  
		Size: 2.5 MB (2476993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646e40f0fafaf90f0a465af3467230b29d503364a85572ff5c363e4efa59ccaf`  
		Last Modified: Fri, 11 Feb 2022 20:54:02 GMT  
		Size: 271.1 MB (271128611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e40bfaf270454734e68901516ce05c530f0cdb17c7ba7e363bb3b6b1a87ec1`  
		Last Modified: Fri, 11 Feb 2022 20:53:37 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f96fb558e1571478e3c1180321dcaa713011cd87239b081e363e87bb182eb0ae`  
		Last Modified: Fri, 11 Feb 2022 20:53:42 GMT  
		Size: 12.5 MB (12526044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:794f151c8cc3ab65962e9593c15df0c7d2a786ccadb630246baf4a8f0d84f32b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.1 MB (396122130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dda5071f1d77e8e2a381b3e65c453ea5d7670a20985d812dd7c463b0e6f6d184`
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
# Fri, 11 Feb 2022 18:45:14 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Fri, 11 Feb 2022 18:46:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 11 Feb 2022 18:46:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Feb 2022 18:46:18 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Fri, 11 Feb 2022 18:46:51 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Fri, 11 Feb 2022 19:05:03 GMT
ARG VERBOSE=false
# Fri, 11 Feb 2022 19:05:03 GMT
ARG OPENJ9_SCC=true
# Fri, 11 Feb 2022 19:05:03 GMT
ARG EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a
# Fri, 11 Feb 2022 19:05:04 GMT
ARG NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c
# Fri, 11 Feb 2022 19:05:04 GMT
ARG NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1
# Fri, 11 Feb 2022 19:05:04 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.1 org.opencontainers.image.revision=cl22.0.0.1920-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 11 Feb 2022 19:05:04 GMT
ENV LIBERTY_VERSION=22.0.0_01
# Fri, 11 Feb 2022 19:05:04 GMT
ARG LIBERTY_URL
# Fri, 11 Feb 2022 19:05:04 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 11 Feb 2022 19:05:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Feb 2022 19:05:17 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Feb 2022 19:05:17 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.1 BuildLabel=cl22.0.0.1920-1900
# Fri, 11 Feb 2022 19:05:17 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 11 Feb 2022 19:05:18 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 11 Feb 2022 19:05:18 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Fri, 11 Feb 2022 19:05:18 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 11 Feb 2022 19:05:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 11 Feb 2022 19:05:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=4889b338a814eb953faba1135d105046ae7d7a62eaf75fb05804214b9fd8ef3a NON_IBM_SHA=8f56725d48ec762b9b270c3bf34fba5b67472f0e1d8d0326a6a25483d363bc9c NOTICES_SHA=73325d908f5c8d24cba975c429c58bf7f631a947ddc206b1081f2c347e30bff1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 11 Feb 2022 19:05:25 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Fri, 11 Feb 2022 19:05:25 GMT
USER 1001
# Fri, 11 Feb 2022 19:05:25 GMT
EXPOSE 9080 9443
# Fri, 11 Feb 2022 19:05:25 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 11 Feb 2022 19:05:26 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 11 Feb 2022 19:05:42 GMT
ARG VERBOSE=false
# Fri, 11 Feb 2022 19:05:42 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 11 Feb 2022 19:10:17 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Fri, 11 Feb 2022 19:10:23 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 11 Feb 2022 19:10:46 GMT
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
	-	`sha256:5515d4a1951c343a0f0bedb92914c34084e82badac27c7f486bdb3ddcefb23ed`  
		Last Modified: Fri, 11 Feb 2022 18:49:10 GMT  
		Size: 46.7 MB (46692267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645951b5910b324b3c7d389bece0964171b59685768b753c86f7a7aaa4e254b7`  
		Last Modified: Fri, 11 Feb 2022 18:49:04 GMT  
		Size: 4.3 MB (4294909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd10a01e01aee4c91f02cfe3257a489b10144ba1784af3b53066cfbe84922b37`  
		Last Modified: Fri, 11 Feb 2022 19:23:05 GMT  
		Size: 14.2 MB (14228969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7d6748cec265f5158aba47b8a8473c5ceae932b1558b29523fbde9d3535436`  
		Last Modified: Fri, 11 Feb 2022 19:23:02 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d57dee6aae9b26451957752a42df571804311b03aacbf4af06ccb75dc09009f`  
		Last Modified: Fri, 11 Feb 2022 19:23:02 GMT  
		Size: 9.7 KB (9669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89c70bc19d05306898001104fd91c9d7bc9afdb3047e25f8e319084268c055a`  
		Last Modified: Fri, 11 Feb 2022 19:23:02 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5704fcb0abc115bc119f007278b6514ecab80925a2e0cc4b12d6735d95433453`  
		Last Modified: Fri, 11 Feb 2022 19:23:02 GMT  
		Size: 10.6 KB (10643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff437d75bb345dada616d167de3319bc8a876a30702d1740260c747f6fa7b10`  
		Last Modified: Fri, 11 Feb 2022 19:23:03 GMT  
		Size: 2.5 MB (2505834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a358ae305c1b3317b398c6ed3a72e26d0d61baef313c304779f4a92f42484f8c`  
		Last Modified: Fri, 11 Feb 2022 19:23:24 GMT  
		Size: 271.1 MB (271128695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d0c185d8a34a3919e5f564a06f40bb23d91d4a4160f8ccc6955ff670ef27e5`  
		Last Modified: Fri, 11 Feb 2022 19:23:13 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af0aa3e229146752d8fd7346f70ef77cc61c4f6014dd62870b396b7bf82b6a6`  
		Last Modified: Fri, 11 Feb 2022 19:23:15 GMT  
		Size: 14.4 MB (14390831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
