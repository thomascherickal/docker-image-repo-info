## `solr:9-slim`

```console
$ docker pull solr@sha256:c6cf1065e77f1f5f583ce7afd69f29cdc9e017f9ed7a1989750a158fe93dc760
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `solr:9-slim` - linux; amd64

```console
$ docker pull solr@sha256:542870c791de293df1542d5b8df1cdcd5f8ae35a22334288053bba2705c7e795
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.1 MB (159121521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0773239a5c402b9329d3333eb86d4dd49ad1c6cf4206178762df7230f671deb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 20:33:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 20:33:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 20:33:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 04 Jul 2023 20:36:31 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:36:31 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Tue, 04 Jul 2023 20:37:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 04 Jul 2023 20:37:08 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 22 Jul 2023 01:22:27 GMT
ARG SOLR_VERSION=9.3.0
# Sat, 22 Jul 2023 01:23:08 GMT
ARG SOLR_DIST=-slim
# Sat, 22 Jul 2023 01:23:08 GMT
ARG SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076
# Sat, 22 Jul 2023 01:23:08 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Sat, 22 Jul 2023 01:23:08 GMT
ARG SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr
# Sat, 22 Jul 2023 01:23:18 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076 SOLR_VERSION=9.3.0
RUN set -ex;   apt-get update;   apt-get -y --no-install-recommends install wget gpg gnupg dirmngr;   rm -rf /var/lib/apt/lists/*;   export SOLR_BINARY="solr-$SOLR_VERSION$SOLR_DIST.tgz";   MAX_REDIRECTS=3;   case "${SOLR_DOWNLOAD_SERVER}" in     (*"apache.org"*);;     (*)       MAX_REDIRECTS=4 &&       SKIP_GPG_CHECK=true;;   esac;   export DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/$SOLR_BINARY";   echo "downloading $DOWNLOAD_URL";   if ! wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$DOWNLOAD_URL" -O "/opt/$SOLR_BINARY"; then rm -f "/opt/$SOLR_BINARY"; fi;   if [ ! -f "/opt/$SOLR_BINARY" ]; then echo "failed download attempt for $SOLR_BINARY"; exit 1; fi;   echo "$SOLR_SHA512 */opt/$SOLR_BINARY" | sha512sum -c -;   if [ -z "$SKIP_GPG_CHECK" ]; then     export GNUPGHOME="/tmp/gnupg_home";     mkdir -p "$GNUPGHOME";     chmod 700 "$GNUPGHOME";     echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";     if [ -n "$SOLR_KEYS" ]; then       wget -nv "https://downloads.apache.org/solr/KEYS" -O- |         gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';       release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";       rm -rf "$GNUPGHOME"/*;       echo "${release_keys}" | gpg --batch --import;     fi;     echo "downloading $DOWNLOAD_URL.asc";     wget -nv "$DOWNLOAD_URL.asc" -O "/opt/$SOLR_BINARY.asc";     (>&2 ls -l "/opt/$SOLR_BINARY" "/opt/$SOLR_BINARY.asc");     gpg --batch --verify "/opt/$SOLR_BINARY.asc" "/opt/$SOLR_BINARY";     { command -v gpgconf; gpgconf --kill all || :; };     rm -r "$GNUPGHOME";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --preserve-permissions --file "/opt/$SOLR_BINARY";   rm "/opt/$SOLR_BINARY"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Sat, 22 Jul 2023 01:23:18 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Sat, 22 Jul 2023 01:23:19 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Sat, 22 Jul 2023 01:23:19 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Sat, 22 Jul 2023 01:23:19 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Sat, 22 Jul 2023 01:23:19 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Sat, 22 Jul 2023 01:23:19 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Sat, 22 Jul 2023 01:23:19 GMT
LABEL org.opencontainers.image.version=9.3.0
# Sat, 22 Jul 2023 01:23:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 22 Jul 2023 01:23:19 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Sat, 22 Jul 2023 01:23:20 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076 SOLR_VERSION=9.3.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Sat, 22 Jul 2023 01:23:20 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076 SOLR_VERSION=9.3.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Sat, 22 Jul 2023 01:23:21 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076 SOLR_VERSION=9.3.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   test ! -e /opt/solr/modules || ln -s /opt/solr/modules /opt/solr/contrib;   test ! -e /opt/solr/prometheus-exporter || ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Sat, 22 Jul 2023 01:23:25 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076 SOLR_VERSION=9.3.0
RUN set -ex;     apt-get update;     apt-get -y --no-install-recommends install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Sat, 22 Jul 2023 01:23:25 GMT
VOLUME [/var/solr]
# Sat, 22 Jul 2023 01:23:25 GMT
EXPOSE 8983
# Sat, 22 Jul 2023 01:23:25 GMT
WORKDIR /opt/solr
# Sat, 22 Jul 2023 01:23:25 GMT
USER 8983
# Sat, 22 Jul 2023 01:23:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Jul 2023 01:23:25 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b566cb887b5c06e04f5cd97660a99e73bd52ceb9d72c6db6383ae8470cc4cf`  
		Last Modified: Tue, 04 Jul 2023 20:41:38 GMT  
		Size: 17.0 MB (17040993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc8f3b3863b8985ba0a6078c433c2f720b393c4a85af108476993b5b1ad4bce`  
		Last Modified: Tue, 04 Jul 2023 20:42:23 GMT  
		Size: 47.0 MB (47006277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb2b830c8b634c56503567ad290d66305d253111cfc90f53a0b81826df2ce81`  
		Last Modified: Tue, 04 Jul 2023 20:42:16 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4d1b4a8124e641596534286af034365fef75fdeee41f0a9c62c55b70e9386e`  
		Last Modified: Sat, 22 Jul 2023 01:24:23 GMT  
		Size: 62.8 MB (62799882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb411464774434c04628d1456c6919147ecb12f50594b2df54923e033f06be29`  
		Last Modified: Sat, 22 Jul 2023 01:24:19 GMT  
		Size: 4.3 KB (4295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9d792089f535ab6781017adc5f502e75f44eec202dc755aca78df2b96e7e1f`  
		Last Modified: Sat, 22 Jul 2023 01:24:19 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:175cc9a3861c877ad6573a83744c9a1d08f28e38cfe0200dea200d748e032e5a`  
		Last Modified: Sat, 22 Jul 2023 01:24:19 GMT  
		Size: 10.6 KB (10645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428f2cc660cbfc0e45f75ecb4fe3fb8ded66d4e41023ce09156b203dd10b7e98`  
		Last Modified: Sat, 22 Jul 2023 01:24:20 GMT  
		Size: 1.8 MB (1827818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9-slim` - linux; arm variant v7

```console
$ docker pull solr@sha256:cc492119f957777e62015c61c48792f80e1b20da7062e842dd8e7ecd4dd11dd8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.2 MB (153244529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d2815199ab1958a53550adf0b2ace774152c44d445d863977f6a1e0150daa5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 28 Jun 2023 08:41:15 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:41:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:41:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:41:15 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:41:18 GMT
ADD file:c13f43a31510c7a4eaa7e4ca90e4f973b19895658b1f9993cab5f93979d4e2dc in / 
# Wed, 28 Jun 2023 08:41:18 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 20:09:30 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 20:09:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 20:09:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 04 Jul 2023 20:12:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:12:13 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Tue, 04 Jul 2023 20:12:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 04 Jul 2023 20:12:48 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 22 Jul 2023 01:13:14 GMT
ARG SOLR_VERSION=9.3.0
# Sat, 22 Jul 2023 01:14:12 GMT
ARG SOLR_DIST=-slim
# Sat, 22 Jul 2023 01:14:12 GMT
ARG SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076
# Sat, 22 Jul 2023 01:14:12 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Sat, 22 Jul 2023 01:14:12 GMT
ARG SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr
# Sat, 22 Jul 2023 01:14:23 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076 SOLR_VERSION=9.3.0
RUN set -ex;   apt-get update;   apt-get -y --no-install-recommends install wget gpg gnupg dirmngr;   rm -rf /var/lib/apt/lists/*;   export SOLR_BINARY="solr-$SOLR_VERSION$SOLR_DIST.tgz";   MAX_REDIRECTS=3;   case "${SOLR_DOWNLOAD_SERVER}" in     (*"apache.org"*);;     (*)       MAX_REDIRECTS=4 &&       SKIP_GPG_CHECK=true;;   esac;   export DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/$SOLR_BINARY";   echo "downloading $DOWNLOAD_URL";   if ! wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$DOWNLOAD_URL" -O "/opt/$SOLR_BINARY"; then rm -f "/opt/$SOLR_BINARY"; fi;   if [ ! -f "/opt/$SOLR_BINARY" ]; then echo "failed download attempt for $SOLR_BINARY"; exit 1; fi;   echo "$SOLR_SHA512 */opt/$SOLR_BINARY" | sha512sum -c -;   if [ -z "$SKIP_GPG_CHECK" ]; then     export GNUPGHOME="/tmp/gnupg_home";     mkdir -p "$GNUPGHOME";     chmod 700 "$GNUPGHOME";     echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";     if [ -n "$SOLR_KEYS" ]; then       wget -nv "https://downloads.apache.org/solr/KEYS" -O- |         gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';       release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";       rm -rf "$GNUPGHOME"/*;       echo "${release_keys}" | gpg --batch --import;     fi;     echo "downloading $DOWNLOAD_URL.asc";     wget -nv "$DOWNLOAD_URL.asc" -O "/opt/$SOLR_BINARY.asc";     (>&2 ls -l "/opt/$SOLR_BINARY" "/opt/$SOLR_BINARY.asc");     gpg --batch --verify "/opt/$SOLR_BINARY.asc" "/opt/$SOLR_BINARY";     { command -v gpgconf; gpgconf --kill all || :; };     rm -r "$GNUPGHOME";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --preserve-permissions --file "/opt/$SOLR_BINARY";   rm "/opt/$SOLR_BINARY"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Sat, 22 Jul 2023 01:14:23 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Sat, 22 Jul 2023 01:14:23 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Sat, 22 Jul 2023 01:14:23 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Sat, 22 Jul 2023 01:14:23 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Sat, 22 Jul 2023 01:14:23 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Sat, 22 Jul 2023 01:14:23 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Sat, 22 Jul 2023 01:14:24 GMT
LABEL org.opencontainers.image.version=9.3.0
# Sat, 22 Jul 2023 01:14:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 22 Jul 2023 01:14:24 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Sat, 22 Jul 2023 01:14:24 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076 SOLR_VERSION=9.3.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Sat, 22 Jul 2023 01:14:25 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076 SOLR_VERSION=9.3.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Sat, 22 Jul 2023 01:14:25 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076 SOLR_VERSION=9.3.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   test ! -e /opt/solr/modules || ln -s /opt/solr/modules /opt/solr/contrib;   test ! -e /opt/solr/prometheus-exporter || ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Sat, 22 Jul 2023 01:14:29 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076 SOLR_VERSION=9.3.0
RUN set -ex;     apt-get update;     apt-get -y --no-install-recommends install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Sat, 22 Jul 2023 01:14:30 GMT
VOLUME [/var/solr]
# Sat, 22 Jul 2023 01:14:30 GMT
EXPOSE 8983
# Sat, 22 Jul 2023 01:14:30 GMT
WORKDIR /opt/solr
# Sat, 22 Jul 2023 01:14:30 GMT
USER 8983
# Sat, 22 Jul 2023 01:14:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Jul 2023 01:14:30 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:63b96265cfe95b9cec847027033d4226b783ecd042036f5c809a7386027f56b0`  
		Last Modified: Fri, 30 Jun 2023 02:08:02 GMT  
		Size: 27.0 MB (27026961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0088a9419e3b2e2bbe5af516cf63e967bd59dd3eb3046bb535e990d2f9cb312d`  
		Last Modified: Tue, 04 Jul 2023 20:16:17 GMT  
		Size: 17.2 MB (17168999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce1dfa4fd36974f85b8031fce1342b22f39e631cd66ec5e0e5a7daae7376ac6`  
		Last Modified: Tue, 04 Jul 2023 20:17:02 GMT  
		Size: 44.6 MB (44579943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0db5973678ee0a40ccac457ba16c09c864183af7ce8d1bd26fc49cbd01ecc3f`  
		Last Modified: Tue, 04 Jul 2023 20:16:55 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39feb64d75e8fffb04368a758d686ddf231c02c9a73366f45061ca5eb572eb74`  
		Last Modified: Sat, 22 Jul 2023 01:15:34 GMT  
		Size: 62.8 MB (62800331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d85c5df93a2b6b41293358f0298fdde68705ab29b74fd3f1eda59bc9c3cd749`  
		Last Modified: Sat, 22 Jul 2023 01:15:29 GMT  
		Size: 4.2 KB (4228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00224f9de1fff093297873595a68b33cf62599d14187bdfeb358d9704d63ebfa`  
		Last Modified: Sat, 22 Jul 2023 01:15:29 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db44608a07c21dfa99fb543bdc76534ed93bd434f03981ae9878061348fe06bc`  
		Last Modified: Sat, 22 Jul 2023 01:15:29 GMT  
		Size: 10.6 KB (10648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7ba6c55ef3d10b348797557e8c3dc5cf502f47990070cc233da9bf12fa1a6a`  
		Last Modified: Sat, 22 Jul 2023 01:15:30 GMT  
		Size: 1.7 MB (1653036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9-slim` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:1df5e3d21c4a2652597c124433b599032053d9ef97e41efddc38f206e3778dde
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.9 MB (157850924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44d8e7a98db892018776eb4db63e75df8cb8d2290659f332e8bb42404b0330a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:32:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 15:32:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 15:32:45 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 04 Jul 2023 15:34:51 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 15:34:51 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Tue, 04 Jul 2023 15:35:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 04 Jul 2023 15:35:17 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 22 Jul 2023 01:05:06 GMT
ARG SOLR_VERSION=9.3.0
# Sat, 22 Jul 2023 01:06:03 GMT
ARG SOLR_DIST=-slim
# Sat, 22 Jul 2023 01:06:03 GMT
ARG SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076
# Sat, 22 Jul 2023 01:06:03 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Sat, 22 Jul 2023 01:06:03 GMT
ARG SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr
# Sat, 22 Jul 2023 01:06:17 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076 SOLR_VERSION=9.3.0
RUN set -ex;   apt-get update;   apt-get -y --no-install-recommends install wget gpg gnupg dirmngr;   rm -rf /var/lib/apt/lists/*;   export SOLR_BINARY="solr-$SOLR_VERSION$SOLR_DIST.tgz";   MAX_REDIRECTS=3;   case "${SOLR_DOWNLOAD_SERVER}" in     (*"apache.org"*);;     (*)       MAX_REDIRECTS=4 &&       SKIP_GPG_CHECK=true;;   esac;   export DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/$SOLR_BINARY";   echo "downloading $DOWNLOAD_URL";   if ! wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$DOWNLOAD_URL" -O "/opt/$SOLR_BINARY"; then rm -f "/opt/$SOLR_BINARY"; fi;   if [ ! -f "/opt/$SOLR_BINARY" ]; then echo "failed download attempt for $SOLR_BINARY"; exit 1; fi;   echo "$SOLR_SHA512 */opt/$SOLR_BINARY" | sha512sum -c -;   if [ -z "$SKIP_GPG_CHECK" ]; then     export GNUPGHOME="/tmp/gnupg_home";     mkdir -p "$GNUPGHOME";     chmod 700 "$GNUPGHOME";     echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";     if [ -n "$SOLR_KEYS" ]; then       wget -nv "https://downloads.apache.org/solr/KEYS" -O- |         gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';       release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";       rm -rf "$GNUPGHOME"/*;       echo "${release_keys}" | gpg --batch --import;     fi;     echo "downloading $DOWNLOAD_URL.asc";     wget -nv "$DOWNLOAD_URL.asc" -O "/opt/$SOLR_BINARY.asc";     (>&2 ls -l "/opt/$SOLR_BINARY" "/opt/$SOLR_BINARY.asc");     gpg --batch --verify "/opt/$SOLR_BINARY.asc" "/opt/$SOLR_BINARY";     { command -v gpgconf; gpgconf --kill all || :; };     rm -r "$GNUPGHOME";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --preserve-permissions --file "/opt/$SOLR_BINARY";   rm "/opt/$SOLR_BINARY"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Sat, 22 Jul 2023 01:06:17 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Sat, 22 Jul 2023 01:06:17 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Sat, 22 Jul 2023 01:06:18 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Sat, 22 Jul 2023 01:06:18 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Sat, 22 Jul 2023 01:06:18 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Sat, 22 Jul 2023 01:06:18 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Sat, 22 Jul 2023 01:06:18 GMT
LABEL org.opencontainers.image.version=9.3.0
# Sat, 22 Jul 2023 01:06:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 22 Jul 2023 01:06:18 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Sat, 22 Jul 2023 01:06:19 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076 SOLR_VERSION=9.3.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Sat, 22 Jul 2023 01:06:19 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076 SOLR_VERSION=9.3.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Sat, 22 Jul 2023 01:06:20 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076 SOLR_VERSION=9.3.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   test ! -e /opt/solr/modules || ln -s /opt/solr/modules /opt/solr/contrib;   test ! -e /opt/solr/prometheus-exporter || ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Sat, 22 Jul 2023 01:06:23 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076 SOLR_VERSION=9.3.0
RUN set -ex;     apt-get update;     apt-get -y --no-install-recommends install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Sat, 22 Jul 2023 01:06:23 GMT
VOLUME [/var/solr]
# Sat, 22 Jul 2023 01:06:23 GMT
EXPOSE 8983
# Sat, 22 Jul 2023 01:06:24 GMT
WORKDIR /opt/solr
# Sat, 22 Jul 2023 01:06:24 GMT
USER 8983
# Sat, 22 Jul 2023 01:06:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Jul 2023 01:06:24 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f85d89e7da0f3af0f527e7300cced784d0ba64249b8c376690599d313cb056`  
		Last Modified: Tue, 04 Jul 2023 15:39:09 GMT  
		Size: 18.5 MB (18466568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1fcde918d2f180d437fd09c8ef6f797f4ea4708a3eb7e748a902cfa5f586f8`  
		Last Modified: Tue, 04 Jul 2023 15:39:47 GMT  
		Size: 46.5 MB (46488633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:befad100d8565490272428227d229ff10ea84d74312878f1dd7605f7838dc916`  
		Last Modified: Tue, 04 Jul 2023 15:39:42 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f9af9267b16c84c48f54f16d7002f64fde9a37c4a3657c7d1c1b82dda9fa24`  
		Last Modified: Sat, 22 Jul 2023 01:07:18 GMT  
		Size: 62.8 MB (62801301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420e074f68387893fae61dd3d8b9c21b119c2319c51bc04da425735284677e80`  
		Last Modified: Sat, 22 Jul 2023 01:07:15 GMT  
		Size: 4.3 KB (4333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d812df0b74f07ebbdeba125468b685b0709b1a3f77491c1464c2473d8a2dc4b`  
		Last Modified: Sat, 22 Jul 2023 01:07:15 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff566725e04731f60656fa1cf2f7d501c10642549df95e0318f605b1e6cd6cbf`  
		Last Modified: Sat, 22 Jul 2023 01:07:15 GMT  
		Size: 10.6 KB (10642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a894ac2fe9bdd912191c5c630eafa36e434ddfc8da092f8250ad5b2b1a016552`  
		Last Modified: Sat, 22 Jul 2023 01:07:15 GMT  
		Size: 1.7 MB (1688054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9-slim` - linux; ppc64le

```console
$ docker pull solr@sha256:7eafaea53009bf11765efa194222f3e2b296d699ce3ed63ef3b500c350d975f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165557652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0adb35b16b78b874be5a5519b3c2d91c5943c330f774f65d7b4cf967967f08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 00:18:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Jul 2023 00:18:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Jul 2023 00:18:19 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Jul 2023 00:24:51 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 00:24:53 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 05 Jul 2023 00:26:09 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 05 Jul 2023 00:26:16 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 22 Jul 2023 01:17:12 GMT
ARG SOLR_VERSION=9.3.0
# Sat, 22 Jul 2023 01:19:21 GMT
ARG SOLR_DIST=-slim
# Sat, 22 Jul 2023 01:19:22 GMT
ARG SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076
# Sat, 22 Jul 2023 01:19:22 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Sat, 22 Jul 2023 01:19:23 GMT
ARG SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr
# Sat, 22 Jul 2023 01:19:56 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076 SOLR_VERSION=9.3.0
RUN set -ex;   apt-get update;   apt-get -y --no-install-recommends install wget gpg gnupg dirmngr;   rm -rf /var/lib/apt/lists/*;   export SOLR_BINARY="solr-$SOLR_VERSION$SOLR_DIST.tgz";   MAX_REDIRECTS=3;   case "${SOLR_DOWNLOAD_SERVER}" in     (*"apache.org"*);;     (*)       MAX_REDIRECTS=4 &&       SKIP_GPG_CHECK=true;;   esac;   export DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/$SOLR_BINARY";   echo "downloading $DOWNLOAD_URL";   if ! wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$DOWNLOAD_URL" -O "/opt/$SOLR_BINARY"; then rm -f "/opt/$SOLR_BINARY"; fi;   if [ ! -f "/opt/$SOLR_BINARY" ]; then echo "failed download attempt for $SOLR_BINARY"; exit 1; fi;   echo "$SOLR_SHA512 */opt/$SOLR_BINARY" | sha512sum -c -;   if [ -z "$SKIP_GPG_CHECK" ]; then     export GNUPGHOME="/tmp/gnupg_home";     mkdir -p "$GNUPGHOME";     chmod 700 "$GNUPGHOME";     echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";     if [ -n "$SOLR_KEYS" ]; then       wget -nv "https://downloads.apache.org/solr/KEYS" -O- |         gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';       release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";       rm -rf "$GNUPGHOME"/*;       echo "${release_keys}" | gpg --batch --import;     fi;     echo "downloading $DOWNLOAD_URL.asc";     wget -nv "$DOWNLOAD_URL.asc" -O "/opt/$SOLR_BINARY.asc";     (>&2 ls -l "/opt/$SOLR_BINARY" "/opt/$SOLR_BINARY.asc");     gpg --batch --verify "/opt/$SOLR_BINARY.asc" "/opt/$SOLR_BINARY";     { command -v gpgconf; gpgconf --kill all || :; };     rm -r "$GNUPGHOME";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --preserve-permissions --file "/opt/$SOLR_BINARY";   rm "/opt/$SOLR_BINARY"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Sat, 22 Jul 2023 01:19:59 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Sat, 22 Jul 2023 01:20:00 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Sat, 22 Jul 2023 01:20:01 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Sat, 22 Jul 2023 01:20:02 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Sat, 22 Jul 2023 01:20:03 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Sat, 22 Jul 2023 01:20:03 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Sat, 22 Jul 2023 01:20:04 GMT
LABEL org.opencontainers.image.version=9.3.0
# Sat, 22 Jul 2023 01:20:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 22 Jul 2023 01:20:06 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Sat, 22 Jul 2023 01:20:07 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076 SOLR_VERSION=9.3.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Sat, 22 Jul 2023 01:20:09 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076 SOLR_VERSION=9.3.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Sat, 22 Jul 2023 01:20:11 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076 SOLR_VERSION=9.3.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   test ! -e /opt/solr/modules || ln -s /opt/solr/modules /opt/solr/contrib;   test ! -e /opt/solr/prometheus-exporter || ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Sat, 22 Jul 2023 01:20:33 GMT
# ARGS: SOLR_DIST=-slim SOLR_DOWNLOAD_SERVER=https://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=432306fa6db9d772df84d6acb3adab095783dda10e55280bfd443e197969271364d86f5c64d737ca6c6660bda81e13ffe404e34feb8447dff6ca0cd302ddd076 SOLR_VERSION=9.3.0
RUN set -ex;     apt-get update;     apt-get -y --no-install-recommends install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Sat, 22 Jul 2023 01:20:38 GMT
VOLUME [/var/solr]
# Sat, 22 Jul 2023 01:20:40 GMT
EXPOSE 8983
# Sat, 22 Jul 2023 01:20:41 GMT
WORKDIR /opt/solr
# Sat, 22 Jul 2023 01:20:42 GMT
USER 8983
# Sat, 22 Jul 2023 01:20:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Jul 2023 01:20:44 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0702eb13eba9354d51e77a2d58efab5ae9583215718d284f381726cce4f00d`  
		Last Modified: Wed, 05 Jul 2023 00:32:18 GMT  
		Size: 18.3 MB (18323397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4c5592e3694086851e16968c2af7d7337a178033ac0ef221e3ef4469b16ee1`  
		Last Modified: Wed, 05 Jul 2023 00:33:32 GMT  
		Size: 46.9 MB (46872503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4f7592eeb86052232f83f93e841960ca9cf8841d428e413b7fc24b8e9ffc9e`  
		Last Modified: Wed, 05 Jul 2023 00:33:20 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e40bb38dde20af7b7b61053c83089ec2a27f30298f80bac01adffab6c5682fd`  
		Last Modified: Sat, 22 Jul 2023 01:22:28 GMT  
		Size: 62.8 MB (62800640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df6d21eb07df2947fb25534af7e79134f69c2074d7f9a39d219a00555170433`  
		Last Modified: Sat, 22 Jul 2023 01:22:22 GMT  
		Size: 4.3 KB (4296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cc5917662687812aafba92b7552da63d2d61ec385c3d218cb8bbb95d6cbc91`  
		Last Modified: Sat, 22 Jul 2023 01:22:22 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2cbc3777c42f3b5a18477378719e44b1a5bf8c4ec35b3c4c9b5ad0c4e39f75`  
		Last Modified: Sat, 22 Jul 2023 01:22:22 GMT  
		Size: 10.7 KB (10659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953c7863a41c33188a353b7cf41d3147da4a9c3a401418813e5a712d293750fe`  
		Last Modified: Sat, 22 Jul 2023 01:22:22 GMT  
		Size: 1.8 MB (1834305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
