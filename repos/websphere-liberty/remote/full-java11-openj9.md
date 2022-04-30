## `websphere-liberty:full-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:23e342a549bacccb0cee6187b46aff5ef27400f96ae14624c9cfd8630c67b88b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:23933a607eac58db2ca0b984e071eb1f0119e1c42eeb79a1a7cb566081c10caa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.2 MB (393154003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:943d9b10968d0dd3e5bef95b2be4588443ebdca847f78924b5cb5d9bad1232f0`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:04:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 02:04:35 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Apr 2022 19:58:21 GMT
ENV JAVA_VERSION=jdk-11.0.15+10_openj9-0.32.0
# Wed, 27 Apr 2022 20:00:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69e4a0b383c7b4187478ddb196de3cdc91560e2be40b8ef66354591e87c36e85';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5e82f7df54786c557d2d9e9ac22df655fd94b9702c73261390903ac87532d545';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='25d4d5e2bbe3eb19bcb9a76aec4b43d4eef5ad66200df3122118f69da5325cf6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='def85f1b00e9c65a8c3b5dcf4da0f1b04c17675b4ff9cd6f5dad61d8dcbd03d0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 27 Apr 2022 20:00:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Apr 2022 20:00:34 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 27 Apr 2022 20:01:09 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 27 Apr 2022 20:52:17 GMT
ARG VERBOSE=false
# Wed, 27 Apr 2022 20:52:17 GMT
ARG OPENJ9_SCC=true
# Wed, 27 Apr 2022 20:52:17 GMT
ARG EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851
# Wed, 27 Apr 2022 20:52:17 GMT
ARG NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e
# Wed, 27 Apr 2022 20:52:17 GMT
ARG NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024
# Wed, 27 Apr 2022 20:52:17 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.4 org.opencontainers.image.revision=cl220420220328-1303 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 27 Apr 2022 20:52:17 GMT
ENV LIBERTY_VERSION=22.0.0_04
# Wed, 27 Apr 2022 20:52:18 GMT
ARG LIBERTY_URL
# Wed, 27 Apr 2022 20:52:18 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 27 Apr 2022 20:52:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Apr 2022 20:52:27 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Apr 2022 20:52:27 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.4 BuildLabel=cl220420220328-1303
# Wed, 27 Apr 2022 20:52:28 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 27 Apr 2022 20:52:28 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 27 Apr 2022 20:52:28 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 27 Apr 2022 20:52:29 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 27 Apr 2022 20:52:29 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 27 Apr 2022 20:52:36 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 27 Apr 2022 20:52:36 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 27 Apr 2022 20:52:36 GMT
USER 1001
# Wed, 27 Apr 2022 20:52:36 GMT
EXPOSE 9080 9443
# Wed, 27 Apr 2022 20:52:36 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 27 Apr 2022 20:52:36 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 27 Apr 2022 20:53:05 GMT
ARG VERBOSE=false
# Wed, 27 Apr 2022 20:53:05 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 27 Apr 2022 20:56:57 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 27 Apr 2022 20:56:58 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 27 Apr 2022 20:57:26 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b11e2aa9202b3c11a943dfa8adc2bef4462ab2165124b84051d10250faff2a0`  
		Last Modified: Fri, 22 Apr 2022 02:08:16 GMT  
		Size: 16.0 MB (16030117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87482ef314cf646e00e5071614a046f7dbe4ab38c82be31b1764118c5b10d7ce`  
		Last Modified: Wed, 27 Apr 2022 20:12:10 GMT  
		Size: 47.7 MB (47691446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa220c0f41c9a8d027e61a2ce230738f17ce92cfe6eb36c5ced117295a33c84`  
		Last Modified: Wed, 27 Apr 2022 20:12:04 GMT  
		Size: 4.2 MB (4214317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eef0f9ff1913008cfb9a48dfb8af2d05d4337c531abbc3140020427f7560729`  
		Last Modified: Wed, 27 Apr 2022 21:22:29 GMT  
		Size: 14.3 MB (14295363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e3c63220be1502e13b9ff03ede3f2eb3b54a70ef0e8d24d838e080f05d03ed`  
		Last Modified: Wed, 27 Apr 2022 21:22:26 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872169d3c19067bc9a1b0060e64ebecb4d33ec08a5ae4fbd86ff72822a6ec731`  
		Last Modified: Wed, 27 Apr 2022 21:22:25 GMT  
		Size: 9.7 KB (9673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048bf67080ee77bbdae6c617033bec4f48188c8c7604254b8acf5ec5fd864a96`  
		Last Modified: Wed, 27 Apr 2022 21:22:25 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aece9e52e1c3f5712efb7ef0df013cd79b0c30babb09f1aa272ddf134dd36e19`  
		Last Modified: Wed, 27 Apr 2022 21:22:25 GMT  
		Size: 10.7 KB (10660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72199f8a6ff9b557f1bab7a86b3f6cb4639935f61593fa2273eebc30c7b9b58`  
		Last Modified: Wed, 27 Apr 2022 21:22:26 GMT  
		Size: 2.5 MB (2522896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3efcf8f2d260f95a9f3d01392d651eeb32e718e219c570b5eb9a40869fa321`  
		Last Modified: Wed, 27 Apr 2022 21:23:02 GMT  
		Size: 265.2 MB (265214498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc825b576f6b2d058d63aa25571cd3eeea0ebd4e7bbe13ee861742bb82746350`  
		Last Modified: Wed, 27 Apr 2022 21:22:48 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e950d2ead4274404f98ea9cc2cfe1d2d60ae42638832f8eb9043b58ec6221b1`  
		Last Modified: Wed, 27 Apr 2022 21:22:51 GMT  
		Size: 14.6 MB (14597128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:ace4968e2c0220e326643376003e14657b74660f112bbb5904fecc794f691a77
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.9 MB (396912573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d79ecbe4f8d5a18093f40c2d8e396139a28c5b774b571af791d96d06f54a340`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 09:45:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 09:46:56 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Apr 2022 22:22:31 GMT
ENV JAVA_VERSION=jdk-11.0.15+10_openj9-0.32.0
# Wed, 27 Apr 2022 22:26:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69e4a0b383c7b4187478ddb196de3cdc91560e2be40b8ef66354591e87c36e85';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5e82f7df54786c557d2d9e9ac22df655fd94b9702c73261390903ac87532d545';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='25d4d5e2bbe3eb19bcb9a76aec4b43d4eef5ad66200df3122118f69da5325cf6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='def85f1b00e9c65a8c3b5dcf4da0f1b04c17675b4ff9cd6f5dad61d8dcbd03d0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 27 Apr 2022 22:26:04 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Apr 2022 22:26:06 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 27 Apr 2022 22:26:45 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 28 Apr 2022 02:55:36 GMT
ARG VERBOSE=false
# Thu, 28 Apr 2022 02:55:40 GMT
ARG OPENJ9_SCC=true
# Thu, 28 Apr 2022 02:55:42 GMT
ARG EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851
# Thu, 28 Apr 2022 02:55:43 GMT
ARG NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e
# Thu, 28 Apr 2022 02:55:45 GMT
ARG NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024
# Thu, 28 Apr 2022 02:55:47 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.4 org.opencontainers.image.revision=cl220420220328-1303 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 28 Apr 2022 02:55:50 GMT
ENV LIBERTY_VERSION=22.0.0_04
# Thu, 28 Apr 2022 02:55:51 GMT
ARG LIBERTY_URL
# Thu, 28 Apr 2022 02:56:12 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 28 Apr 2022 02:57:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 28 Apr 2022 02:57:48 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Apr 2022 02:57:49 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.4 BuildLabel=cl220420220328-1303
# Thu, 28 Apr 2022 02:57:51 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 28 Apr 2022 02:57:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 28 Apr 2022 02:57:57 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Thu, 28 Apr 2022 02:57:58 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 28 Apr 2022 02:58:05 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 28 Apr 2022 02:58:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 28 Apr 2022 02:58:23 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 28 Apr 2022 02:58:24 GMT
USER 1001
# Thu, 28 Apr 2022 02:58:25 GMT
EXPOSE 9080 9443
# Thu, 28 Apr 2022 02:58:26 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 28 Apr 2022 02:58:28 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 28 Apr 2022 03:01:32 GMT
ARG VERBOSE=false
# Thu, 28 Apr 2022 03:01:35 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 28 Apr 2022 03:06:22 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Thu, 28 Apr 2022 03:06:33 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 28 Apr 2022 03:07:23 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc56b8d6fd0bb34b3c200e96dec3af60f79a6f302365ccc050f056b1d5993a3`  
		Last Modified: Fri, 22 Apr 2022 09:58:22 GMT  
		Size: 17.2 MB (17204271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcaa6e7c86b37af0530f56a1e0150a9af29558f3cab36cf281cc996d4e58941c`  
		Last Modified: Wed, 27 Apr 2022 22:44:14 GMT  
		Size: 48.4 MB (48378492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739d132964ddfe7009ec856ed073ab49a9c911ade9c70f71ce0b9fb83f1250aa`  
		Last Modified: Wed, 27 Apr 2022 22:44:06 GMT  
		Size: 3.3 MB (3343032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c573357d3b657ee044995a6f53cc35877ab885392b49ab56d9139a533760eb3`  
		Last Modified: Thu, 28 Apr 2022 03:46:34 GMT  
		Size: 14.3 MB (14295908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfcda1fc3ed9b1a022a952ff1036785988a55e9be601c88409970e8c9260cf1`  
		Last Modified: Thu, 28 Apr 2022 03:46:29 GMT  
		Size: 690.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3977861b1d2c72d2787503c84082d244254a3552984aa30f50e6eae49b2405e4`  
		Last Modified: Thu, 28 Apr 2022 03:46:29 GMT  
		Size: 9.7 KB (9675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23d746b959f8dcf094c3f5738611cef7ccfa6410bd2de56fbdb3581f2f301e6`  
		Last Modified: Thu, 28 Apr 2022 03:46:29 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab8e846cbb390b462ea00cc8b9070e73a877d74175b9b8c9d288ca0c455a272`  
		Last Modified: Thu, 28 Apr 2022 03:46:29 GMT  
		Size: 10.7 KB (10672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133e5ee0dd8c02fb8820bc389e0c4c1011af445eeffceaa09a63cc94d7c695d0`  
		Last Modified: Thu, 28 Apr 2022 03:46:30 GMT  
		Size: 2.5 MB (2511900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf270ec15f2d57da12b61765169ea14c524b16dc7ae5bd37024ce208aa284d0`  
		Last Modified: Thu, 28 Apr 2022 03:47:20 GMT  
		Size: 265.2 MB (265215172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac6d380c122f0cc63ec6089145f8b0a4431c60da8178e68d4418420bc12947f`  
		Last Modified: Thu, 28 Apr 2022 03:46:57 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2210c92255e610bd22b337d1af793bcbc98b149ca6fc9c980ffdc89fa197cbd8`  
		Last Modified: Thu, 28 Apr 2022 03:46:59 GMT  
		Size: 12.7 MB (12651169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:11142685070c07aa20c6c56e677a62e2b86d6aa19762175bd46edbcdb4444733
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.4 MB (390379746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9b6b9b46ae7da36e6422dead80b66e831bc1557ed20c9794707a8a4f5d158fc`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:22:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 29 Apr 2022 23:22:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:32:55 GMT
ENV JAVA_VERSION=jdk-11.0.15+10_openj9-0.32.0
# Fri, 29 Apr 2022 23:33:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69e4a0b383c7b4187478ddb196de3cdc91560e2be40b8ef66354591e87c36e85';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5e82f7df54786c557d2d9e9ac22df655fd94b9702c73261390903ac87532d545';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='25d4d5e2bbe3eb19bcb9a76aec4b43d4eef5ad66200df3122118f69da5325cf6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='def85f1b00e9c65a8c3b5dcf4da0f1b04c17675b4ff9cd6f5dad61d8dcbd03d0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 29 Apr 2022 23:33:58 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Apr 2022 23:33:59 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Fri, 29 Apr 2022 23:34:31 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Sat, 30 Apr 2022 01:15:25 GMT
ARG VERBOSE=false
# Sat, 30 Apr 2022 01:15:25 GMT
ARG OPENJ9_SCC=true
# Sat, 30 Apr 2022 01:15:26 GMT
ARG EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851
# Sat, 30 Apr 2022 01:15:26 GMT
ARG NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e
# Sat, 30 Apr 2022 01:15:26 GMT
ARG NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024
# Sat, 30 Apr 2022 01:15:26 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.4 org.opencontainers.image.revision=cl220420220328-1303 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Sat, 30 Apr 2022 01:15:27 GMT
ENV LIBERTY_VERSION=22.0.0_04
# Sat, 30 Apr 2022 01:15:27 GMT
ARG LIBERTY_URL
# Sat, 30 Apr 2022 01:15:27 GMT
ARG DOWNLOAD_OPTIONS=
# Sat, 30 Apr 2022 01:15:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:15:39 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 30 Apr 2022 01:15:40 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.4 BuildLabel=cl220420220328-1303
# Sat, 30 Apr 2022 01:15:40 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Sat, 30 Apr 2022 01:15:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 30 Apr 2022 01:15:41 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Sat, 30 Apr 2022 01:15:41 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Sat, 30 Apr 2022 01:15:42 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Sat, 30 Apr 2022 01:15:49 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Sat, 30 Apr 2022 01:15:49 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Sat, 30 Apr 2022 01:15:49 GMT
USER 1001
# Sat, 30 Apr 2022 01:15:49 GMT
EXPOSE 9080 9443
# Sat, 30 Apr 2022 01:15:50 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Sat, 30 Apr 2022 01:15:50 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Sat, 30 Apr 2022 01:21:45 GMT
ARG VERBOSE=false
# Sat, 30 Apr 2022 01:21:45 GMT
ARG REPOSITORIES_PROPERTIES=
# Sat, 30 Apr 2022 01:26:07 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Sat, 30 Apr 2022 01:26:20 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Sat, 30 Apr 2022 01:26:44 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1002590b38d45b986e07362b8635ab8cb57c796f0a8ae1a3c707970fe0200e54`  
		Last Modified: Fri, 29 Apr 2022 23:25:27 GMT  
		Size: 15.7 MB (15739301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8db8f55d6f000d8c25bc0d84644806d48ffa2ffe1a9f1b5445be9339237017`  
		Last Modified: Fri, 29 Apr 2022 23:42:12 GMT  
		Size: 46.7 MB (46721690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea77f2031d57aa0c948bdcddb61f7d6ed06146fc9413cdeeb9de79ee7fd1c0f5`  
		Last Modified: Fri, 29 Apr 2022 23:42:07 GMT  
		Size: 4.3 MB (4328081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d97a12f5c45c316a472a4eba02c0913a39c3cc5edfedd481d99825834eb7e3`  
		Last Modified: Sat, 30 Apr 2022 02:07:20 GMT  
		Size: 14.3 MB (14295557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169895b794ddbec98d2f110cfbc3f128403ca4956135900864dc9f0638d59c91`  
		Last Modified: Sat, 30 Apr 2022 02:07:18 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bcde2eee6bda1671664ee05f14025527cbcd124ef4332b8b6aaafef6ba7894`  
		Last Modified: Sat, 30 Apr 2022 02:07:18 GMT  
		Size: 9.7 KB (9674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d122245321644e0d44be3c85b12c864273ba99aeaa247725086494f9d6a675`  
		Last Modified: Sat, 30 Apr 2022 02:07:18 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3801ba261ba0c0bc0ae449986ff88e09c8eb102eec0bae1026c6ec72e0cdf5`  
		Last Modified: Sat, 30 Apr 2022 02:07:18 GMT  
		Size: 10.7 KB (10652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bae98d4cd39a3eaf5555dcf10c36de2d2ead9a38ac734d29ae71c0db438e4`  
		Last Modified: Sat, 30 Apr 2022 02:07:19 GMT  
		Size: 2.5 MB (2537158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc072c7e2c05218ba1ac045ac643821c2b7b5dd9126b0caf43c37333b3bb1bc`  
		Last Modified: Sat, 30 Apr 2022 02:08:01 GMT  
		Size: 265.2 MB (265215287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3aee8b0bf0605f5fb9ba1d2bcca052f18cbb79bc03aca506a43012503a2866`  
		Last Modified: Sat, 30 Apr 2022 02:07:50 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4900ee19e761c849bff9b7af0964e3aa49770b666ed0d0295d6ae4cd96b05794`  
		Last Modified: Sat, 30 Apr 2022 02:07:52 GMT  
		Size: 14.5 MB (14455021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
