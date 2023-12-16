## `open-liberty:beta-java11`

```console
$ docker pull open-liberty@sha256:da9b2ce7e05087a57441e927b31b5c2a50e0c4d7b0d62a4b4d9a5ebbaf3ea8b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:beta-java11` - linux; amd64

```console
$ docker pull open-liberty@sha256:f85edf534bf7134420ec4689b4ce484d2e0233441df7212f282d6c4c5273dab7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **439.5 MB (439515881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e2b9c4b0636254013f8101aed6b05ec930e862ea101062d3d1a627b619c0a53`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 02:23:58 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 02:24:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 02:27:39 GMT
ENV JAVA_VERSION=jdk-11.0.21+9_openj9-0.41.0
# Sat, 02 Dec 2023 02:29:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='5eb5d5d6006e1066b5c72d3b000f1c8fda572fa64189af103ef1176235cd3174';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.21%2B9_openj9-0.41.0/ibm-semeru-open-jre_aarch64_linux_11.0.21_9_openj9-0.41.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='0495d4d122dfb7ae160d9c76549f62fdd77b9c8ceddc9d4aced882c3c5157ba5';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.21%2B9_openj9-0.41.0/ibm-semeru-open-jre_ppc64le_linux_11.0.21_9_openj9-0.41.0.tar.gz';          ;;        amd64|x86_64)          ESUM='324f7e8d75490cc76d5cf6a46b43f50ec1206a97d49e1549d1c65f1583fc51d5';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.21%2B9_openj9-0.41.0/ibm-semeru-open-jre_x64_linux_11.0.21_9_openj9-0.41.0.tar.gz';          ;;        s390x)          ESUM='a061cc8b2df7d42333e1d3ddb90535b8b86f76bd04d5c481d677f8167394249f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.21%2B9_openj9-0.41.0/ibm-semeru-open-jre_s390x_linux_11.0.21_9_openj9-0.41.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 02 Dec 2023 02:29:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 02:29:24 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Sat, 02 Dec 2023 02:29:59 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Sat, 02 Dec 2023 11:28:35 GMT
USER root
# Wed, 13 Dec 2023 18:21:26 GMT
ARG LIBERTY_VERSION=24.0.0.1-beta
# Wed, 13 Dec 2023 18:21:27 GMT
ARG LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4
# Wed, 13 Dec 2023 18:21:27 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip
# Wed, 13 Dec 2023 18:21:27 GMT
ARG LIBERTY_BUILD_LABEL=cl231220231127-1901
# Wed, 13 Dec 2023 18:21:27 GMT
ARG OPENJ9_SCC=true
# Wed, 13 Dec 2023 18:21:27 GMT
ARG VERBOSE=false
# Wed, 13 Dec 2023 18:21:27 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Melissa Lee, Thomas Watson, Michal Broz, Wendy Raschke org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl231220231127-1901 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with IBM Semeru Runtime Open Edition OpenJDK 17 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=24.0.0.1-beta
# Wed, 13 Dec 2023 18:21:27 GMT
COPY file:b2d50545eedb1d5c43e3914a49059b907fd99eab5d731eb6d4ff519f47d88408 in /opt/ol/NOTICES 
# Wed, 13 Dec 2023 18:21:27 GMT
COPY dir:3a03be0df9fe59a90276be087434855a86a8818483ded6f49c3c57610fb6842d in /opt/ol/helpers 
# Wed, 13 Dec 2023 18:21:27 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 13 Dec 2023 18:21:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl231220231127-1901 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4 LIBERTY_VERSION=24.0.0.1-beta OPENJ9_SCC=true VERBOSE=false
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_aarch64';          DUMB_INIT_SHA256=b7d648f97154a99c539b63c55979cd29f005f88430fb383007fe3458340b795e;          ;;        amd64|x86_64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_x86_64';          DUMB_INIT_SHA256=e874b55f3279ca41415d290c512a7ba9d08f98041b28ae7c2acb19a545f1c4df;          ;;        ppc64el|ppc64le)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_ppc64le';          DUMB_INIT_SHA256=3d15e80e29f0f4fa1fc686b00613a2220bc37e83a35283d4b4cca1fbd0a5609f;          ;;        s390x)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_s390x';          DUMB_INIT_SHA256=47e4601b152fc6dcb1891e66c30ecc62a2939fd7ffd1515a7c30f281cfec53b7;          ;;       *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /usr/bin/dumb-init ${DUMB_INIT_URL};     echo "${DUMB_INIT_SHA256} */usr/bin/dumb-init" | sha256sum -c -;     chmod +x /usr/bin/dumb-init;
# Wed, 13 Dec 2023 18:21:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl231220231127-1901 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4 LIBERTY_VERSION=24.0.0.1-beta OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && cp /opt/ol/wlp/LICENSE /licenses/     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 13 Dec 2023 18:21:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ol/wlp/bin:/opt/ol/helpers/build LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 13 Dec 2023 18:21:46 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl231220231127-1901 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4 LIBERTY_VERSION=24.0.0.1-beta VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea     && rm -rf /opt/ol/wlp/usr/servers/defaultServer/server.env
# Wed, 13 Dec 2023 18:21:47 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl231220231127-1901 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4 LIBERTY_VERSION=24.0.0.1-beta VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && ln -s /opt/ol/fixes /fixes     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 13 Dec 2023 18:22:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl231220231127-1901 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4 LIBERTY_VERSION=24.0.0.1-beta VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 13 Dec 2023 18:22:17 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 13 Dec 2023 18:22:17 GMT
USER 1001
# Wed, 13 Dec 2023 18:22:17 GMT
EXPOSE 9080 9443
# Wed, 13 Dec 2023 18:22:18 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 13 Dec 2023 18:22:18 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:cbe3537751ce03ea42788c2fbe2d5d336180dc2e20472c8cdba8b3224191d101`  
		Last Modified: Wed, 29 Nov 2023 19:24:54 GMT  
		Size: 30.4 MB (30446322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a261eab81e521775977f42fd67a3196085829d7723b5ca804ff8e0e504f9526`  
		Last Modified: Sat, 02 Dec 2023 02:37:49 GMT  
		Size: 12.2 MB (12155087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f692ab6864cd14000e7fa8c3715feb08739daed312639a593694d8282e898bb2`  
		Last Modified: Sat, 02 Dec 2023 02:39:41 GMT  
		Size: 49.0 MB (48954945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb8257204401237d1dfef2b9329a6bb81b357b04b5529a8d1bf3d1330b8f485`  
		Last Modified: Sat, 02 Dec 2023 02:39:34 GMT  
		Size: 4.2 MB (4242125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae7bbc2160f08fea8d3d02cc45d7bc04e60131e477dfae3e9caf2e5d37d9013`  
		Last Modified: Wed, 13 Dec 2023 18:28:35 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e83581eff71065f8a49eb08209aea23a61bf16871fb1305610e63ed852e4d12`  
		Last Modified: Wed, 13 Dec 2023 18:28:34 GMT  
		Size: 9.6 KB (9577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b378229ca01aa0c53e37f1c177e67705f9a86b023e7b507c63d95718666ecb`  
		Last Modified: Wed, 13 Dec 2023 18:28:34 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdc86b34c2c2de32ccbd064ead657c897a47a46582327438c8d8492dff8b15b`  
		Last Modified: Wed, 13 Dec 2023 18:28:32 GMT  
		Size: 31.7 KB (31746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104d641818b371a2d774b4e1cd953323d9363502ae2d4c449cb996932ef16dac`  
		Last Modified: Wed, 13 Dec 2023 18:28:47 GMT  
		Size: 330.6 MB (330613196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7a7046ed65da890d519a16846cfb5bb974eeafe2ef3612e3ea3041f8d368c7`  
		Last Modified: Wed, 13 Dec 2023 18:28:32 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249d308e2bb8d192f02837dd07f4690ee6c93268715452b1a70e44145f0bcdcb`  
		Last Modified: Wed, 13 Dec 2023 18:28:32 GMT  
		Size: 11.0 KB (11030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7231a54bef5e9a42237861824f058be73cc802b553d3945fa16b9452322a695f`  
		Last Modified: Wed, 13 Dec 2023 18:28:34 GMT  
		Size: 13.0 MB (13049328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:beta-java11` - linux; arm64 variant v8

```console
$ docker pull open-liberty@sha256:42991fadb5cb3d130a155fb93910409b2c4a5415747b3ca9185d2d4b06eabe61
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **435.4 MB (435418887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:303aba1df73cd73f12dc4395b0d0262416418865a6c864abcf646f9da16407f2`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 07:20:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 07:21:21 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 07:24:21 GMT
ENV JAVA_VERSION=jdk-11.0.21+9_openj9-0.41.0
# Sat, 02 Dec 2023 07:26:02 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='5eb5d5d6006e1066b5c72d3b000f1c8fda572fa64189af103ef1176235cd3174';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.21%2B9_openj9-0.41.0/ibm-semeru-open-jre_aarch64_linux_11.0.21_9_openj9-0.41.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='0495d4d122dfb7ae160d9c76549f62fdd77b9c8ceddc9d4aced882c3c5157ba5';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.21%2B9_openj9-0.41.0/ibm-semeru-open-jre_ppc64le_linux_11.0.21_9_openj9-0.41.0.tar.gz';          ;;        amd64|x86_64)          ESUM='324f7e8d75490cc76d5cf6a46b43f50ec1206a97d49e1549d1c65f1583fc51d5';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.21%2B9_openj9-0.41.0/ibm-semeru-open-jre_x64_linux_11.0.21_9_openj9-0.41.0.tar.gz';          ;;        s390x)          ESUM='a061cc8b2df7d42333e1d3ddb90535b8b86f76bd04d5c481d677f8167394249f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.21%2B9_openj9-0.41.0/ibm-semeru-open-jre_s390x_linux_11.0.21_9_openj9-0.41.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 02 Dec 2023 07:26:03 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 07:26:03 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Sat, 02 Dec 2023 07:26:37 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Sat, 02 Dec 2023 12:22:33 GMT
USER root
# Wed, 13 Dec 2023 18:40:58 GMT
ARG LIBERTY_VERSION=24.0.0.1-beta
# Wed, 13 Dec 2023 18:40:58 GMT
ARG LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4
# Wed, 13 Dec 2023 18:40:58 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip
# Wed, 13 Dec 2023 18:40:58 GMT
ARG LIBERTY_BUILD_LABEL=cl231220231127-1901
# Wed, 13 Dec 2023 18:40:58 GMT
ARG OPENJ9_SCC=true
# Wed, 13 Dec 2023 18:40:58 GMT
ARG VERBOSE=false
# Wed, 13 Dec 2023 18:40:58 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Melissa Lee, Thomas Watson, Michal Broz, Wendy Raschke org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl231220231127-1901 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with IBM Semeru Runtime Open Edition OpenJDK 17 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=24.0.0.1-beta
# Wed, 13 Dec 2023 18:40:58 GMT
COPY file:b2d50545eedb1d5c43e3914a49059b907fd99eab5d731eb6d4ff519f47d88408 in /opt/ol/NOTICES 
# Wed, 13 Dec 2023 18:40:59 GMT
COPY dir:3a03be0df9fe59a90276be087434855a86a8818483ded6f49c3c57610fb6842d in /opt/ol/helpers 
# Wed, 13 Dec 2023 18:40:59 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 13 Dec 2023 18:41:00 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl231220231127-1901 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4 LIBERTY_VERSION=24.0.0.1-beta OPENJ9_SCC=true VERBOSE=false
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_aarch64';          DUMB_INIT_SHA256=b7d648f97154a99c539b63c55979cd29f005f88430fb383007fe3458340b795e;          ;;        amd64|x86_64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_x86_64';          DUMB_INIT_SHA256=e874b55f3279ca41415d290c512a7ba9d08f98041b28ae7c2acb19a545f1c4df;          ;;        ppc64el|ppc64le)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_ppc64le';          DUMB_INIT_SHA256=3d15e80e29f0f4fa1fc686b00613a2220bc37e83a35283d4b4cca1fbd0a5609f;          ;;        s390x)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_s390x';          DUMB_INIT_SHA256=47e4601b152fc6dcb1891e66c30ecc62a2939fd7ffd1515a7c30f281cfec53b7;          ;;       *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /usr/bin/dumb-init ${DUMB_INIT_URL};     echo "${DUMB_INIT_SHA256} */usr/bin/dumb-init" | sha256sum -c -;     chmod +x /usr/bin/dumb-init;
# Wed, 13 Dec 2023 18:41:13 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl231220231127-1901 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4 LIBERTY_VERSION=24.0.0.1-beta OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && cp /opt/ol/wlp/LICENSE /licenses/     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 13 Dec 2023 18:41:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ol/wlp/bin:/opt/ol/helpers/build LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 13 Dec 2023 18:41:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl231220231127-1901 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4 LIBERTY_VERSION=24.0.0.1-beta VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea     && rm -rf /opt/ol/wlp/usr/servers/defaultServer/server.env
# Wed, 13 Dec 2023 18:41:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl231220231127-1901 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4 LIBERTY_VERSION=24.0.0.1-beta VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && ln -s /opt/ol/fixes /fixes     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 13 Dec 2023 18:41:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl231220231127-1901 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4 LIBERTY_VERSION=24.0.0.1-beta VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 13 Dec 2023 18:41:44 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 13 Dec 2023 18:41:44 GMT
USER 1001
# Wed, 13 Dec 2023 18:41:44 GMT
EXPOSE 9080 9443
# Wed, 13 Dec 2023 18:41:44 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 13 Dec 2023 18:41:45 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95c7df977cc051774d451b6622a7dec0910ee80283f12ed6e3d66e2fa624c39`  
		Last Modified: Sat, 02 Dec 2023 07:34:00 GMT  
		Size: 12.1 MB (12113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c53257c7c145a7192dc9b365d035d7268becfa6c0da9cc5ffb4fbe4e50c85e8`  
		Last Modified: Sat, 02 Dec 2023 07:35:40 GMT  
		Size: 47.7 MB (47739547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d03b16c57ab76a1a0c37303d6da6a9ecf734203050cd91b245b951b55114a1`  
		Last Modified: Sat, 02 Dec 2023 07:35:36 GMT  
		Size: 4.0 MB (4047424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1395378a0d71fae766c5aa3de900c1e45e688b357342ad25beae754b18b588a8`  
		Last Modified: Wed, 13 Dec 2023 18:48:23 GMT  
		Size: 1.1 KB (1073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f3a50f1dc87a052e9ab84009feb9e5b543829b504256f16401dc4ac21efedf`  
		Last Modified: Wed, 13 Dec 2023 18:48:22 GMT  
		Size: 9.6 KB (9581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb7b318450d895de8277add4ab8d0989d8851f4b36aedf3d777e5692497fb48`  
		Last Modified: Wed, 13 Dec 2023 18:48:22 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d9e435ba53370470ce1f3da139738ad3ceb106e548bc77ddaf2e1130141006`  
		Last Modified: Wed, 13 Dec 2023 18:48:20 GMT  
		Size: 42.3 KB (42317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b989523f38778a4fd81b2e7b2d8fa74d0a7dc0ee0939b9c0bc9133efac483a34`  
		Last Modified: Wed, 13 Dec 2023 18:48:33 GMT  
		Size: 330.6 MB (330614563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39481abd7d3b717271ea9aed99b406bccda97e3e2405584fbb975b3b1a46178`  
		Last Modified: Wed, 13 Dec 2023 18:48:20 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd00618322c19bc8fedcf173bd6b50b3c08ef69419e1ad19b56dea33b5afc67`  
		Last Modified: Wed, 13 Dec 2023 18:48:20 GMT  
		Size: 11.0 KB (11048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98affd0af85faf7d9a0e3d0bbffe38ca89280eb385340d20396907de2f0a0027`  
		Last Modified: Wed, 13 Dec 2023 18:48:22 GMT  
		Size: 12.4 MB (12438027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:beta-java11` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:1b05e4255136a92a057771e3375ef292163270243866bcdaa29f1122d56e9108
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **443.6 MB (443627927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4624c09dab9f38715dd67dbcbe62c10453c098da0138119380ac01ba75df4789`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 12 Dec 2023 11:43:51 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:43:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:43:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:43:52 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:43:55 GMT
ADD file:bda128b553d54e39b55daceea1f0ad351c73f83835bbf65d10e5af879ce6fee7 in / 
# Tue, 12 Dec 2023 11:43:56 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 10:56:27 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Dec 2023 10:56:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:00:44 GMT
ENV JAVA_VERSION=jdk-11.0.21+9_openj9-0.41.0
# Sat, 16 Dec 2023 11:02:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='5eb5d5d6006e1066b5c72d3b000f1c8fda572fa64189af103ef1176235cd3174';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.21%2B9_openj9-0.41.0/ibm-semeru-open-jre_aarch64_linux_11.0.21_9_openj9-0.41.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='0495d4d122dfb7ae160d9c76549f62fdd77b9c8ceddc9d4aced882c3c5157ba5';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.21%2B9_openj9-0.41.0/ibm-semeru-open-jre_ppc64le_linux_11.0.21_9_openj9-0.41.0.tar.gz';          ;;        amd64|x86_64)          ESUM='324f7e8d75490cc76d5cf6a46b43f50ec1206a97d49e1549d1c65f1583fc51d5';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.21%2B9_openj9-0.41.0/ibm-semeru-open-jre_x64_linux_11.0.21_9_openj9-0.41.0.tar.gz';          ;;        s390x)          ESUM='a061cc8b2df7d42333e1d3ddb90535b8b86f76bd04d5c481d677f8167394249f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.21%2B9_openj9-0.41.0/ibm-semeru-open-jre_s390x_linux_11.0.21_9_openj9-0.41.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 16 Dec 2023 11:02:45 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 Dec 2023 11:02:45 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Sat, 16 Dec 2023 11:03:21 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Sat, 16 Dec 2023 13:58:57 GMT
USER root
# Sat, 16 Dec 2023 15:13:20 GMT
ARG LIBERTY_VERSION=24.0.0.1-beta
# Sat, 16 Dec 2023 15:13:21 GMT
ARG LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4
# Sat, 16 Dec 2023 15:13:21 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip
# Sat, 16 Dec 2023 15:13:22 GMT
ARG LIBERTY_BUILD_LABEL=cl231220231127-1901
# Sat, 16 Dec 2023 15:13:22 GMT
ARG OPENJ9_SCC=true
# Sat, 16 Dec 2023 15:13:22 GMT
ARG VERBOSE=false
# Sat, 16 Dec 2023 15:13:22 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Melissa Lee, Thomas Watson, Michal Broz, Wendy Raschke org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl231220231127-1901 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with IBM Semeru Runtime Open Edition OpenJDK 17 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=24.0.0.1-beta
# Sat, 16 Dec 2023 15:13:23 GMT
COPY file:b2d50545eedb1d5c43e3914a49059b907fd99eab5d731eb6d4ff519f47d88408 in /opt/ol/NOTICES 
# Sat, 16 Dec 2023 15:13:23 GMT
COPY dir:3a03be0df9fe59a90276be087434855a86a8818483ded6f49c3c57610fb6842d in /opt/ol/helpers 
# Sat, 16 Dec 2023 15:13:23 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sat, 16 Dec 2023 15:13:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl231220231127-1901 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4 LIBERTY_VERSION=24.0.0.1-beta OPENJ9_SCC=true VERBOSE=false
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_aarch64';          DUMB_INIT_SHA256=b7d648f97154a99c539b63c55979cd29f005f88430fb383007fe3458340b795e;          ;;        amd64|x86_64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_x86_64';          DUMB_INIT_SHA256=e874b55f3279ca41415d290c512a7ba9d08f98041b28ae7c2acb19a545f1c4df;          ;;        ppc64el|ppc64le)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_ppc64le';          DUMB_INIT_SHA256=3d15e80e29f0f4fa1fc686b00613a2220bc37e83a35283d4b4cca1fbd0a5609f;          ;;        s390x)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_s390x';          DUMB_INIT_SHA256=47e4601b152fc6dcb1891e66c30ecc62a2939fd7ffd1515a7c30f281cfec53b7;          ;;       *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /usr/bin/dumb-init ${DUMB_INIT_URL};     echo "${DUMB_INIT_SHA256} */usr/bin/dumb-init" | sha256sum -c -;     chmod +x /usr/bin/dumb-init;
# Sat, 16 Dec 2023 15:13:47 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl231220231127-1901 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4 LIBERTY_VERSION=24.0.0.1-beta OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && cp /opt/ol/wlp/LICENSE /licenses/     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sat, 16 Dec 2023 15:13:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ol/wlp/bin:/opt/ol/helpers/build LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sat, 16 Dec 2023 15:13:53 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl231220231127-1901 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4 LIBERTY_VERSION=24.0.0.1-beta VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea     && rm -rf /opt/ol/wlp/usr/servers/defaultServer/server.env
# Sat, 16 Dec 2023 15:13:55 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl231220231127-1901 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4 LIBERTY_VERSION=24.0.0.1-beta VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && ln -s /opt/ol/fixes /fixes     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sat, 16 Dec 2023 15:14:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl231220231127-1901 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4 LIBERTY_VERSION=24.0.0.1-beta VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sat, 16 Dec 2023 15:14:30 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Sat, 16 Dec 2023 15:14:31 GMT
USER 1001
# Sat, 16 Dec 2023 15:14:31 GMT
EXPOSE 9080 9443
# Sat, 16 Dec 2023 15:14:31 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sat, 16 Dec 2023 15:14:31 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:7775720178c79208fc0d1b977c06891ef7230f39bc02e948d233c49f8a202fcf`  
		Last Modified: Sat, 16 Dec 2023 10:35:18 GMT  
		Size: 35.7 MB (35655287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbc811dfc8395d193589d30acb2a8cb783934cad69ab06a1989b2d9c01af4c8`  
		Last Modified: Sat, 16 Dec 2023 11:12:30 GMT  
		Size: 12.9 MB (12892026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc557220eba109df7a2a9e9ddc490e0b5675871b6a30e6e13e637418da616003`  
		Last Modified: Sat, 16 Dec 2023 11:14:42 GMT  
		Size: 49.7 MB (49705297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ebe2fae29638d65c115278003011a2dc9f912fae118d12b90a2d5aaca8a909d`  
		Last Modified: Sat, 16 Dec 2023 11:14:35 GMT  
		Size: 3.3 MB (3343897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18899a0e97c27599792c4d405022276092fd304278f12b57a0017b3467163572`  
		Last Modified: Sat, 16 Dec 2023 15:28:36 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac78c5cd6003f293e21dbd6be853fed8a6efc8ddfc0d99615a7fd61aff2ab33`  
		Last Modified: Sat, 16 Dec 2023 15:28:36 GMT  
		Size: 9.6 KB (9585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe933b5bfe22d7129e51ec4f362e1f63f65543ee8e2eb068ab52d894eb9309e`  
		Last Modified: Sat, 16 Dec 2023 15:28:36 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5987ad7c2bc2ab48377952f178648850f04b03a1339a99950d70285bf2acb324`  
		Last Modified: Sat, 16 Dec 2023 15:28:34 GMT  
		Size: 36.5 KB (36495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee260784caa47f56b3590bfbefef17378cfe49cb8c22183fc909f9c0025ffed6`  
		Last Modified: Sat, 16 Dec 2023 15:28:51 GMT  
		Size: 330.6 MB (330613912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a6f1d3ca8fa97db6ddc05e3232365348996e1f864692cd740c74170670f41c`  
		Last Modified: Sat, 16 Dec 2023 15:28:34 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4a490c7c3a04e395cb93557b1912863f1ea6807e00fda2267208e8f0dbccaf`  
		Last Modified: Sat, 16 Dec 2023 15:28:33 GMT  
		Size: 11.0 KB (11040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddc8d3cf647595aa789ecda68af198d2634941be4d0e6bdc7b98f06dd4d179b`  
		Last Modified: Sat, 16 Dec 2023 15:28:35 GMT  
		Size: 11.4 MB (11357860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:beta-java11` - linux; s390x

```console
$ docker pull open-liberty@sha256:1a168fb974a24ff0e3c686017be6b78a4224d54b62930267bfbb0424d839eaff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.2 MB (437185339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:134647b1e2270033c7bbe27a50463026b070f41cf041a4a97c63afaba9aa2f54`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 12 Dec 2023 11:44:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:44:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:44:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:44:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:44:59 GMT
ADD file:1729e720d10023da7d783040cefa8f30d3c61772a5e1ae577182a1fcba69aff1 in / 
# Tue, 12 Dec 2023 11:44:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 07:56:35 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Dec 2023 07:56:45 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 08:00:40 GMT
ENV JAVA_VERSION=jdk-11.0.21+9_openj9-0.41.0
# Sat, 16 Dec 2023 08:02:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='5eb5d5d6006e1066b5c72d3b000f1c8fda572fa64189af103ef1176235cd3174';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.21%2B9_openj9-0.41.0/ibm-semeru-open-jre_aarch64_linux_11.0.21_9_openj9-0.41.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='0495d4d122dfb7ae160d9c76549f62fdd77b9c8ceddc9d4aced882c3c5157ba5';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.21%2B9_openj9-0.41.0/ibm-semeru-open-jre_ppc64le_linux_11.0.21_9_openj9-0.41.0.tar.gz';          ;;        amd64|x86_64)          ESUM='324f7e8d75490cc76d5cf6a46b43f50ec1206a97d49e1549d1c65f1583fc51d5';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.21%2B9_openj9-0.41.0/ibm-semeru-open-jre_x64_linux_11.0.21_9_openj9-0.41.0.tar.gz';          ;;        s390x)          ESUM='a061cc8b2df7d42333e1d3ddb90535b8b86f76bd04d5c481d677f8167394249f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.21%2B9_openj9-0.41.0/ibm-semeru-open-jre_s390x_linux_11.0.21_9_openj9-0.41.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 16 Dec 2023 08:03:04 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 Dec 2023 08:03:05 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Sat, 16 Dec 2023 08:03:40 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Sat, 16 Dec 2023 09:37:23 GMT
USER root
# Sat, 16 Dec 2023 10:41:01 GMT
ARG LIBERTY_VERSION=24.0.0.1-beta
# Sat, 16 Dec 2023 10:41:01 GMT
ARG LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4
# Sat, 16 Dec 2023 10:41:01 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip
# Sat, 16 Dec 2023 10:41:01 GMT
ARG LIBERTY_BUILD_LABEL=cl231220231127-1901
# Sat, 16 Dec 2023 10:41:01 GMT
ARG OPENJ9_SCC=true
# Sat, 16 Dec 2023 10:41:01 GMT
ARG VERBOSE=false
# Sat, 16 Dec 2023 10:41:02 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Melissa Lee, Thomas Watson, Michal Broz, Wendy Raschke org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl231220231127-1901 org.opencontainers.image.description=This image contains the Open Liberty beta runtime with IBM Semeru Runtime Open Edition OpenJDK 17 with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty Beta org.opencontainers.image.version=24.0.0.1-beta
# Sat, 16 Dec 2023 10:41:02 GMT
COPY file:b2d50545eedb1d5c43e3914a49059b907fd99eab5d731eb6d4ff519f47d88408 in /opt/ol/NOTICES 
# Sat, 16 Dec 2023 10:41:02 GMT
COPY dir:3a03be0df9fe59a90276be087434855a86a8818483ded6f49c3c57610fb6842d in /opt/ol/helpers 
# Sat, 16 Dec 2023 10:41:02 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sat, 16 Dec 2023 10:41:03 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl231220231127-1901 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4 LIBERTY_VERSION=24.0.0.1-beta OPENJ9_SCC=true VERBOSE=false
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_aarch64';          DUMB_INIT_SHA256=b7d648f97154a99c539b63c55979cd29f005f88430fb383007fe3458340b795e;          ;;        amd64|x86_64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_x86_64';          DUMB_INIT_SHA256=e874b55f3279ca41415d290c512a7ba9d08f98041b28ae7c2acb19a545f1c4df;          ;;        ppc64el|ppc64le)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_ppc64le';          DUMB_INIT_SHA256=3d15e80e29f0f4fa1fc686b00613a2220bc37e83a35283d4b4cca1fbd0a5609f;          ;;        s390x)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_s390x';          DUMB_INIT_SHA256=47e4601b152fc6dcb1891e66c30ecc62a2939fd7ffd1515a7c30f281cfec53b7;          ;;       *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /usr/bin/dumb-init ${DUMB_INIT_URL};     echo "${DUMB_INIT_SHA256} */usr/bin/dumb-init" | sha256sum -c -;     chmod +x /usr/bin/dumb-init;
# Sat, 16 Dec 2023 10:41:22 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl231220231127-1901 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4 LIBERTY_VERSION=24.0.0.1-beta OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && mkdir -p /licenses     && cp /opt/ol/wlp/LICENSE /licenses/     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sat, 16 Dec 2023 10:41:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ol/wlp/bin:/opt/ol/helpers/build LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sat, 16 Dec 2023 10:41:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl231220231127-1901 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4 LIBERTY_VERSION=24.0.0.1-beta VERBOSE=false
RUN /opt/ol/wlp/bin/server create --template=javaee8     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea     && rm -rf /opt/ol/wlp/usr/servers/defaultServer/server.env
# Sat, 16 Dec 2023 10:41:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl231220231127-1901 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4 LIBERTY_VERSION=24.0.0.1-beta VERBOSE=false
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && mkdir -p /config/dropins     && mkdir -p /config/apps     && ln -s /opt/ol/wlp /liberty     && ln -s /opt/ol/fixes /fixes     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sat, 16 Dec 2023 10:41:56 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl231220231127-1901 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/beta/openliberty-runtime/24.0.0.1-beta/openliberty-runtime-24.0.0.1-beta.zip LIBERTY_SHA=79485f9280899431406d1be4eb60dbc3a1b522a4 LIBERTY_VERSION=24.0.0.1-beta VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sat, 16 Dec 2023 10:41:57 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Sat, 16 Dec 2023 10:41:57 GMT
USER 1001
# Sat, 16 Dec 2023 10:41:57 GMT
EXPOSE 9080 9443
# Sat, 16 Dec 2023 10:41:57 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sat, 16 Dec 2023 10:41:57 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:6949655473f9a6801351bc2ee9bef80a58f5ac2dd31547e0d4f473c53d282400`  
		Last Modified: Sat, 16 Dec 2023 07:42:42 GMT  
		Size: 28.7 MB (28654553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faadb4f032ac796bbd76d4fbd3ea1c6a3984cb437adc9d463772f3453f9e0a54`  
		Last Modified: Sat, 16 Dec 2023 08:13:40 GMT  
		Size: 12.2 MB (12199927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155920ed46a90be2a260af6a4006105527a0ac4ab0e87bc8f92549c6c319cd9b`  
		Last Modified: Sat, 16 Dec 2023 08:15:17 GMT  
		Size: 48.2 MB (48240661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f9751e6993cc7a8a77503fb46e5bf638b95c77027fa81e17cc46cc2a2a3007`  
		Last Modified: Sat, 16 Dec 2023 08:15:11 GMT  
		Size: 4.4 MB (4418820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ac54a2d751f730126947b8c2236f5854e2eefd96ba02dbd8706931abbe26f8`  
		Last Modified: Sat, 16 Dec 2023 10:53:22 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0551a90bbff329c1571d6efa3e26afef87f07d157305eda27fbdb128395ae0d`  
		Last Modified: Sat, 16 Dec 2023 10:53:22 GMT  
		Size: 9.6 KB (9582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d89b5212399e3487eaa7124aee44bb2dd2dfd35e53a258770e36d9beb1fd436`  
		Last Modified: Sat, 16 Dec 2023 10:53:22 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282030b026c402795315d71990c3c0a97a3f522e65cedbc90071167a40e19835`  
		Last Modified: Sat, 16 Dec 2023 10:53:21 GMT  
		Size: 33.1 KB (33113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c55c588aa88c2949ec9d1d4f38d24f9a6e92289b99f3169a4dd62250fbe4bf`  
		Last Modified: Sat, 16 Dec 2023 10:53:34 GMT  
		Size: 330.6 MB (330613474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117329d9f61f71ca72c148e3b41fd1fb42deaac9b55b386b6b9e7709391b6d17`  
		Last Modified: Sat, 16 Dec 2023 10:53:21 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6e8250d791ff278cd1184d4cb3291f6eaf36a538437a598ed1197e363df697`  
		Last Modified: Sat, 16 Dec 2023 10:53:21 GMT  
		Size: 11.0 KB (11039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132fe2063b66ddfb8002c0e95ae6f9526cf606b963cf3717f82e332a83a7cd3e`  
		Last Modified: Sat, 16 Dec 2023 10:53:22 GMT  
		Size: 13.0 MB (13001636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
