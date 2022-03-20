## `open-liberty:kernel-slim-java8-openj9`

```console
$ docker pull open-liberty@sha256:fdd18ca6ffa81e5e447329a57a337926bc996b33e0f7a5893a2be97ee4b43312
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:kernel-slim-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:5514363601ea71981603f3cc2ba4e856e1014175934b09295f619802840d2e56
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.4 MB (113436473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fda3374b07dfa2936755459e649daea867da10923e90c820ac1df234055521e`
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
# Thu, 03 Mar 2022 23:58:56 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Thu, 03 Mar 2022 23:59:52 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 03 Mar 2022 23:59:52 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 03:43:04 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 17 Mar 2022 03:43:39 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Sat, 19 Mar 2022 17:55:11 GMT
ARG LIBERTY_VERSION=22.0.0.3
# Sat, 19 Mar 2022 17:55:12 GMT
ARG LIBERTY_SHA=9d22fb7415f8e4b9f6246c57b8f38bba191b697b
# Sat, 19 Mar 2022 17:55:12 GMT
ARG LIBERTY_BUILD_LABEL=cl220320220302-1100
# Sat, 19 Mar 2022 17:55:12 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.3/openliberty-kernel-22.0.0.3.zip
# Sat, 19 Mar 2022 17:55:12 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Sat, 19 Mar 2022 17:55:12 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Sat, 19 Mar 2022 17:55:12 GMT
ARG OPENJ9_SCC=true
# Sat, 19 Mar 2022 17:55:12 GMT
ARG VERBOSE=false
# Sat, 19 Mar 2022 17:55:12 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.3
# Sat, 19 Mar 2022 17:55:12 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Sat, 19 Mar 2022 17:55:12 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sat, 19 Mar 2022 17:55:18 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.3/openliberty-kernel-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9d22fb7415f8e4b9f6246c57b8f38bba191b697b LIBERTY_VERSION=22.0.0.3 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sat, 19 Mar 2022 17:55:18 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sat, 19 Mar 2022 17:55:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.3/openliberty-kernel-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9d22fb7415f8e4b9f6246c57b8f38bba191b697b LIBERTY_VERSION=22.0.0.3 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 19 Mar 2022 17:55:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.3/openliberty-kernel-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9d22fb7415f8e4b9f6246c57b8f38bba191b697b LIBERTY_VERSION=22.0.0.3 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sat, 19 Mar 2022 17:55:26 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.3/openliberty-kernel-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9d22fb7415f8e4b9f6246c57b8f38bba191b697b LIBERTY_VERSION=22.0.0.3 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sat, 19 Mar 2022 17:55:26 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Sat, 19 Mar 2022 17:55:26 GMT
USER 1001
# Sat, 19 Mar 2022 17:55:26 GMT
EXPOSE 9080 9443
# Sat, 19 Mar 2022 17:55:27 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sat, 19 Mar 2022 17:55:27 GMT
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
	-	`sha256:1c515c1adfc3a7f9bb549f560de1547b50dbdad87445623a06545eecc01ae258`  
		Last Modified: Fri, 04 Mar 2022 00:07:16 GMT  
		Size: 50.0 MB (49952788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d50ffaa9cbdc80d62ff6966566fb1ac3ee9a2b9a4d9aeb3bb1d9aef3af5029`  
		Last Modified: Thu, 17 Mar 2022 03:52:05 GMT  
		Size: 4.3 MB (4314621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17ef4917768a405ce97e7381f30450ea8dcb804d1dfaf34c0eb918e541b235b`  
		Last Modified: Sat, 19 Mar 2022 18:01:29 GMT  
		Size: 8.1 KB (8108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b3d5a1e7aae833fea852883e9e6ff72fd2bc7622d59fe472d2e2b551791be1`  
		Last Modified: Sat, 19 Mar 2022 18:01:27 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c4a9e03e6f1c2c228556a7daaf42eda8d8260e947b4b222daa92c6d3257127`  
		Last Modified: Sat, 19 Mar 2022 18:01:28 GMT  
		Size: 12.1 MB (12052062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3dbd71aab08de4f46462834db458be287b4c4107110faccf4d653bc57cb539`  
		Last Modified: Sat, 19 Mar 2022 18:01:27 GMT  
		Size: 940.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5119fdaa7df16bc9dd7434a58201a0947e8a5db2403f0ec582bc9bf4378afd0`  
		Last Modified: Sat, 19 Mar 2022 18:01:27 GMT  
		Size: 9.2 KB (9209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c0963eaeca279e4c915acc0575ebb1c7509a4b281cf7110901633671e6531a`  
		Last Modified: Sat, 19 Mar 2022 18:01:28 GMT  
		Size: 2.5 MB (2501859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-slim-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:3b2e56f4389242734e37955410cfe07b0d577ed1b3a8e62c4eac75c7d2f06012
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118650962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e6ff75b22d423d6ca2d24c227e673480f8c244e9b03951b67bf420af0454fcc`
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
# Sat, 19 Mar 2022 20:28:58 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Sat, 19 Mar 2022 20:30:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 19 Mar 2022 20:30:43 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Mar 2022 20:30:45 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Sat, 19 Mar 2022 20:31:27 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Sun, 20 Mar 2022 00:23:31 GMT
ARG LIBERTY_VERSION=22.0.0.3
# Sun, 20 Mar 2022 00:23:34 GMT
ARG LIBERTY_SHA=9d22fb7415f8e4b9f6246c57b8f38bba191b697b
# Sun, 20 Mar 2022 00:23:36 GMT
ARG LIBERTY_BUILD_LABEL=cl220320220302-1100
# Sun, 20 Mar 2022 00:23:40 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.3/openliberty-kernel-22.0.0.3.zip
# Sun, 20 Mar 2022 00:23:42 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Sun, 20 Mar 2022 00:23:44 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Sun, 20 Mar 2022 00:23:46 GMT
ARG OPENJ9_SCC=true
# Sun, 20 Mar 2022 00:23:48 GMT
ARG VERBOSE=false
# Sun, 20 Mar 2022 00:23:53 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.3
# Sun, 20 Mar 2022 00:23:55 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Sun, 20 Mar 2022 00:23:56 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sun, 20 Mar 2022 00:24:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.3/openliberty-kernel-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9d22fb7415f8e4b9f6246c57b8f38bba191b697b LIBERTY_VERSION=22.0.0.3 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sun, 20 Mar 2022 00:24:20 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sun, 20 Mar 2022 00:24:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.3/openliberty-kernel-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9d22fb7415f8e4b9f6246c57b8f38bba191b697b LIBERTY_VERSION=22.0.0.3 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sun, 20 Mar 2022 00:24:38 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.3/openliberty-kernel-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9d22fb7415f8e4b9f6246c57b8f38bba191b697b LIBERTY_VERSION=22.0.0.3 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sun, 20 Mar 2022 00:24:58 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.3/openliberty-kernel-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9d22fb7415f8e4b9f6246c57b8f38bba191b697b LIBERTY_VERSION=22.0.0.3 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sun, 20 Mar 2022 00:25:01 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Sun, 20 Mar 2022 00:25:06 GMT
USER 1001
# Sun, 20 Mar 2022 00:25:11 GMT
EXPOSE 9080 9443
# Sun, 20 Mar 2022 00:25:17 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sun, 20 Mar 2022 00:25:22 GMT
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
	-	`sha256:43129e3089643c88de6bd2faca8222bfc1eb82c6d0b095cb3ffe8937dfb56b7a`  
		Last Modified: Sat, 19 Mar 2022 20:43:32 GMT  
		Size: 50.4 MB (50445485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fcef59f8a7cdb6034c8a9c0eeb221ddac45a122488dbc79c2fbfacdc0c95d48`  
		Last Modified: Sat, 19 Mar 2022 20:43:28 GMT  
		Size: 3.5 MB (3471997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8774368b7ccae90b58be95b9db1b1a8f85f973436a43beae1256816dab468bb2`  
		Last Modified: Sun, 20 Mar 2022 00:59:59 GMT  
		Size: 8.1 KB (8113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:813606b2c76288e3179ffb4dd27c90a6082e219f396eabe905073ec5bc89c241`  
		Last Modified: Sun, 20 Mar 2022 00:59:55 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972e3dc394d3274a0eebf0ff5b761ca41c9f4462425c8b4e7b1f3d52cf503d48`  
		Last Modified: Sun, 20 Mar 2022 00:59:57 GMT  
		Size: 11.7 MB (11740935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4986383397726f6797777d9aa0b792e78d3767e27550ee43ccc186f141d5f2`  
		Last Modified: Sun, 20 Mar 2022 00:59:56 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecab51d3cda51b089d5437a1ec3e4fc0a99e462cca6ccdf1ec92fefc359c2587`  
		Last Modified: Sun, 20 Mar 2022 00:59:55 GMT  
		Size: 9.2 KB (9233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dcd4b15204950b58f77f1882da77cdd4e9cdf136b211119e75b792335c35c3`  
		Last Modified: Sun, 20 Mar 2022 00:59:56 GMT  
		Size: 2.5 MB (2476289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-slim-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:fdcf525c98608f911648358daa7c484741cc77633d7abc72b5795eaeef798628
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110584871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:148e7f29c01ffc9f6a20693edd90f85229a4220245478498f2dd25af2d107c67`
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
# Fri, 18 Mar 2022 17:43:19 GMT
ENV JAVA_VERSION=jdk8u322-b06_openj9-0.30.0
# Fri, 18 Mar 2022 17:44:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4ab48680e1bab366d6161fd131e6fdfc4ba1ed9b777f519c00a6719e7d23e90';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_aarch64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='207442401f7f672a0f89e6bc2542235d4f7f0fe02f8d485d0b2cdbe69965bce1';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_ppc64le_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9744927fa07671cde675e90efc4b8f72dff8a7fb13fbf86339548c61f93dc486';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_x64_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        s390x)          ESUM='f711dbcacc0964efcf8354eace0b1d2a3e7f58271612430745b4d4b986fdc63d';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u322-b06_openj9-0.30.0/ibm-semeru-open-jre_s390x_linux_8u322b06_openj9-0.30.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 18 Mar 2022 17:44:19 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Mar 2022 17:44:19 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Fri, 18 Mar 2022 17:44:51 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Fri, 18 Mar 2022 18:07:42 GMT
ARG LIBERTY_VERSION=22.0.0.3
# Fri, 18 Mar 2022 18:07:42 GMT
ARG LIBERTY_SHA=9d22fb7415f8e4b9f6246c57b8f38bba191b697b
# Fri, 18 Mar 2022 18:07:42 GMT
ARG LIBERTY_BUILD_LABEL=cl220320220302-1100
# Fri, 18 Mar 2022 18:07:42 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.3/openliberty-kernel-22.0.0.3.zip
# Fri, 18 Mar 2022 18:07:42 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Fri, 18 Mar 2022 18:07:42 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Fri, 18 Mar 2022 18:07:43 GMT
ARG OPENJ9_SCC=true
# Fri, 18 Mar 2022 18:07:43 GMT
ARG VERBOSE=false
# Fri, 18 Mar 2022 18:07:43 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl220320220302-1100 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.3
# Fri, 18 Mar 2022 18:07:43 GMT
COPY dir:dea07490d51f53c887a4a2d6ade59fdcb72993a025bee3d76672fb9870bb0ef2 in /opt/ol/helpers 
# Fri, 18 Mar 2022 18:07:43 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 18 Mar 2022 18:07:48 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.3/openliberty-kernel-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9d22fb7415f8e4b9f6246c57b8f38bba191b697b LIBERTY_VERSION=22.0.0.3 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 18 Mar 2022 18:07:48 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 18 Mar 2022 18:07:49 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.3/openliberty-kernel-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9d22fb7415f8e4b9f6246c57b8f38bba191b697b LIBERTY_VERSION=22.0.0.3 VERBOSE=false
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 18 Mar 2022 18:07:50 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.3/openliberty-kernel-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9d22fb7415f8e4b9f6246c57b8f38bba191b697b LIBERTY_VERSION=22.0.0.3 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 18 Mar 2022 18:07:54 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220320220302-1100 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-kernel/22.0.0.3/openliberty-kernel-22.0.0.3.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=9d22fb7415f8e4b9f6246c57b8f38bba191b697b LIBERTY_VERSION=22.0.0.3 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache /output/workarea     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 18 Mar 2022 18:07:54 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Fri, 18 Mar 2022 18:07:55 GMT
USER 1001
# Fri, 18 Mar 2022 18:07:55 GMT
EXPOSE 9080 9443
# Fri, 18 Mar 2022 18:07:55 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 18 Mar 2022 18:07:55 GMT
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
	-	`sha256:b612a02d2a499cb5f5d15171088e4cfd33d79e9e9c2404ddaab5b951ad4d6c66`  
		Last Modified: Fri, 18 Mar 2022 17:51:46 GMT  
		Size: 49.2 MB (49184592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12ca14bd9d54e5bdbf1608bc8cfefad7abab55fec8a058d1ec23bb8222b6daf`  
		Last Modified: Fri, 18 Mar 2022 17:51:41 GMT  
		Size: 4.3 MB (4287719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85b8c1be1bda05631953fd055bc65751d816164fb084dbd0d80739e0c78d2ba`  
		Last Modified: Fri, 18 Mar 2022 18:17:30 GMT  
		Size: 8.1 KB (8113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7caeaa94acec9f3d0a0b881d38df7bae7fca603efebecf474fa0f23f94ff4cb`  
		Last Modified: Fri, 18 Mar 2022 18:17:29 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f860751da30ef1bd3e17f48033b0a20b9aad5dac908da9d41e111074422e64e2`  
		Last Modified: Fri, 18 Mar 2022 18:17:29 GMT  
		Size: 11.7 MB (11740559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98afca8962aeafa5a238f0c6cbcf8c58a84e2b09373aec35c82ba1114c5f2d43`  
		Last Modified: Fri, 18 Mar 2022 18:17:29 GMT  
		Size: 941.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f23abb0e59a142c82e984b5ab46dfea62bdd6474606a4ee7ba91dd07e91ef4f`  
		Last Modified: Fri, 18 Mar 2022 18:17:29 GMT  
		Size: 9.2 KB (9208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a5d53bb59d933be3481b46cf8322099ca7b23761fab1cfa71cff07040682a5`  
		Last Modified: Fri, 18 Mar 2022 18:17:29 GMT  
		Size: 2.5 MB (2528944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
