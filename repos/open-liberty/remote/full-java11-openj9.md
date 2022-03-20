## `open-liberty:full-java11-openj9`

```console
$ docker pull open-liberty@sha256:fe84189ad20b26f80fcf0a994e8ca20f1894bca9b0b355b6bda7dacc889fd509
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:full-java11-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:8e98db07a4f999a5e9fed64b70c0707473dd04f67d297d5555089370e3369882
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.9 MB (395901966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13443beb667d2ef2c262326bea59f75b33d2b1952fa1f8cfe64082d5098e125b`
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
# Sat, 19 Mar 2022 17:55:31 GMT
ARG LIBERTY_VERSION=22.0.0.3
# Sat, 19 Mar 2022 17:57:08 GMT
ARG LIBERTY_SHA=e57c6c986050db8eceb6467e24b3bd78ac33eee2
# Sat, 19 Mar 2022 17:57:09 GMT
ARG LIBERTY_BUILD_LABEL=cl220320220302-1100
# Sat, 19 Mar 2022 17:57:09 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.3/openliberty-runtime-22.0.0.3.zip
# Sat, 19 Mar 2022 17:57:09 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Sat, 19 Mar 2022 17:57:09 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Sat, 19 Mar 2022 17:57:09 GMT
ARG OPENJ9_SCC=true
# Sat, 19 Mar 2022 17:57:09 GMT
ARG VERBOSE=false
# Sat, 19 Mar 2022 17:57:09 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.3
# Sat, 19 Mar 2022 17:57:09 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Sat, 19 Mar 2022 17:57:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sat, 19 Mar 2022 17:57:22 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.3/openliberty-runtime-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=e57c6c986050db8eceb6467e24b3bd78ac33eee2 LIBERTY_VERSION=22.0.0.3 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sat, 19 Mar 2022 17:57:23 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sat, 19 Mar 2022 17:57:24 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.3/openliberty-runtime-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=e57c6c986050db8eceb6467e24b3bd78ac33eee2 LIBERTY_VERSION=22.0.0.3 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 19 Mar 2022 17:57:24 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.3/openliberty-runtime-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=e57c6c986050db8eceb6467e24b3bd78ac33eee2 LIBERTY_VERSION=22.0.0.3 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sat, 19 Mar 2022 17:58:02 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.3/openliberty-runtime-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=e57c6c986050db8eceb6467e24b3bd78ac33eee2 LIBERTY_VERSION=22.0.0.3 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sat, 19 Mar 2022 17:58:02 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Sat, 19 Mar 2022 17:58:02 GMT
USER 1001
# Sat, 19 Mar 2022 17:58:02 GMT
EXPOSE 9080 9443
# Sat, 19 Mar 2022 17:58:02 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sat, 19 Mar 2022 17:58:02 GMT
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
	-	`sha256:cedba220b11875d9ca0deae34741980a811b28a4f50520290640f47ac25e9f07`  
		Last Modified: Sat, 19 Mar 2022 18:02:27 GMT  
		Size: 8.5 KB (8549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb2ce5b3c9226f61c2fe49eae5383a0f6b43edfa760d1b617d5d3175dad8b5d`  
		Last Modified: Sat, 19 Mar 2022 18:02:24 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36104244404c90b189ed6d3fcdb7bd25e3b4514c3eaf0406d606a207eae690b`  
		Last Modified: Sat, 19 Mar 2022 18:02:40 GMT  
		Size: 285.0 MB (285013304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03a1501514a7ffb66477c79fdae9b4ccd38c5235396dabd46be3fb7e621b26b`  
		Last Modified: Sat, 19 Mar 2022 18:02:24 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9695405e182547cb7777544ef00807376b77d88eeaf89d650aa7d0900716f70c`  
		Last Modified: Sat, 19 Mar 2022 18:02:24 GMT  
		Size: 10.0 KB (10047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58092d981bfe7fb5b30bf8d12f716a314724adb9ca64dadb487089d0e97455b`  
		Last Modified: Sat, 19 Mar 2022 18:02:27 GMT  
		Size: 14.2 MB (14153333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full-java11-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:7c613c3a05b2dc8ca003defaf67bec9f066b0f242fc1ecdbbf5d9a284e11e314
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.2 MB (399192697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fb02a501bc8a0f17bd81b1fef2482db6d441e2f7fe48c170b3dde386f5a426c`
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
# Sun, 20 Mar 2022 00:25:41 GMT
ARG LIBERTY_VERSION=22.0.0.3
# Sun, 20 Mar 2022 00:32:40 GMT
ARG LIBERTY_SHA=e57c6c986050db8eceb6467e24b3bd78ac33eee2
# Sun, 20 Mar 2022 00:32:43 GMT
ARG LIBERTY_BUILD_LABEL=cl220320220302-1100
# Sun, 20 Mar 2022 00:32:45 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.3/openliberty-runtime-22.0.0.3.zip
# Sun, 20 Mar 2022 00:32:50 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Sun, 20 Mar 2022 00:32:53 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Sun, 20 Mar 2022 00:32:57 GMT
ARG OPENJ9_SCC=true
# Sun, 20 Mar 2022 00:33:00 GMT
ARG VERBOSE=false
# Sun, 20 Mar 2022 00:33:02 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.3
# Sun, 20 Mar 2022 00:33:04 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Sun, 20 Mar 2022 00:33:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sun, 20 Mar 2022 00:33:58 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.3/openliberty-runtime-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=e57c6c986050db8eceb6467e24b3bd78ac33eee2 LIBERTY_VERSION=22.0.0.3 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sun, 20 Mar 2022 00:34:05 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sun, 20 Mar 2022 00:34:11 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.3/openliberty-runtime-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=e57c6c986050db8eceb6467e24b3bd78ac33eee2 LIBERTY_VERSION=22.0.0.3 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sun, 20 Mar 2022 00:34:20 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.3/openliberty-runtime-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=e57c6c986050db8eceb6467e24b3bd78ac33eee2 LIBERTY_VERSION=22.0.0.3 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sun, 20 Mar 2022 00:35:13 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.3/openliberty-runtime-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=e57c6c986050db8eceb6467e24b3bd78ac33eee2 LIBERTY_VERSION=22.0.0.3 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sun, 20 Mar 2022 00:35:15 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Sun, 20 Mar 2022 00:35:20 GMT
USER 1001
# Sun, 20 Mar 2022 00:35:24 GMT
EXPOSE 9080 9443
# Sun, 20 Mar 2022 00:35:29 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sun, 20 Mar 2022 00:35:34 GMT
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
	-	`sha256:ea676ee06987205e6c9873246fc66ee13e32f166db171b25e884c28c2de12e72`  
		Last Modified: Sun, 20 Mar 2022 01:01:23 GMT  
		Size: 8.6 KB (8552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9547af7f9d6472f186c40bd8a693f212873ef8b83ecdb1a25781b71452284f44`  
		Last Modified: Sun, 20 Mar 2022 01:01:21 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66e20912f2a3c2dfad5e6ae210943bd162bf5c0005d35aee053f1c4c0b7f0d7`  
		Last Modified: Sun, 20 Mar 2022 01:01:45 GMT  
		Size: 284.7 MB (284703456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f22c7b84baae29ed922b62655e839cc01cec9d27c68ef336f2aaac8c4a5db26c`  
		Last Modified: Sun, 20 Mar 2022 01:01:21 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d782dfc65c0b9eef9a9c72932ec81597efc20710f9347007f818cabf832aa6bf`  
		Last Modified: Sun, 20 Mar 2022 01:01:21 GMT  
		Size: 10.1 KB (10068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b48b03fbbe8e81123c11b241b240d132ac7448f6f1ce6d84264c2ed594ef04`  
		Last Modified: Sun, 20 Mar 2022 01:01:23 GMT  
		Size: 12.3 MB (12293009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full-java11-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:376913d47015387cb8bc0e2b21ed21188c97a289a1936e816b4c561e3496c5cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.5 MB (392528217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aa3ecbb46b0643752d631d4368241cff6e61c93665735210c0f7219a2ea63b5`
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
# Fri, 18 Mar 2022 18:08:01 GMT
ARG LIBERTY_VERSION=22.0.0.3
# Fri, 18 Mar 2022 18:09:30 GMT
ARG LIBERTY_SHA=e57c6c986050db8eceb6467e24b3bd78ac33eee2
# Fri, 18 Mar 2022 18:09:30 GMT
ARG LIBERTY_BUILD_LABEL=cl220320220302-1100
# Fri, 18 Mar 2022 18:09:30 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.3/openliberty-runtime-22.0.0.3.zip
# Fri, 18 Mar 2022 18:09:30 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Fri, 18 Mar 2022 18:09:31 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Fri, 18 Mar 2022 18:09:31 GMT
ARG OPENJ9_SCC=true
# Fri, 18 Mar 2022 18:09:31 GMT
ARG VERBOSE=false
# Fri, 18 Mar 2022 18:09:31 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.3
# Fri, 18 Mar 2022 18:09:31 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Fri, 18 Mar 2022 18:09:31 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 18 Mar 2022 18:09:47 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.3/openliberty-runtime-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=e57c6c986050db8eceb6467e24b3bd78ac33eee2 LIBERTY_VERSION=22.0.0.3 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 18 Mar 2022 18:09:52 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 18 Mar 2022 18:09:52 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.3/openliberty-runtime-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=e57c6c986050db8eceb6467e24b3bd78ac33eee2 LIBERTY_VERSION=22.0.0.3 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 18 Mar 2022 18:09:53 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.3/openliberty-runtime-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=e57c6c986050db8eceb6467e24b3bd78ac33eee2 LIBERTY_VERSION=22.0.0.3 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 18 Mar 2022 18:10:15 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.3/openliberty-runtime-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=e57c6c986050db8eceb6467e24b3bd78ac33eee2 LIBERTY_VERSION=22.0.0.3 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 18 Mar 2022 18:10:15 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Fri, 18 Mar 2022 18:10:15 GMT
USER 1001
# Fri, 18 Mar 2022 18:10:15 GMT
EXPOSE 9080 9443
# Fri, 18 Mar 2022 18:10:16 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 18 Mar 2022 18:10:16 GMT
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
	-	`sha256:b9240cbc613173f267f65cb877368903be62bb0d50f90e8da933107e9a47d421`  
		Last Modified: Fri, 18 Mar 2022 18:18:09 GMT  
		Size: 8.6 KB (8552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b8c572830ca5bd1ba59f5aaddd8dd09dcb015be590da18b862b98b16af3b18`  
		Last Modified: Fri, 18 Mar 2022 18:18:09 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af21826194019b47ea2f806605d4128d7f9772ac762973a81ba6f6d8fb09dc57`  
		Last Modified: Fri, 18 Mar 2022 18:18:19 GMT  
		Size: 284.7 MB (284703080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd0f3cd626eb8d80bb607450b8e535cb0ef48e552be08e08b222e8213f7ba1d`  
		Last Modified: Fri, 18 Mar 2022 18:18:09 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c92a43d85387257f1474685bfd2adc85b233d946b8fb904d8bd693ef9fa991c`  
		Last Modified: Fri, 18 Mar 2022 18:18:08 GMT  
		Size: 10.0 KB (10041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada9301098f0a23dd0597a94cc2326ff574dce424ed8df1d7a245bcd8285b9a8`  
		Last Modified: Fri, 18 Mar 2022 18:18:10 GMT  
		Size: 14.0 MB (13950445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
