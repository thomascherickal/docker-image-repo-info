## `open-liberty:beta-java11`

```console
$ docker pull open-liberty@sha256:a3ce303ac0d60ab2d83b3fa460687adf8cedb7bf081f10bed289b0b7819ce316
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:beta-java11` - linux; amd64

```console
$ docker pull open-liberty@sha256:6211a0f27625dfa5c131a1b765347121834fb8832e2ceb3615cbe4deb9bac582
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.9 MB (404850450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b8ade9649879d29dcea548d8d4d68460a6ded90af1e77c4c96f1a209fa82e1d`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 03 Mar 2022 20:19:33 GMT
ADD file:8a50ad78a668527e974b05a3dfbfd64760de3cb643ceb8a8805d21f6ceab3389 in / 
# Thu, 03 Mar 2022 20:19:33 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 21:23:35 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 03 Mar 2022 23:58:55 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 00:00:36 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Fri, 04 Mar 2022 00:01:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 04 Mar 2022 00:01:40 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 03:45:47 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 17 Mar 2022 03:46:28 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Sat, 19 Mar 2022 17:52:53 GMT
ARG LIBERTY_VERSION=22.0.0.4-beta
# Sat, 19 Mar 2022 17:52:53 GMT
ARG LIBERTY_SHA=a8cbd6e6b91184eda126235f31e63c198ba821dc
# Sat, 19 Mar 2022 17:52:53 GMT
ARG LIBERTY_BUILD_LABEL=cl220320220302-1100
# Sat, 19 Mar 2022 17:52:53 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.4-beta/openliberty-runtime-22.0.0.4-beta.zip
# Sat, 19 Mar 2022 17:52:53 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Sat, 19 Mar 2022 17:52:54 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Sat, 19 Mar 2022 17:52:54 GMT
ARG OPENJ9_SCC=true
# Sat, 19 Mar 2022 17:52:54 GMT
ARG VERBOSE=false
# Sat, 19 Mar 2022 17:52:54 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with IBM Semeru Runtime Open Edition OpenJDK 11 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=22.0.0.4-beta
# Sat, 19 Mar 2022 17:52:54 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Sat, 19 Mar 2022 17:52:54 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sat, 19 Mar 2022 17:53:11 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.4-beta/openliberty-runtime-22.0.0.4-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=a8cbd6e6b91184eda126235f31e63c198ba821dc LIBERTY_VERSION=22.0.0.4-beta OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sat, 19 Mar 2022 17:53:12 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sat, 19 Mar 2022 17:53:13 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.4-beta/openliberty-runtime-22.0.0.4-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=a8cbd6e6b91184eda126235f31e63c198ba821dc LIBERTY_VERSION=22.0.0.4-beta VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 19 Mar 2022 17:53:13 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.4-beta/openliberty-runtime-22.0.0.4-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=a8cbd6e6b91184eda126235f31e63c198ba821dc LIBERTY_VERSION=22.0.0.4-beta VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sat, 19 Mar 2022 17:53:52 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.4-beta/openliberty-runtime-22.0.0.4-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=a8cbd6e6b91184eda126235f31e63c198ba821dc LIBERTY_VERSION=22.0.0.4-beta VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sat, 19 Mar 2022 17:53:52 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Sat, 19 Mar 2022 17:53:52 GMT
USER 1001
# Sat, 19 Mar 2022 17:53:52 GMT
EXPOSE 9080 9443
# Sat, 19 Mar 2022 17:53:52 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sat, 19 Mar 2022 17:53:52 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:7c3b88808835aa80f1ef7f03083c5ae781d0f44e644537cd72de4ce6c5e62e00`  
		Last Modified: Thu, 03 Mar 2022 20:20:44 GMT  
		Size: 28.6 MB (28565751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d66994d054da0091fad11fb497b2a23c0cfd350d897d78d57f78b3200b90fd6`  
		Last Modified: Fri, 04 Mar 2022 00:06:51 GMT  
		Size: 16.0 MB (16030868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567b8f8eb8089aa72d03cfbac6276b00568320b44f8548f5c65bd83bd5fe2358`  
		Last Modified: Fri, 04 Mar 2022 00:07:59 GMT  
		Size: 47.7 MB (47658340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eacdf7e8adff97c2aaefd37ec49e55a864d76f4117411f6e121a8a144d4af6ba`  
		Last Modified: Thu, 17 Mar 2022 03:52:45 GMT  
		Size: 4.5 MB (4460215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c053ded084e4d6b538782597f6b8f3982f17e8180977d50b159201d692418faf`  
		Last Modified: Sat, 19 Mar 2022 18:00:42 GMT  
		Size: 8.6 KB (8552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5813366702b674d3dcad8072a38362a7c73b00267940b7d0245eda6973179ff5`  
		Last Modified: Sat, 19 Mar 2022 18:00:40 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d380783e330d0dd3ec5dc196f6c7dac87111ec9c74ff9c1a88679bf267bc12`  
		Last Modified: Sat, 19 Mar 2022 18:00:56 GMT  
		Size: 293.9 MB (293927412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4894812d38a92d38a96318868428e40a63c679774c26b48156e4e70caa8aec9a`  
		Last Modified: Sat, 19 Mar 2022 18:00:40 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f80437f8151838e3c81f552527f7a9faf32b609a0167f594ed98929cf44eeec`  
		Last Modified: Sat, 19 Mar 2022 18:00:40 GMT  
		Size: 10.0 KB (10048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbc20c8416ac79d0c23254ed77aa903b0e1317beb0a3f5f2361a63687fc3298`  
		Last Modified: Sat, 19 Mar 2022 18:00:42 GMT  
		Size: 14.2 MB (14187701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:beta-java11` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:4c04a45765791f9504213c8ebdbc243bd5a631a3af2dab0075f13aaea955b5de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **408.1 MB (408113288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:990c6ecf06eb48e3770c547b32b1db809a870ac24b8351a40eda919b3bd4a8dc`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 18 Mar 2022 00:48:28 GMT
ADD file:4f85f0964cc66c6d7dd6a29e535eb2235ff8847d3c3aa3342c74cc53710ae499 in / 
# Fri, 18 Mar 2022 00:48:34 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 20:09:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 19 Mar 2022 20:10:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 20:31:46 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Sat, 19 Mar 2022 20:33:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 19 Mar 2022 20:33:49 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Mar 2022 20:33:51 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Sat, 19 Mar 2022 20:34:31 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Sun, 20 Mar 2022 00:17:10 GMT
ARG LIBERTY_VERSION=22.0.0.4-beta
# Sun, 20 Mar 2022 00:17:13 GMT
ARG LIBERTY_SHA=a8cbd6e6b91184eda126235f31e63c198ba821dc
# Sun, 20 Mar 2022 00:17:16 GMT
ARG LIBERTY_BUILD_LABEL=cl220320220302-1100
# Sun, 20 Mar 2022 00:17:20 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.4-beta/openliberty-runtime-22.0.0.4-beta.zip
# Sun, 20 Mar 2022 00:17:25 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Sun, 20 Mar 2022 00:17:31 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Sun, 20 Mar 2022 00:17:36 GMT
ARG OPENJ9_SCC=true
# Sun, 20 Mar 2022 00:17:40 GMT
ARG VERBOSE=false
# Sun, 20 Mar 2022 00:17:41 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with IBM Semeru Runtime Open Edition OpenJDK 11 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=22.0.0.4-beta
# Sun, 20 Mar 2022 00:17:43 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Sun, 20 Mar 2022 00:17:45 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sun, 20 Mar 2022 00:18:21 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.4-beta/openliberty-runtime-22.0.0.4-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=a8cbd6e6b91184eda126235f31e63c198ba821dc LIBERTY_VERSION=22.0.0.4-beta OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sun, 20 Mar 2022 00:18:30 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sun, 20 Mar 2022 00:18:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.4-beta/openliberty-runtime-22.0.0.4-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=a8cbd6e6b91184eda126235f31e63c198ba821dc LIBERTY_VERSION=22.0.0.4-beta VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sun, 20 Mar 2022 00:18:53 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.4-beta/openliberty-runtime-22.0.0.4-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=a8cbd6e6b91184eda126235f31e63c198ba821dc LIBERTY_VERSION=22.0.0.4-beta VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sun, 20 Mar 2022 00:19:45 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.4-beta/openliberty-runtime-22.0.0.4-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=a8cbd6e6b91184eda126235f31e63c198ba821dc LIBERTY_VERSION=22.0.0.4-beta VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sun, 20 Mar 2022 00:19:48 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Sun, 20 Mar 2022 00:19:49 GMT
USER 1001
# Sun, 20 Mar 2022 00:19:52 GMT
EXPOSE 9080 9443
# Sun, 20 Mar 2022 00:19:54 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sun, 20 Mar 2022 00:19:56 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:cf1115d7b3bb72f50de3eb695005fb2c88fb88d73f535f164b306c4ab972c570`  
		Last Modified: Fri, 18 Mar 2022 00:51:19 GMT  
		Size: 33.3 MB (33292416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81c83f5d2456f061b5e8436215d94c771940ee113ed327dd33b701564ffa58e`  
		Last Modified: Sat, 19 Mar 2022 20:18:16 GMT  
		Size: 17.2 MB (17205279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31287ee67a63b038a11fb5dae4cdfd185d32800683034a8648e155e1de731493`  
		Last Modified: Sat, 19 Mar 2022 20:44:31 GMT  
		Size: 48.4 MB (48356005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d306304c5f38584058f0e4ec3da1967d38c5cfcebde00783dcece7beea5d05`  
		Last Modified: Sat, 19 Mar 2022 20:44:23 GMT  
		Size: 3.3 MB (3322378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11c1353b575c2b74bcc4eb7bd9e46b14d97f605b93e56b1d2bedf2583787b0e`  
		Last Modified: Sun, 20 Mar 2022 00:58:52 GMT  
		Size: 8.5 KB (8547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ad3a1e57dd4b553ac91929589233ae26fa6eb1af0a9d8a3001cb035ffc188b`  
		Last Modified: Sun, 20 Mar 2022 00:58:49 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea0b00589f6c544f3607e06d49b36e01c828f72b08d51b5e9d58856b40b15e7`  
		Last Modified: Sun, 20 Mar 2022 00:59:13 GMT  
		Size: 293.6 MB (293616207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58483d4ed3c58303a2d2398a4486cfbbde30ba92d0d8ce13304c6cf7993b565a`  
		Last Modified: Sun, 20 Mar 2022 00:58:49 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47fdcbee6f952559ea453a6cc9efd188cbb31cc3e7fe77f929f111f3bfe84799`  
		Last Modified: Sun, 20 Mar 2022 00:58:49 GMT  
		Size: 10.1 KB (10056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a933c033b7920bfd632f6d4167ce693032df6784674c4946ca98a9766503b9b1`  
		Last Modified: Sun, 20 Mar 2022 00:58:52 GMT  
		Size: 12.3 MB (12300862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:beta-java11` - linux; s390x

```console
$ docker pull open-liberty@sha256:b5ae06f04e1ab5764aabddb6e76610337a67b0c0d33be6873d7b9ea3e24b7d12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **401.5 MB (401477666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b303d9527db055289f4912083ee2a8e1166347403110a4f108df39f4b0e492d6`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 18 Mar 2022 00:37:14 GMT
ADD file:5827631949b30d4d05b5515208aedd6d4bc801d2243920cc4fb78e45d0b92bea in / 
# Fri, 18 Mar 2022 00:37:16 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 17:43:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 18 Mar 2022 17:43:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 17:44:58 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1_openj9-0.30.1
# Fri, 18 Mar 2022 17:45:59 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7c639ec9fff1e9d401b9e616bd63bf5cf046bbe6381ba89fdc1b2a2aa31c22bd';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_aarch64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7f2ac9794343a450d0fcf5be392ce4d6abd5f13a6a1c9beb9e69b0d29abc0a60';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_ppc64le_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        amd64|x86_64)          ESUM='f8debbd4326883a47c8afe8bbaabb5ed63d1cd2d82ef42b0fea2c6e2e54f74f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_x64_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        s390x)          ESUM='c0707d8389945f144f8910314ae8eed1d99dd7a653ae3d8e2f58ce656e3c7349';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.14.1%2B1_openj9-0.30.1/ibm-semeru-open-jre_s390x_linux_11.0.14.1_1_openj9-0.30.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 18 Mar 2022 17:46:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Mar 2022 17:46:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Fri, 18 Mar 2022 17:46:34 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Fri, 18 Mar 2022 18:05:46 GMT
ARG LIBERTY_VERSION=22.0.0.4-beta
# Fri, 18 Mar 2022 18:05:46 GMT
ARG LIBERTY_SHA=a8cbd6e6b91184eda126235f31e63c198ba821dc
# Fri, 18 Mar 2022 18:05:46 GMT
ARG LIBERTY_BUILD_LABEL=cl220320220302-1100
# Fri, 18 Mar 2022 18:05:46 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.4-beta/openliberty-runtime-22.0.0.4-beta.zip
# Fri, 18 Mar 2022 18:05:46 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Fri, 18 Mar 2022 18:05:47 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Fri, 18 Mar 2022 18:05:47 GMT
ARG OPENJ9_SCC=true
# Fri, 18 Mar 2022 18:05:47 GMT
ARG VERBOSE=false
# Fri, 18 Mar 2022 18:05:47 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with IBM Semeru Runtime Open Edition OpenJDK 11 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=22.0.0.4-beta
# Fri, 18 Mar 2022 18:05:47 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Fri, 18 Mar 2022 18:05:47 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 18 Mar 2022 18:06:03 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.4-beta/openliberty-runtime-22.0.0.4-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=a8cbd6e6b91184eda126235f31e63c198ba821dc LIBERTY_VERSION=22.0.0.4-beta OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 18 Mar 2022 18:06:08 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 18 Mar 2022 18:06:09 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.4-beta/openliberty-runtime-22.0.0.4-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=a8cbd6e6b91184eda126235f31e63c198ba821dc LIBERTY_VERSION=22.0.0.4-beta VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 18 Mar 2022 18:06:09 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.4-beta/openliberty-runtime-22.0.0.4-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=a8cbd6e6b91184eda126235f31e63c198ba821dc LIBERTY_VERSION=22.0.0.4-beta VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 18 Mar 2022 18:06:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/22.0.0.4-beta/openliberty-runtime-22.0.0.4-beta.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=a8cbd6e6b91184eda126235f31e63c198ba821dc LIBERTY_VERSION=22.0.0.4-beta VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 18 Mar 2022 18:06:31 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Fri, 18 Mar 2022 18:06:31 GMT
USER 1001
# Fri, 18 Mar 2022 18:06:31 GMT
EXPOSE 9080 9443
# Fri, 18 Mar 2022 18:06:31 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 18 Mar 2022 18:06:31 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:709bbd04f56c5b854c32271f7441419f9a84086a0425b65a4bf8e7bb6e6adead`  
		Last Modified: Fri, 18 Mar 2022 00:38:44 GMT  
		Size: 27.1 MB (27084832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0777226b5521f9913ce20a43e00d1a7e6408add50a54f88ffd01f70cecf1e6`  
		Last Modified: Fri, 18 Mar 2022 17:51:28 GMT  
		Size: 15.7 MB (15739697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63430b80eb5f44ccf1dd404e7aa7e6f91c328799416b424cb5b85ddbeac3fd7`  
		Last Modified: Fri, 18 Mar 2022 17:52:18 GMT  
		Size: 46.7 MB (46692259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da42904d6bfe0d4b4695c5f1c08250b03b5461679ca28501b99e50528b8f8cf6`  
		Last Modified: Fri, 18 Mar 2022 17:52:12 GMT  
		Size: 4.3 MB (4337783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe101a6b812e3e7b2aa73c0e469d52195ff0abd9a2a7c0a2e7ed4ca1e0b0a77`  
		Last Modified: Fri, 18 Mar 2022 18:16:56 GMT  
		Size: 8.6 KB (8551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5847dd295feed3d984813811123898788c7bc8eada7fa256bf8bd0bfb5297ee`  
		Last Modified: Fri, 18 Mar 2022 18:16:55 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a937237bb76ba600a74d5766c063585b2dec7e16dad33ac0e169e95aac4838e1`  
		Last Modified: Fri, 18 Mar 2022 18:17:06 GMT  
		Size: 293.6 MB (293615859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f692ab5e7b63cf9ed44b32d8d49dbb710c4f397689c924484f6f4e24809aa6d7`  
		Last Modified: Fri, 18 Mar 2022 18:16:54 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e085f7535164154c56aef2f242909bdc0cf81eee9f4b998f3f694a3a2eaa81c`  
		Last Modified: Fri, 18 Mar 2022 18:16:55 GMT  
		Size: 10.0 KB (10048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510d6d60815873818a302578a5688dee7ded4e135b616fdde0b9a9ac0e02001c`  
		Last Modified: Fri, 18 Mar 2022 18:16:56 GMT  
		Size: 14.0 MB (13987105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
