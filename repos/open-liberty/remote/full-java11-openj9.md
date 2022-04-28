## `open-liberty:full-java11-openj9`

```console
$ docker pull open-liberty@sha256:5ea475aa2a05906e6648880d6971542bdc6aed30909b39c9883e8df2d4c3ea1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:full-java11-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:2193ca84ed0b0bba60a9b82d3e4f2503c9cbb874ebe07d76d0181de3295b4a97
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.8 MB (395837409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:501e52a5ae31c39416b3af70e70eba03559d8a47e565704245fb97908f1664eb`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

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
# Wed, 27 Apr 2022 21:28:51 GMT
ARG LIBERTY_VERSION=22.0.0.4
# Wed, 27 Apr 2022 21:30:18 GMT
ARG LIBERTY_SHA=4c7e360f5564a246a3accc46386d6cdd5360e2fb
# Wed, 27 Apr 2022 21:30:18 GMT
ARG LIBERTY_BUILD_LABEL=cl220420220328-1303
# Wed, 27 Apr 2022 21:30:18 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.4/openliberty-runtime-22.0.0.4.zip
# Wed, 27 Apr 2022 21:30:18 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 27 Apr 2022 21:30:18 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 27 Apr 2022 21:30:19 GMT
ARG OPENJ9_SCC=true
# Wed, 27 Apr 2022 21:30:19 GMT
ARG VERBOSE=false
# Wed, 27 Apr 2022 21:30:19 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl220420220328-1303 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.4
# Wed, 27 Apr 2022 21:30:19 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 27 Apr 2022 21:30:19 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 27 Apr 2022 21:30:32 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220420220328-1303 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.4/openliberty-runtime-22.0.0.4.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=4c7e360f5564a246a3accc46386d6cdd5360e2fb LIBERTY_VERSION=22.0.0.4 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 27 Apr 2022 21:30:32 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 27 Apr 2022 21:30:33 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220420220328-1303 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.4/openliberty-runtime-22.0.0.4.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=4c7e360f5564a246a3accc46386d6cdd5360e2fb LIBERTY_VERSION=22.0.0.4 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 27 Apr 2022 21:30:34 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220420220328-1303 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.4/openliberty-runtime-22.0.0.4.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=4c7e360f5564a246a3accc46386d6cdd5360e2fb LIBERTY_VERSION=22.0.0.4 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 27 Apr 2022 21:31:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220420220328-1303 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.4/openliberty-runtime-22.0.0.4.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=4c7e360f5564a246a3accc46386d6cdd5360e2fb LIBERTY_VERSION=22.0.0.4 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 27 Apr 2022 21:31:00 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 27 Apr 2022 21:31:00 GMT
USER 1001
# Wed, 27 Apr 2022 21:31:00 GMT
EXPOSE 9080 9443
# Wed, 27 Apr 2022 21:31:00 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 27 Apr 2022 21:31:00 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:0313d3c3a133e131fbbefaa2247ce43132b78d08631cfd02146847579b0cba44`  
		Last Modified: Wed, 27 Apr 2022 21:41:43 GMT  
		Size: 8.6 KB (8551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cefd7d4443a184a9bf0b0453333626685b1932b983af9102c3f042833601558`  
		Last Modified: Wed, 27 Apr 2022 21:41:40 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96be080ceac27347ba547dbe6261c7ab74dcb37e553ba4f8622f27641e6cc55d`  
		Last Modified: Wed, 27 Apr 2022 21:41:54 GMT  
		Size: 285.4 MB (285444033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd1d7856564e9016f731a31df84bbc41f9f16a413bdda44c3b8911332c48258`  
		Last Modified: Wed, 27 Apr 2022 21:41:40 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4abc9a53bd03a7152aa28e6fed71221db5307cc22fcbbbc7c12dafedd71c469`  
		Last Modified: Wed, 27 Apr 2022 21:41:41 GMT  
		Size: 10.0 KB (10044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db04fd0b8805a58ffd9e4bc7d0ac96163e090ea7ea3304f1f001e4d59349f4f4`  
		Last Modified: Wed, 27 Apr 2022 21:41:43 GMT  
		Size: 13.9 MB (13871375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full-java11-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:74b7f46eb339d05ca9f862c97661975f0aff8c0d857b313748b0e11bea3eaa6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **400.1 MB (400069740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abacc03bbdaa13ef326be61e5ec85dd64047c79adc69509db4ae434550966c34`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

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
# Thu, 28 Apr 2022 02:00:59 GMT
ARG LIBERTY_VERSION=22.0.0.4
# Thu, 28 Apr 2022 02:07:14 GMT
ARG LIBERTY_SHA=4c7e360f5564a246a3accc46386d6cdd5360e2fb
# Thu, 28 Apr 2022 02:07:18 GMT
ARG LIBERTY_BUILD_LABEL=cl220420220328-1303
# Thu, 28 Apr 2022 02:07:25 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.4/openliberty-runtime-22.0.0.4.zip
# Thu, 28 Apr 2022 02:07:29 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Thu, 28 Apr 2022 02:07:37 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Thu, 28 Apr 2022 02:07:40 GMT
ARG OPENJ9_SCC=true
# Thu, 28 Apr 2022 02:07:48 GMT
ARG VERBOSE=false
# Thu, 28 Apr 2022 02:07:50 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl220420220328-1303 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.4
# Thu, 28 Apr 2022 02:07:52 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Thu, 28 Apr 2022 02:07:53 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 28 Apr 2022 02:08:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220420220328-1303 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.4/openliberty-runtime-22.0.0.4.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=4c7e360f5564a246a3accc46386d6cdd5360e2fb LIBERTY_VERSION=22.0.0.4 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 28 Apr 2022 02:08:35 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 28 Apr 2022 02:08:42 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220420220328-1303 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.4/openliberty-runtime-22.0.0.4.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=4c7e360f5564a246a3accc46386d6cdd5360e2fb LIBERTY_VERSION=22.0.0.4 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 28 Apr 2022 02:08:47 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220420220328-1303 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.4/openliberty-runtime-22.0.0.4.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=4c7e360f5564a246a3accc46386d6cdd5360e2fb LIBERTY_VERSION=22.0.0.4 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 28 Apr 2022 02:09:32 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220420220328-1303 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.4/openliberty-runtime-22.0.0.4.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=4c7e360f5564a246a3accc46386d6cdd5360e2fb LIBERTY_VERSION=22.0.0.4 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 28 Apr 2022 02:09:35 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 28 Apr 2022 02:09:37 GMT
USER 1001
# Thu, 28 Apr 2022 02:09:39 GMT
EXPOSE 9080 9443
# Thu, 28 Apr 2022 02:09:41 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 28 Apr 2022 02:09:43 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
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
	-	`sha256:70edcfa714249473d579cc4534d70e21b221e87d069ac0dcc6510ccf214e2acf`  
		Last Modified: Thu, 28 Apr 2022 02:48:00 GMT  
		Size: 8.5 KB (8547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afaa5a545374f026f1c61f53fa71fd039d660a35da737f7387645bce554f8974`  
		Last Modified: Thu, 28 Apr 2022 02:47:57 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af8dbe41e82e4b41dc23cab306e7d5ba1b7ec236f64624996ebd896caf92d5c`  
		Last Modified: Thu, 28 Apr 2022 02:48:43 GMT  
		Size: 285.4 MB (285444613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95bdd60a52865380f652ebecb3a3d7bacc0cd011167796c08c98bf34d1cfde82`  
		Last Modified: Thu, 28 Apr 2022 02:47:57 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1840d9fad891d076dea73562105eeb405ba46e087bcaefb076708e4671de7d`  
		Last Modified: Thu, 28 Apr 2022 02:47:57 GMT  
		Size: 10.0 KB (10049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fb3fe2583b107ea44d9a423a5c9d47319b613c56cd5cca1aec9b22cee883ec`  
		Last Modified: Thu, 28 Apr 2022 02:48:00 GMT  
		Size: 12.4 MB (12388829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full-java11-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:8b180d97ab653ff045ece786102f992a29a5b2ace20f1a38ef6dae440c84a235
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.3 MB (393267657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce4e5bd928f3ec9b18c3cfc96dec447c586513f1d66f3a94536ea6d532749627`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 01:54:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 01:55:39 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Apr 2022 19:43:25 GMT
ENV JAVA_VERSION=jdk-11.0.15+10_openj9-0.32.0
# Wed, 27 Apr 2022 19:44:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69e4a0b383c7b4187478ddb196de3cdc91560e2be40b8ef66354591e87c36e85';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5e82f7df54786c557d2d9e9ac22df655fd94b9702c73261390903ac87532d545';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='25d4d5e2bbe3eb19bcb9a76aec4b43d4eef5ad66200df3122118f69da5325cf6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='def85f1b00e9c65a8c3b5dcf4da0f1b04c17675b4ff9cd6f5dad61d8dcbd03d0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.15%2B10_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_11.0.15_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 27 Apr 2022 19:44:30 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Apr 2022 19:44:30 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 27 Apr 2022 19:45:04 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 27 Apr 2022 21:27:24 GMT
ARG LIBERTY_VERSION=22.0.0.4
# Wed, 27 Apr 2022 21:30:03 GMT
ARG LIBERTY_SHA=4c7e360f5564a246a3accc46386d6cdd5360e2fb
# Wed, 27 Apr 2022 21:30:03 GMT
ARG LIBERTY_BUILD_LABEL=cl220420220328-1303
# Wed, 27 Apr 2022 21:30:03 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.4/openliberty-runtime-22.0.0.4.zip
# Wed, 27 Apr 2022 21:30:04 GMT
ARG LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE
# Wed, 27 Apr 2022 21:30:04 GMT
ARG LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7
# Wed, 27 Apr 2022 21:30:05 GMT
ARG OPENJ9_SCC=true
# Wed, 27 Apr 2022 21:30:05 GMT
ARG VERBOSE=false
# Wed, 27 Apr 2022 21:30:05 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Leo Christy Jesuraj org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl220420220328-1303 org.opencontainers.image.description=This image contains the Open Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=22.0.0.4
# Wed, 27 Apr 2022 21:30:06 GMT
COPY dir:e4ff10e677106842e92e637318ee2b51440fb46859dd7032cee783fd3955cb73 in /opt/ol/helpers 
# Wed, 27 Apr 2022 21:30:06 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 27 Apr 2022 21:30:47 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220420220328-1303 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.4/openliberty-runtime-22.0.0.4.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=4c7e360f5564a246a3accc46386d6cdd5360e2fb LIBERTY_VERSION=22.0.0.4 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && wget -q $LIBERTY_LICENSE_URL -O /licenses/LICENSE     && echo "$LIBERTY_LICENSE_SHA /licenses/LICENSE" | sha1sum -c --strict --check     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 27 Apr 2022 21:31:02 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 27 Apr 2022 21:31:03 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220420220328-1303 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.4/openliberty-runtime-22.0.0.4.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=4c7e360f5564a246a3accc46386d6cdd5360e2fb LIBERTY_VERSION=22.0.0.4 VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 27 Apr 2022 21:31:04 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220420220328-1303 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.4/openliberty-runtime-22.0.0.4.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=4c7e360f5564a246a3accc46386d6cdd5360e2fb LIBERTY_VERSION=22.0.0.4 VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 27 Apr 2022 21:31:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl220420220328-1303 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/22.0.0.4/openliberty-runtime-22.0.0.4.zip LIBERTY_LICENSE_SHA=84f00503d6516c91190de866e78d6010899673b7 LIBERTY_LICENSE_URL=https://raw.githubusercontent.com/OpenLiberty/open-liberty/master/LICENSE LIBERTY_SHA=4c7e360f5564a246a3accc46386d6cdd5360e2fb LIBERTY_VERSION=22.0.0.4 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 27 Apr 2022 21:31:29 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 27 Apr 2022 21:31:29 GMT
USER 1001
# Wed, 27 Apr 2022 21:31:29 GMT
EXPOSE 9080 9443
# Wed, 27 Apr 2022 21:31:29 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 27 Apr 2022 21:31:29 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ad99882b01b0ab3e7045a65b2c93f1319b8763364d776de22578aaade5be51`  
		Last Modified: Fri, 22 Apr 2022 02:02:24 GMT  
		Size: 15.7 MB (15738876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66deee1f4946e000ec003b0c3abf1d14dfc64eafa125296784e8b03711fb4d25`  
		Last Modified: Wed, 27 Apr 2022 19:51:12 GMT  
		Size: 46.7 MB (46721679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4c21f99632efa3864a937316f8654db3b26ce698223f4c67f9f4544b6c359a`  
		Last Modified: Wed, 27 Apr 2022 19:51:07 GMT  
		Size: 4.3 MB (4290538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56156de35f300ae9952b95a69fa8f437a4b63d2d7986e7f11379219760f0ce56`  
		Last Modified: Wed, 27 Apr 2022 21:43:53 GMT  
		Size: 8.6 KB (8552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5027f513f7e365a660e6b8a4f58b63b835e42cb4936e0da4e7adadd86beae5ab`  
		Last Modified: Wed, 27 Apr 2022 21:43:51 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aca69514bd1f16af65af1bc4021e7c63c22ccd702466094fd4df2d59ac61767`  
		Last Modified: Wed, 27 Apr 2022 21:44:03 GMT  
		Size: 285.4 MB (285444395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdbe83b4f47d07718d799fda801f5103a8372dcc0c393a6ec849d3d59c1842c`  
		Last Modified: Wed, 27 Apr 2022 21:43:52 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7f27bd971125a0198d1bcc4c570335ada464f41e30365e352b8338f13d888e`  
		Last Modified: Wed, 27 Apr 2022 21:43:51 GMT  
		Size: 10.1 KB (10052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535e9481a61e95dc9aeee95c5e7e99cc94e9bc8ba6e4903ee320687466f56cfd`  
		Last Modified: Wed, 27 Apr 2022 21:43:53 GMT  
		Size: 14.0 MB (13966316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
