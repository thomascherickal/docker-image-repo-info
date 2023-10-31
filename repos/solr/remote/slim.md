## `solr:slim`

```console
$ docker pull solr@sha256:aa5af0dc8e4d037ca8f555f268fff717e7c50aff79425cf2f975eebe7da89490
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `solr:slim` - linux; amd64

```console
$ docker pull solr@sha256:7bef3f01e97c82fb0f17eafe8f84a4692756ca4fdd2abf2a78f45923ede79740
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.0 MB (160970985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76fb4167a9ede03418829a4474ff4fcad420df1479a2c5dd2a1283d696a4dd1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 05:51:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 05:51:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 05:51:05 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 13 Oct 2023 05:53:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 05:53:53 GMT
ENV JAVA_VERSION=jdk-17.0.8.1+1
# Fri, 13 Oct 2023 05:54:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0a1c5c9ee9d20832c87bd1e99a4c4a96947b59bb35c72683fe895d705f202737';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        armhf|arm)          ESUM='8af898c5d356f0b2cee2db67ff9c8e7a8e738c0f6b3a61c383150b3168b9ea58';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jre_arm_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='4aadc18e58d20c37c69cf6ec2cc3299b76f5b21073fc8e6101e11268d7a33b5b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='5eff8141fd282b3473fd649e04c113ba044cf19f0c513b951b700c28a81c1d6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jre_s390x_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ab68857594792474a3049ede09ea1178e42df29803a6a41be771794f571b2d4e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jre_x64_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 13 Oct 2023 05:54:29 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 13 Oct 2023 05:54:29 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Fri, 13 Oct 2023 05:54:29 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 17 Oct 2023 01:39:56 GMT
ARG SOLR_VERSION=9.4.0
# Tue, 17 Oct 2023 01:40:37 GMT
ARG SOLR_DIST=-slim
# Tue, 17 Oct 2023 01:40:37 GMT
ARG SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a
# Tue, 17 Oct 2023 01:40:37 GMT
ARG SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E
# Tue, 17 Oct 2023 01:40:37 GMT
ARG SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr
# Tue, 17 Oct 2023 01:40:48 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;   apt-get update;   apt-get -y --no-install-recommends install wget gpg gnupg dirmngr;   rm -rf /var/lib/apt/lists/*;   export SOLR_BINARY="solr-$SOLR_VERSION$SOLR_DIST.tgz";   MAX_REDIRECTS=3;   case "${SOLR_DOWNLOAD_SERVER}" in     (*"apache.org"*);;     (*)       MAX_REDIRECTS=4 &&       SKIP_GPG_CHECK=true;;   esac;   export DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/$SOLR_BINARY";   echo "downloading $DOWNLOAD_URL";   if ! wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$DOWNLOAD_URL" -O "/opt/$SOLR_BINARY"; then rm -f "/opt/$SOLR_BINARY"; fi;   if [ ! -f "/opt/$SOLR_BINARY" ]; then echo "failed download attempt for $SOLR_BINARY"; exit 1; fi;   echo "$SOLR_SHA512 */opt/$SOLR_BINARY" | sha512sum -c -;   if [ -z "$SKIP_GPG_CHECK" ]; then     export GNUPGHOME="/tmp/gnupg_home";     mkdir -p "$GNUPGHOME";     chmod 700 "$GNUPGHOME";     echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";     if [ -n "$SOLR_KEYS" ]; then       wget -nv "https://downloads.apache.org/solr/KEYS" -O- |         gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';       release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";       rm -rf "$GNUPGHOME"/*;       echo "${release_keys}" | gpg --batch --import;     fi;     echo "downloading $DOWNLOAD_URL.asc";     wget -nv "$DOWNLOAD_URL.asc" -O "/opt/$SOLR_BINARY.asc";     (>&2 ls -l "/opt/$SOLR_BINARY" "/opt/$SOLR_BINARY.asc");     gpg --batch --verify "/opt/$SOLR_BINARY.asc" "/opt/$SOLR_BINARY";     { command -v gpgconf; gpgconf --kill all || :; };     rm -r "$GNUPGHOME";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --preserve-permissions --file "/opt/$SOLR_BINARY";   rm "/opt/$SOLR_BINARY"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Tue, 17 Oct 2023 01:40:49 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Tue, 17 Oct 2023 01:40:49 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Tue, 17 Oct 2023 01:40:49 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Tue, 17 Oct 2023 01:40:49 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Tue, 17 Oct 2023 01:40:49 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Tue, 17 Oct 2023 01:40:49 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Tue, 17 Oct 2023 01:40:49 GMT
LABEL org.opencontainers.image.version=9.4.0
# Tue, 17 Oct 2023 01:40:49 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 17 Oct 2023 01:40:49 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0 SOLR_ZK_EMBEDDED_HOST=0.0.0.0
# Tue, 17 Oct 2023 01:40:50 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 17 Oct 2023 01:40:50 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Tue, 17 Oct 2023 01:40:51 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   test ! -e /opt/solr/modules || ln -s /opt/solr/modules /opt/solr/contrib;   test ! -e /opt/solr/prometheus-exporter || ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Tue, 17 Oct 2023 01:40:55 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;     apt-get update;     apt-get -y --no-install-recommends install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Tue, 17 Oct 2023 01:40:55 GMT
VOLUME [/var/solr]
# Tue, 17 Oct 2023 01:40:56 GMT
EXPOSE 8983
# Tue, 17 Oct 2023 01:40:56 GMT
WORKDIR /opt/solr
# Tue, 17 Oct 2023 01:40:56 GMT
USER 8983
# Tue, 17 Oct 2023 01:40:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Oct 2023 01:40:56 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50431c77a77b7f46c78e4929a36d42dcb3551c22e0404d2bee6e8a15cc650640`  
		Last Modified: Fri, 13 Oct 2023 05:59:21 GMT  
		Size: 17.5 MB (17454843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd8e860e67230bfef1a2f42f986d22713cfc307559996493f6aac0f0bfc32c8`  
		Last Modified: Fri, 13 Oct 2023 06:00:06 GMT  
		Size: 47.2 MB (47209787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637e2db99ae6d5d22792dba960463b31fc445d5be9e3383fef9f0be96900a680`  
		Last Modified: Fri, 13 Oct 2023 05:59:59 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de1c2853278b16ef01c0abfa4065794c145daefc507cb6cb6fb56a1803a58bb`  
		Last Modified: Fri, 13 Oct 2023 05:59:59 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cebd247ed4b183e803c8a68923e19ce5ded4213dce8c31e0b7af7dc8d877d8d`  
		Last Modified: Tue, 17 Oct 2023 01:42:08 GMT  
		Size: 64.0 MB (64022405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8172615e73d84dd92aec94bf4d59fc7681c764bfe5bd6364dc214213f50b7b2d`  
		Last Modified: Tue, 17 Oct 2023 01:42:04 GMT  
		Size: 4.3 KB (4297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26756abab1474ebcd4dc316d3a23b2c003a4f666e6712205c90c0b969af05d64`  
		Last Modified: Tue, 17 Oct 2023 01:42:04 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf0757d8cf2246544911800dbd077616a6859dfe5443bd01b3950c5df76e0d5`  
		Last Modified: Tue, 17 Oct 2023 01:42:04 GMT  
		Size: 10.8 KB (10751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c8eb78c3ce29686f32d317c90fec1070af8ce19e7a7f5418c0cd4c7d8ed010`  
		Last Modified: Tue, 17 Oct 2023 01:42:04 GMT  
		Size: 1.8 MB (1828674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:slim` - linux; arm variant v7

```console
$ docker pull solr@sha256:ca3f7131a8e6e7a8e9a96f63d6022e3aa21ecc226cfa6a24c064d9f2140b899f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155581106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cd9bfafa1896f78b060b0c228e5577bca822e78d4e7061d94387db3b12f8c60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:56 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:35:01 GMT
ADD file:4b9d52f97ed5796b14772a84c1e7213402430d32312d15ae04a2dcc9fc485a52 in / 
# Thu, 05 Oct 2023 07:35:02 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 01:15:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 01:15:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 01:15:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 30 Oct 2023 23:01:12 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 30 Oct 2023 23:01:12 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Mon, 30 Oct 2023 23:01:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 30 Oct 2023 23:01:43 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:01:43 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:01:43 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 31 Oct 2023 00:44:39 GMT
ARG SOLR_VERSION=9.4.0
# Tue, 31 Oct 2023 00:45:37 GMT
ARG SOLR_DIST=-slim
# Tue, 31 Oct 2023 00:45:37 GMT
ARG SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a
# Tue, 31 Oct 2023 00:45:37 GMT
ARG SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E
# Tue, 31 Oct 2023 00:45:37 GMT
ARG SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr
# Tue, 31 Oct 2023 00:45:52 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;   apt-get update;   apt-get -y --no-install-recommends install wget gpg gnupg dirmngr;   rm -rf /var/lib/apt/lists/*;   export SOLR_BINARY="solr-$SOLR_VERSION$SOLR_DIST.tgz";   MAX_REDIRECTS=3;   case "${SOLR_DOWNLOAD_SERVER}" in     (*"apache.org"*);;     (*)       MAX_REDIRECTS=4 &&       SKIP_GPG_CHECK=true;;   esac;   export DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/$SOLR_BINARY";   echo "downloading $DOWNLOAD_URL";   if ! wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$DOWNLOAD_URL" -O "/opt/$SOLR_BINARY"; then rm -f "/opt/$SOLR_BINARY"; fi;   if [ ! -f "/opt/$SOLR_BINARY" ]; then echo "failed download attempt for $SOLR_BINARY"; exit 1; fi;   echo "$SOLR_SHA512 */opt/$SOLR_BINARY" | sha512sum -c -;   if [ -z "$SKIP_GPG_CHECK" ]; then     export GNUPGHOME="/tmp/gnupg_home";     mkdir -p "$GNUPGHOME";     chmod 700 "$GNUPGHOME";     echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";     if [ -n "$SOLR_KEYS" ]; then       wget -nv "https://downloads.apache.org/solr/KEYS" -O- |         gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';       release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";       rm -rf "$GNUPGHOME"/*;       echo "${release_keys}" | gpg --batch --import;     fi;     echo "downloading $DOWNLOAD_URL.asc";     wget -nv "$DOWNLOAD_URL.asc" -O "/opt/$SOLR_BINARY.asc";     (>&2 ls -l "/opt/$SOLR_BINARY" "/opt/$SOLR_BINARY.asc");     gpg --batch --verify "/opt/$SOLR_BINARY.asc" "/opt/$SOLR_BINARY";     { command -v gpgconf; gpgconf --kill all || :; };     rm -r "$GNUPGHOME";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --preserve-permissions --file "/opt/$SOLR_BINARY";   rm "/opt/$SOLR_BINARY"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Tue, 31 Oct 2023 00:45:53 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Tue, 31 Oct 2023 00:45:53 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Tue, 31 Oct 2023 00:45:53 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Tue, 31 Oct 2023 00:45:53 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Tue, 31 Oct 2023 00:45:53 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Tue, 31 Oct 2023 00:45:53 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Tue, 31 Oct 2023 00:45:53 GMT
LABEL org.opencontainers.image.version=9.4.0
# Tue, 31 Oct 2023 00:45:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 31 Oct 2023 00:45:53 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0 SOLR_ZK_EMBEDDED_HOST=0.0.0.0
# Tue, 31 Oct 2023 00:45:54 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 31 Oct 2023 00:45:54 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Tue, 31 Oct 2023 00:45:55 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   test ! -e /opt/solr/modules || ln -s /opt/solr/modules /opt/solr/contrib;   test ! -e /opt/solr/prometheus-exporter || ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Tue, 31 Oct 2023 00:45:59 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;     apt-get update;     apt-get -y --no-install-recommends install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Tue, 31 Oct 2023 00:46:00 GMT
VOLUME [/var/solr]
# Tue, 31 Oct 2023 00:46:00 GMT
EXPOSE 8983
# Tue, 31 Oct 2023 00:46:00 GMT
WORKDIR /opt/solr
# Tue, 31 Oct 2023 00:46:00 GMT
USER 8983
# Tue, 31 Oct 2023 00:46:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Oct 2023 00:46:00 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:c4f28c22de51200ba6a71d2274daa2f71735946524265b3c45752d2cec53dee0`  
		Last Modified: Fri, 06 Oct 2023 02:02:33 GMT  
		Size: 27.5 MB (27513969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce5de55a5083371ea9acd5e9e4a92410bf534c9db006abc1006968e5a9117c9`  
		Last Modified: Mon, 30 Oct 2023 23:04:23 GMT  
		Size: 17.6 MB (17586150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8907f1de52d231e3b798196965ed39e0756ab6301bd9aca54036adfdeada2d6`  
		Last Modified: Mon, 30 Oct 2023 23:05:09 GMT  
		Size: 44.8 MB (44786987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3e20fda5a616714fca45d81cd97a30a96d84c7625808fa6a15f34499d6bcda`  
		Last Modified: Mon, 30 Oct 2023 23:05:02 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030f61d8dd14b738dc95a1ce8dc01993ff0cc2d78956151efba88cfac2a4aa3a`  
		Last Modified: Mon, 30 Oct 2023 23:05:02 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:021f64987e035a6e019b752e6aa0dedcff80f7f33f557235dfae8fd004e059c4`  
		Last Modified: Tue, 31 Oct 2023 00:53:05 GMT  
		Size: 64.0 MB (64023422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d05f55b3debd9c08716da0f4ff7037134c5c3e7767be2c40ef49dcbb78ae90c`  
		Last Modified: Tue, 31 Oct 2023 00:53:00 GMT  
		Size: 4.2 KB (4224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a438f0cd6cc1e81dfef87501d7000d435366acdab5f295afe6e612571dd07f`  
		Last Modified: Tue, 31 Oct 2023 00:53:00 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c6ff992efdbee1a1703cf622dbfaa56c2511f048c362329111ff39eddba2245`  
		Last Modified: Tue, 31 Oct 2023 00:53:00 GMT  
		Size: 10.8 KB (10758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98762fed7e8edc7a355f6a0cea29e4b07534362eb45768badd40d26cd9a3cac1`  
		Last Modified: Tue, 31 Oct 2023 00:53:00 GMT  
		Size: 1.7 MB (1654481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:slim` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:43347e13b3ad625bc04d45cefc264cec5cccecc302b11270183e9e3252ee703c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.6 MB (159603416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff91918d5c36c1240e86cfa39c2dea39331749fe6e4c82d7bbad4465c5e48d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:46:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 02:46:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 02:46:31 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 30 Oct 2023 23:44:05 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 30 Oct 2023 23:44:05 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Mon, 30 Oct 2023 23:45:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 30 Oct 2023 23:45:35 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:45:35 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:45:35 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 31 Oct 2023 02:28:38 GMT
ARG SOLR_VERSION=9.4.0
# Tue, 31 Oct 2023 02:29:35 GMT
ARG SOLR_DIST=-slim
# Tue, 31 Oct 2023 02:29:35 GMT
ARG SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a
# Tue, 31 Oct 2023 02:29:35 GMT
ARG SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E
# Tue, 31 Oct 2023 02:29:36 GMT
ARG SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr
# Tue, 31 Oct 2023 02:29:49 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;   apt-get update;   apt-get -y --no-install-recommends install wget gpg gnupg dirmngr;   rm -rf /var/lib/apt/lists/*;   export SOLR_BINARY="solr-$SOLR_VERSION$SOLR_DIST.tgz";   MAX_REDIRECTS=3;   case "${SOLR_DOWNLOAD_SERVER}" in     (*"apache.org"*);;     (*)       MAX_REDIRECTS=4 &&       SKIP_GPG_CHECK=true;;   esac;   export DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/$SOLR_BINARY";   echo "downloading $DOWNLOAD_URL";   if ! wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$DOWNLOAD_URL" -O "/opt/$SOLR_BINARY"; then rm -f "/opt/$SOLR_BINARY"; fi;   if [ ! -f "/opt/$SOLR_BINARY" ]; then echo "failed download attempt for $SOLR_BINARY"; exit 1; fi;   echo "$SOLR_SHA512 */opt/$SOLR_BINARY" | sha512sum -c -;   if [ -z "$SKIP_GPG_CHECK" ]; then     export GNUPGHOME="/tmp/gnupg_home";     mkdir -p "$GNUPGHOME";     chmod 700 "$GNUPGHOME";     echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";     if [ -n "$SOLR_KEYS" ]; then       wget -nv "https://downloads.apache.org/solr/KEYS" -O- |         gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';       release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";       rm -rf "$GNUPGHOME"/*;       echo "${release_keys}" | gpg --batch --import;     fi;     echo "downloading $DOWNLOAD_URL.asc";     wget -nv "$DOWNLOAD_URL.asc" -O "/opt/$SOLR_BINARY.asc";     (>&2 ls -l "/opt/$SOLR_BINARY" "/opt/$SOLR_BINARY.asc");     gpg --batch --verify "/opt/$SOLR_BINARY.asc" "/opt/$SOLR_BINARY";     { command -v gpgconf; gpgconf --kill all || :; };     rm -r "$GNUPGHOME";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --preserve-permissions --file "/opt/$SOLR_BINARY";   rm "/opt/$SOLR_BINARY"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Tue, 31 Oct 2023 02:29:50 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Tue, 31 Oct 2023 02:29:50 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Tue, 31 Oct 2023 02:29:50 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Tue, 31 Oct 2023 02:29:50 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Tue, 31 Oct 2023 02:29:50 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Tue, 31 Oct 2023 02:29:50 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Tue, 31 Oct 2023 02:29:50 GMT
LABEL org.opencontainers.image.version=9.4.0
# Tue, 31 Oct 2023 02:29:50 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 31 Oct 2023 02:29:50 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0 SOLR_ZK_EMBEDDED_HOST=0.0.0.0
# Tue, 31 Oct 2023 02:29:51 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 31 Oct 2023 02:29:51 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Tue, 31 Oct 2023 02:29:52 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   test ! -e /opt/solr/modules || ln -s /opt/solr/modules /opt/solr/contrib;   test ! -e /opt/solr/prometheus-exporter || ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Tue, 31 Oct 2023 02:29:56 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;     apt-get update;     apt-get -y --no-install-recommends install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Tue, 31 Oct 2023 02:29:56 GMT
VOLUME [/var/solr]
# Tue, 31 Oct 2023 02:29:56 GMT
EXPOSE 8983
# Tue, 31 Oct 2023 02:29:56 GMT
WORKDIR /opt/solr
# Tue, 31 Oct 2023 02:29:56 GMT
USER 8983
# Tue, 31 Oct 2023 02:29:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Oct 2023 02:29:56 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f494a0917249ff640404cd9965fcd6a5ed5b7725fc21ff44518307f60c8e0a`  
		Last Modified: Mon, 30 Oct 2023 23:50:44 GMT  
		Size: 18.9 MB (18858788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf992ac9f7594e95247c785c373702afa5ebbf20db8b34fad80efa1ff3e0736`  
		Last Modified: Mon, 30 Oct 2023 23:52:03 GMT  
		Size: 46.6 MB (46623965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652d455f0a073aa4bc59de2e451f4c5a2ad6d6d9cb13538ef955d11e722e6c45`  
		Last Modified: Mon, 30 Oct 2023 23:51:58 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fce918b0b707b682534041104ace8701cb441f12b5ce2fb5e983bfe29694385`  
		Last Modified: Mon, 30 Oct 2023 23:51:58 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b1fc99d7127f28225b434b61c18076a3e86255e4883ca1bd06e9924a72661d`  
		Last Modified: Tue, 31 Oct 2023 02:40:11 GMT  
		Size: 64.0 MB (64023841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75b9e401271431278656fa980c2a3d660b22401e1714d878aa230b9e99d04ed`  
		Last Modified: Tue, 31 Oct 2023 02:40:08 GMT  
		Size: 4.3 KB (4328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10519a076e59cb4be780980141b2afec092a1dd7a20ce581ef2ceb564867420d`  
		Last Modified: Tue, 31 Oct 2023 02:40:08 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f329d422aedaa6c563d6e5e6e4444517a49f1b0d41e984642e1c2c6389c760a`  
		Last Modified: Tue, 31 Oct 2023 02:40:08 GMT  
		Size: 10.8 KB (10760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ed5c86b1a52b9351e4281b44b85cabb4834018262d535ae79858672904e0cf`  
		Last Modified: Tue, 31 Oct 2023 02:40:08 GMT  
		Size: 1.7 MB (1688680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:slim` - linux; ppc64le

```console
$ docker pull solr@sha256:95278ac3d6dbddaaafe86431e3ce7d82f3df8db24a8bc1c57ad09209b729d914
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.3 MB (167281636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cba7572799cc8ecddd4a7a796e1ae392ba693878fb177a449ec1101ff8dca5d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:18 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:34:22 GMT
ADD file:595ff761b2778bdc6bb59cbe8ce51c4a247e0f279ccd59a17b5be6cdeac0b4d2 in / 
# Thu, 05 Oct 2023 07:34:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 08:00:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 08:00:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 08:00:41 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 30 Oct 2023 23:24:27 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 30 Oct 2023 23:24:28 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Mon, 30 Oct 2023 23:26:48 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 30 Oct 2023 23:26:51 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:26:51 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:26:51 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 31 Oct 2023 00:58:25 GMT
ARG SOLR_VERSION=9.4.0
# Tue, 31 Oct 2023 00:59:35 GMT
ARG SOLR_DIST=-slim
# Tue, 31 Oct 2023 00:59:35 GMT
ARG SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a
# Tue, 31 Oct 2023 00:59:36 GMT
ARG SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E
# Tue, 31 Oct 2023 00:59:36 GMT
ARG SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr
# Tue, 31 Oct 2023 00:59:55 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;   apt-get update;   apt-get -y --no-install-recommends install wget gpg gnupg dirmngr;   rm -rf /var/lib/apt/lists/*;   export SOLR_BINARY="solr-$SOLR_VERSION$SOLR_DIST.tgz";   MAX_REDIRECTS=3;   case "${SOLR_DOWNLOAD_SERVER}" in     (*"apache.org"*);;     (*)       MAX_REDIRECTS=4 &&       SKIP_GPG_CHECK=true;;   esac;   export DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/$SOLR_BINARY";   echo "downloading $DOWNLOAD_URL";   if ! wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$DOWNLOAD_URL" -O "/opt/$SOLR_BINARY"; then rm -f "/opt/$SOLR_BINARY"; fi;   if [ ! -f "/opt/$SOLR_BINARY" ]; then echo "failed download attempt for $SOLR_BINARY"; exit 1; fi;   echo "$SOLR_SHA512 */opt/$SOLR_BINARY" | sha512sum -c -;   if [ -z "$SKIP_GPG_CHECK" ]; then     export GNUPGHOME="/tmp/gnupg_home";     mkdir -p "$GNUPGHOME";     chmod 700 "$GNUPGHOME";     echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";     if [ -n "$SOLR_KEYS" ]; then       wget -nv "https://downloads.apache.org/solr/KEYS" -O- |         gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';       release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";       rm -rf "$GNUPGHOME"/*;       echo "${release_keys}" | gpg --batch --import;     fi;     echo "downloading $DOWNLOAD_URL.asc";     wget -nv "$DOWNLOAD_URL.asc" -O "/opt/$SOLR_BINARY.asc";     (>&2 ls -l "/opt/$SOLR_BINARY" "/opt/$SOLR_BINARY.asc");     gpg --batch --verify "/opt/$SOLR_BINARY.asc" "/opt/$SOLR_BINARY";     { command -v gpgconf; gpgconf --kill all || :; };     rm -r "$GNUPGHOME";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --preserve-permissions --file "/opt/$SOLR_BINARY";   rm "/opt/$SOLR_BINARY"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Tue, 31 Oct 2023 00:59:56 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Tue, 31 Oct 2023 00:59:56 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Tue, 31 Oct 2023 00:59:56 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Tue, 31 Oct 2023 00:59:57 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Tue, 31 Oct 2023 00:59:57 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Tue, 31 Oct 2023 00:59:57 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Tue, 31 Oct 2023 00:59:57 GMT
LABEL org.opencontainers.image.version=9.4.0
# Tue, 31 Oct 2023 00:59:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 31 Oct 2023 00:59:58 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0 SOLR_ZK_EMBEDDED_HOST=0.0.0.0
# Tue, 31 Oct 2023 00:59:59 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 31 Oct 2023 01:00:00 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Tue, 31 Oct 2023 01:00:00 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   test ! -e /opt/solr/modules || ln -s /opt/solr/modules /opt/solr/contrib;   test ! -e /opt/solr/prometheus-exporter || ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Tue, 31 Oct 2023 01:00:07 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;     apt-get update;     apt-get -y --no-install-recommends install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Tue, 31 Oct 2023 01:00:08 GMT
VOLUME [/var/solr]
# Tue, 31 Oct 2023 01:00:08 GMT
EXPOSE 8983
# Tue, 31 Oct 2023 01:00:08 GMT
WORKDIR /opt/solr
# Tue, 31 Oct 2023 01:00:08 GMT
USER 8983
# Tue, 31 Oct 2023 01:00:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Oct 2023 01:00:09 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:589c4cce1daa100afadbdbeda96025d02f85c117e0e60b70801af41b4e618668`  
		Last Modified: Fri, 13 Oct 2023 06:13:20 GMT  
		Size: 35.7 MB (35682793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494f75987917a46354a891e88bff3d330d2cb87ae470f00c3e4eb11c59000dc4`  
		Last Modified: Mon, 30 Oct 2023 23:32:42 GMT  
		Size: 18.7 MB (18724494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb60edc6b5afb117807f9ca243d0ed6eefd19b8acac8aaf2198b45d56b64673d`  
		Last Modified: Mon, 30 Oct 2023 23:34:21 GMT  
		Size: 47.0 MB (46999759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daccf8f9f3100ea7991ff837336b7788150dd87ffdac0df550a359507a802d0f`  
		Last Modified: Mon, 30 Oct 2023 23:34:13 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a98aebb4d9dde64307227b7c51540281a085c9619c02bf335ff3265fd20468`  
		Last Modified: Mon, 30 Oct 2023 23:34:13 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda7e6c6d3cd579819df02dfd627ebb3306dcdc550f54573bc6a1d2991d76f3b`  
		Last Modified: Tue, 31 Oct 2023 01:09:40 GMT  
		Size: 64.0 MB (64023143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5470b7af568b3744fd5063f41da8f6f7effad933e7878984677bd842e08bb852`  
		Last Modified: Tue, 31 Oct 2023 01:09:35 GMT  
		Size: 4.3 KB (4297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047889b1129e2a83c7e6d97bc414495c45cbf7b80b9bb4d2c1a50b96298d28ed`  
		Last Modified: Tue, 31 Oct 2023 01:09:35 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759221206d8fdd2e4166ab758913f62b487d68476e6667653e54e7362328cfae`  
		Last Modified: Tue, 31 Oct 2023 01:09:35 GMT  
		Size: 10.8 KB (10753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2907707412704a5a4b79634da2ed76a5c75f5e0cb27c175078588d50e7de30da`  
		Last Modified: Tue, 31 Oct 2023 01:09:36 GMT  
		Size: 1.8 MB (1835281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:slim` - linux; s390x

```console
$ docker pull solr@sha256:4c2ac61c2278165937d9b02dba961a6b0cc23dcef20739d878910d7624fc8751
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.5 MB (155474022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a147f632ba4b0b12163e14e2cad34e70fe13f8fb3f75a0807ecbcbadbf00f2a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 05 Oct 2023 07:29:34 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:29:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:29:36 GMT
ADD file:d165475f8f027ab758a463da57c8c29f5d302f0a87a475ac68fdfae30005c7ac in / 
# Thu, 05 Oct 2023 07:29:36 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 10:09:28 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 10:09:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 10:09:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 30 Oct 2023 23:26:44 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 30 Oct 2023 23:26:46 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Mon, 30 Oct 2023 23:27:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 30 Oct 2023 23:27:50 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:27:50 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:27:50 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 31 Oct 2023 00:56:00 GMT
ARG SOLR_VERSION=9.4.0
# Tue, 31 Oct 2023 00:56:53 GMT
ARG SOLR_DIST=-slim
# Tue, 31 Oct 2023 00:56:53 GMT
ARG SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a
# Tue, 31 Oct 2023 00:56:53 GMT
ARG SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E
# Tue, 31 Oct 2023 00:56:53 GMT
ARG SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr
# Tue, 31 Oct 2023 00:57:05 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;   apt-get update;   apt-get -y --no-install-recommends install wget gpg gnupg dirmngr;   rm -rf /var/lib/apt/lists/*;   export SOLR_BINARY="solr-$SOLR_VERSION$SOLR_DIST.tgz";   MAX_REDIRECTS=3;   case "${SOLR_DOWNLOAD_SERVER}" in     (*"apache.org"*);;     (*)       MAX_REDIRECTS=4 &&       SKIP_GPG_CHECK=true;;   esac;   export DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/$SOLR_BINARY";   echo "downloading $DOWNLOAD_URL";   if ! wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$DOWNLOAD_URL" -O "/opt/$SOLR_BINARY"; then rm -f "/opt/$SOLR_BINARY"; fi;   if [ ! -f "/opt/$SOLR_BINARY" ]; then echo "failed download attempt for $SOLR_BINARY"; exit 1; fi;   echo "$SOLR_SHA512 */opt/$SOLR_BINARY" | sha512sum -c -;   if [ -z "$SKIP_GPG_CHECK" ]; then     export GNUPGHOME="/tmp/gnupg_home";     mkdir -p "$GNUPGHOME";     chmod 700 "$GNUPGHOME";     echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";     if [ -n "$SOLR_KEYS" ]; then       wget -nv "https://downloads.apache.org/solr/KEYS" -O- |         gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';       release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";       rm -rf "$GNUPGHOME"/*;       echo "${release_keys}" | gpg --batch --import;     fi;     echo "downloading $DOWNLOAD_URL.asc";     wget -nv "$DOWNLOAD_URL.asc" -O "/opt/$SOLR_BINARY.asc";     (>&2 ls -l "/opt/$SOLR_BINARY" "/opt/$SOLR_BINARY.asc");     gpg --batch --verify "/opt/$SOLR_BINARY.asc" "/opt/$SOLR_BINARY";     { command -v gpgconf; gpgconf --kill all || :; };     rm -r "$GNUPGHOME";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --preserve-permissions --file "/opt/$SOLR_BINARY";   rm "/opt/$SOLR_BINARY"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Tue, 31 Oct 2023 00:57:06 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Tue, 31 Oct 2023 00:57:07 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Tue, 31 Oct 2023 00:57:07 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Tue, 31 Oct 2023 00:57:07 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Tue, 31 Oct 2023 00:57:07 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Tue, 31 Oct 2023 00:57:07 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Tue, 31 Oct 2023 00:57:07 GMT
LABEL org.opencontainers.image.version=9.4.0
# Tue, 31 Oct 2023 00:57:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 31 Oct 2023 00:57:07 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0 SOLR_ZK_EMBEDDED_HOST=0.0.0.0
# Tue, 31 Oct 2023 00:57:08 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 31 Oct 2023 00:57:09 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Tue, 31 Oct 2023 00:57:09 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   test ! -e /opt/solr/modules || ln -s /opt/solr/modules /opt/solr/contrib;   test ! -e /opt/solr/prometheus-exporter || ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Tue, 31 Oct 2023 00:57:12 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=2289AC4180E130507D7A82F479C211E0AEFCA72E SOLR_SHA512=4ae8929f4c8ac275b1c9e8c45f17c3557fa34c46d9fdb171243f5c575466a9dba86216fbb0ea951a7ae9f16acf38ce292276dd9f033b82b2e5211de9d8ed397a SOLR_VERSION=9.4.0
RUN set -ex;     apt-get update;     apt-get -y --no-install-recommends install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Tue, 31 Oct 2023 00:57:12 GMT
VOLUME [/var/solr]
# Tue, 31 Oct 2023 00:57:13 GMT
EXPOSE 8983
# Tue, 31 Oct 2023 00:57:13 GMT
WORKDIR /opt/solr
# Tue, 31 Oct 2023 00:57:13 GMT
USER 8983
# Tue, 31 Oct 2023 00:57:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Oct 2023 00:57:13 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:818e4e246beb9ab026d2b95bf051fe9610b92dbc0a35b45d09b0cf237b6f3c2e`  
		Last Modified: Fri, 13 Oct 2023 10:16:45 GMT  
		Size: 28.7 MB (28650497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fd9089ff570b1dfbf551e4263c4e283a141fa14f2c9a883b102522fb88942d`  
		Last Modified: Mon, 30 Oct 2023 23:30:42 GMT  
		Size: 17.3 MB (17254458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a906515289c418bbfec894bb59e09ae1511d21cf0e8d0a532863411321b86050`  
		Last Modified: Mon, 30 Oct 2023 23:31:34 GMT  
		Size: 43.8 MB (43754406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef8030eda8efb304314e4f37622c0b8c9af866d58ae687798696e82cb6ff2a4`  
		Last Modified: Mon, 30 Oct 2023 23:31:28 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8adf2568b18a66daa134954dd64a7ca86e2d783b5abb6cadb54ea5820b96e629`  
		Last Modified: Mon, 30 Oct 2023 23:31:28 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299ffc2721e34722daa03adc3366009b21b2c636ae146770ed48941a3e93daa0`  
		Last Modified: Tue, 31 Oct 2023 01:04:27 GMT  
		Size: 64.0 MB (64022838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8e7a5aea35ba3839efc28aa916655f1c371df37b395dc58a683237f5226741`  
		Last Modified: Tue, 31 Oct 2023 01:04:22 GMT  
		Size: 4.3 KB (4329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58087af3b7059edb1cc002ce9bcb29933cd4c9075d21384014c35b1e18119227`  
		Last Modified: Tue, 31 Oct 2023 01:04:22 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d7368021b4261d03f4868c26927cb8cc2726a3a82b259d3e680a17b24c4817`  
		Last Modified: Tue, 31 Oct 2023 01:04:22 GMT  
		Size: 10.8 KB (10753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d202caab721a37567fbefd62f5f5797d93ae520d8fe8ac08f6cc12fba89551c1`  
		Last Modified: Tue, 31 Oct 2023 01:04:23 GMT  
		Size: 1.8 MB (1775625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
