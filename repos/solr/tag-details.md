<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `solr`

-	[`solr:8`](#solr8)
-	[`solr:8-slim`](#solr8-slim)
-	[`solr:8.11`](#solr811)
-	[`solr:8.11-slim`](#solr811-slim)
-	[`solr:8.11.2`](#solr8112)
-	[`solr:8.11.2-slim`](#solr8112-slim)
-	[`solr:9`](#solr9)
-	[`solr:9.0`](#solr90)
-	[`solr:9.0.0`](#solr900)
-	[`solr:9.1`](#solr91)
-	[`solr:9.1.1`](#solr911)
-	[`solr:9.2`](#solr92)
-	[`solr:9.2.1`](#solr921)
-	[`solr:latest`](#solrlatest)

## `solr:8`

```console
$ docker pull solr@sha256:123ec0e30b444b5a6a02dc2435efa4c987d4ea56e59096e2b9ef4f4cec29cd4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `solr:8` - linux; amd64

```console
$ docker pull solr@sha256:7b77d4d3a0e9caf84e5e862e571bed8b9ca1331fc749d73f718d0eaeed6b46c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.9 MB (314902545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c927f6e7447da43ff7b242422647ceaa3fdd2f428714cd1c45eb7401037a3b7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:15:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:15:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:15:07 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:15:39 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:16:51 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 02:17:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:17:31 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:29:28 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 05:29:28 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:29:35 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 05:29:35 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 05:29:36 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:29:41 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 05:30:14 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 05:30:15 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 05:30:15 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:30:15 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:30:15 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:30:15 GMT
USER 8983
# Fri, 16 Jun 2023 05:30:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:30:15 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491508b827d83492c058d6e12e6ee1fe2f0e8328a6a5254f225537a15ef24bfe`  
		Last Modified: Fri, 16 Jun 2023 02:20:43 GMT  
		Size: 16.4 MB (16413378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1d6f5b86c355e0656c507178ce8f4719ba6d4640dd32454ae56a021577aff2`  
		Last Modified: Fri, 16 Jun 2023 02:22:39 GMT  
		Size: 46.7 MB (46664972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8c9ad9fc2c5ff99353581f54c02e5ccfc7a745f9d254b89b2a76ab4b5a1388`  
		Last Modified: Fri, 16 Jun 2023 02:22:33 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8875bfce5e356f6a6c69b048c0352efb474398130f74d3d4ba4dc7b9f442145b`  
		Last Modified: Fri, 16 Jun 2023 05:31:41 GMT  
		Size: 4.9 MB (4901233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7a509476958a6dae54a50468f11922b675ecc500508d78f8b6681279c296ba`  
		Last Modified: Fri, 16 Jun 2023 05:31:40 GMT  
		Size: 4.3 KB (4292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5463314ac566a3f0665b25ff19f588bb4c8b1b4018d6030b153925465b811b`  
		Last Modified: Fri, 16 Jun 2023 05:31:40 GMT  
		Size: 3.5 KB (3464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c63f7ff1fc39d233fb0b8d502c6c25e56f6a67d5c1c499de29b09fcb492250e`  
		Last Modified: Fri, 16 Jun 2023 05:31:50 GMT  
		Size: 218.3 MB (218328218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1ea8856e2cb8f18a8018967fcd79e03003b3f827d8a5d43ed6ee01d317403d`  
		Last Modified: Fri, 16 Jun 2023 05:31:40 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8` - linux; arm variant v7

```console
$ docker pull solr@sha256:0c813cc7f3ec53209e6a37ae486a6310e52a49ab3fd115534c89f1d16bb0741e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.2 MB (307245039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b3ba4de150bda0840a7845811dbde7ce970246384bb4da34c971c7750a6bdf6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:24:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 01:24:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 01:24:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 01:24:49 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:26:23 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 01:27:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 01:27:04 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 02:41:14 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 02:41:14 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 02:41:15 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 02:41:21 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 02:41:21 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 02:41:21 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 02:41:31 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 02:42:09 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 02:42:10 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 02:42:10 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 02:42:10 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 02:42:10 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 02:42:10 GMT
USER 8983
# Fri, 16 Jun 2023 02:42:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 02:42:10 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:2d97abfcf215d35e8a846b390350fea9f455676b41221360fe8782163a1c46bb`  
		Last Modified: Thu, 15 Jun 2023 03:47:54 GMT  
		Size: 24.6 MB (24589116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9495a3be9c2c6747ed337799b868bba61986a721c67a700acfe6af4401aae5`  
		Last Modified: Fri, 16 Jun 2023 01:29:03 GMT  
		Size: 15.2 MB (15239860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa4be1a0221ca370894af24240ab41f02e9de16f9e2bcc3c291249e1a6f6e5b`  
		Last Modified: Fri, 16 Jun 2023 01:30:57 GMT  
		Size: 44.9 MB (44878070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9485255e1b5f7cd153d07a1b5898ee5e5bd85aa4a691daf554143ced7212c1`  
		Last Modified: Fri, 16 Jun 2023 01:30:50 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a7c708415525a81959edf16bc3d49f0f9a353a6ccbe62118f35a41d4badccb`  
		Last Modified: Fri, 16 Jun 2023 02:43:43 GMT  
		Size: 4.2 MB (4195564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef49861acb2439bd6a0a6f42a08da858a6dacef45c4b6b6d7c825973b22ee68`  
		Last Modified: Fri, 16 Jun 2023 02:43:42 GMT  
		Size: 4.2 KB (4227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184ca62e04698d0a2ce1cb95dba1910b5f5ac02f61355c24c5880a7c7be9eeb1`  
		Last Modified: Fri, 16 Jun 2023 02:43:43 GMT  
		Size: 3.5 KB (3468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9500fd7b0d4b665ed021c59c63e5b1dd2f1ad367bad3d01f7bc40900f851910`  
		Last Modified: Fri, 16 Jun 2023 02:43:54 GMT  
		Size: 218.3 MB (218328266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59dbadb77c53a247c461ee32ccfb2599ba7a1a573cd73de04c1f97630b61a67`  
		Last Modified: Fri, 16 Jun 2023 02:43:42 GMT  
		Size: 6.3 KB (6307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:1b4ea0e0e35837d0f6db13fb2a1e553d6a95adaff4852931281318d1f93d2ed2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.6 MB (311572971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:788806992a790f53caca77b9db76e2b2989ee188ed8ef3e767ba02d794c6b1da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:44:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:44:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:44:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:45:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:46:28 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 02:47:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:47:05 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:50:19 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 05:50:19 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:50:25 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 05:50:25 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 05:50:25 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:50:36 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 05:51:07 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 05:51:08 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 05:51:08 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:51:08 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:51:08 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:51:08 GMT
USER 8983
# Fri, 16 Jun 2023 05:51:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:51:09 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded85a30fdd137ed744a50296a089c18b7521b4a6423755763e7800084a35202`  
		Last Modified: Fri, 16 Jun 2023 02:49:42 GMT  
		Size: 16.3 MB (16269114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfc7474bf0993d4c615cd8ced7ac374026ba3ed62d57c6c3b883ddd60eeab1c`  
		Last Modified: Fri, 16 Jun 2023 02:51:23 GMT  
		Size: 45.0 MB (45009934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4224185bc45707d5ecf5e90b3d2f02b37a434000cac542530a00b3b48bfe3cc1`  
		Last Modified: Fri, 16 Jun 2023 02:51:18 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da95bc002c942fa9153e103b1a5d713d4d697a87cf89efc2dbabcf2f687582c9`  
		Last Modified: Fri, 16 Jun 2023 05:52:23 GMT  
		Size: 4.8 MB (4751007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea88f6087b1841d5b9307ee6b15a0d5181f2dfd7d72cf259b6324134d53ade6`  
		Last Modified: Fri, 16 Jun 2023 05:52:22 GMT  
		Size: 4.3 KB (4332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd91ceaa583a76bc85231b9ce41fd23fa35fb9256ee47d37ce5519525f1f4eab`  
		Last Modified: Fri, 16 Jun 2023 05:52:22 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed79fba284b4b35a82f34cdd8a083b228f925fe9d329c07e0f9d33c9607d2253`  
		Last Modified: Fri, 16 Jun 2023 05:52:30 GMT  
		Size: 218.3 MB (218328212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3106b45811e1338a0676a17f56cb843f09ca7f99f7780418d14da2e75efb0b`  
		Last Modified: Fri, 16 Jun 2023 05:52:22 GMT  
		Size: 6.3 KB (6309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8` - linux; ppc64le

```console
$ docker pull solr@sha256:e5bf7de5f3a81916ba68d0803b2a20683c3f343526ac4504bf83ff58a3554e7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.2 MB (317172564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622e27233dfd4792c9d6f51e19e2c8549ad71521b3e68abd69f92eceb9ec6724`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:24 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:25 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:28 GMT
ADD file:0a2372ac4d43f0f4ada2b55dd0a359df73a828a9aa9426bfdd05a02b9c4b2bd9 in / 
# Mon, 05 Jun 2023 17:08:28 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:17:32 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:17:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:17:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:18:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:20:58 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 02:22:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:22:25 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 07:41:31 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 07:41:31 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 07:41:32 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 07:41:32 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 07:41:33 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 07:41:33 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 07:41:34 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 07:41:55 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 07:41:56 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 07:42:00 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 07:42:17 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 07:42:49 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 07:42:52 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 07:42:53 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 07:42:55 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 07:42:57 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 07:42:58 GMT
USER 8983
# Fri, 16 Jun 2023 07:42:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 07:42:59 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:1fbda4a01aa9e184a223c30ab58441354cde30fe3083bc1d8ca9f7823ab4fe68`  
		Last Modified: Fri, 16 Jun 2023 01:24:20 GMT  
		Size: 33.3 MB (33309776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb717f01d0b915280274134b467bc61cb1a7be1d9c6a9fe149dd3e9ab5d4d5`  
		Last Modified: Fri, 16 Jun 2023 02:26:38 GMT  
		Size: 17.6 MB (17648879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd6c33e350c331fd82a3898e4308740b9228a93a9bd1cfbf209b8ac158961d6`  
		Last Modified: Fri, 16 Jun 2023 02:29:11 GMT  
		Size: 42.1 MB (42093841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ce0cb194906f7f8bf1248463cbef057861d206d072004bad81d1784fdb4b54`  
		Last Modified: Fri, 16 Jun 2023 02:29:00 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17d3ac8d21a63094e82ec5c4dc8dfa1c0cbfd4a7108d667bbf3b154435fa7f5`  
		Last Modified: Fri, 16 Jun 2023 07:44:57 GMT  
		Size: 5.8 MB (5777612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d596f773882c647c8f31f469e949edc08d29108d6e9eb47e8c45fae8fe6b8720`  
		Last Modified: Fri, 16 Jun 2023 07:44:55 GMT  
		Size: 4.3 KB (4297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7413d7cf84cc22e166149d3b19012981e5bcf3d7de8c109d5331ed65b172585`  
		Last Modified: Fri, 16 Jun 2023 07:44:55 GMT  
		Size: 3.5 KB (3469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5dedd276de4704622c2f0ba1ccc9b716e2b2000dc8af1b59a94b4c3f7c66a3`  
		Last Modified: Fri, 16 Jun 2023 07:45:12 GMT  
		Size: 218.3 MB (218328223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba39db06026d8858274e3c4e59ed877a895145ee633b4585cc44b1f4c38115b`  
		Last Modified: Fri, 16 Jun 2023 07:44:55 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8` - linux; s390x

```console
$ docker pull solr@sha256:3cb7e3eb537f722ef2d096a1cc9e90107d5a26a93eac004e2be96f7709fa7a7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.7 MB (306665402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc08946ca2b22de4fde16a15d59e3eb3989c0f8948b178b9440a9df20d36de60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:35 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:37 GMT
ADD file:44c66c03ba0afcc05de1b2078f83e8bfe04706b31491fcd3fdd93cfc88d5f06c in / 
# Thu, 13 Apr 2023 13:09:37 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:16:00 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:16:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:16:00 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:16:11 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:41:46 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:43:00 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:43:03 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:36:38 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 26 Apr 2023 20:36:38 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_VERSION=8.11.2
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:36:43 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 26 Apr 2023 20:36:44 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 26 Apr 2023 20:36:44 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:36:51 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 26 Apr 2023 20:37:07 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 26 Apr 2023 20:37:11 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 26 Apr 2023 20:37:11 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:37:12 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:37:12 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:37:12 GMT
USER 8983
# Wed, 26 Apr 2023 20:37:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:37:12 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:f11b609b1d63f2d37c0e3789823e7a7e62a078bddca7c46da8602655989c62d9`  
		Last Modified: Fri, 14 Apr 2023 09:38:39 GMT  
		Size: 27.0 MB (27016370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c307a57c5f07334cfab6db8f8324b0c9dff13121ec34d8db1d4a71e3529d4b5`  
		Last Modified: Tue, 18 Apr 2023 01:18:27 GMT  
		Size: 16.0 MB (16035272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f2464ae2b2cf26ad0951e353283a0faff6e21082c5b3ffc1ee96700cd352db8`  
		Last Modified: Wed, 26 Apr 2023 19:46:33 GMT  
		Size: 40.5 MB (40540743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2357373aba3b86e27f47b65c90b2c45aa55910d7a8e20ab95b0211c90ac0afc5`  
		Last Modified: Wed, 26 Apr 2023 19:46:28 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283aa23eb2725cd0f2f9e5627452bda5952b9f2b8279f3973cff4bc6bd8f2f8c`  
		Last Modified: Wed, 26 Apr 2023 20:38:26 GMT  
		Size: 4.7 MB (4730562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b9b134fa6b4ae6e10d35a150c618d122d72cb88c9c0def17080d179a2bc4fa`  
		Last Modified: Wed, 26 Apr 2023 20:38:25 GMT  
		Size: 4.3 KB (4333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b39ba054e26d24e3a1ea7e6e0fa808358921ad07e25bfe70ebde348e13891c`  
		Last Modified: Wed, 26 Apr 2023 20:38:25 GMT  
		Size: 3.5 KB (3468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a942f8f7937f22541141bb4ad17bd44e43cf1cbf39893673e50f572aa2f3fc27`  
		Last Modified: Wed, 26 Apr 2023 20:38:34 GMT  
		Size: 218.3 MB (218328187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3753012f9147597bbee82b53507c05d7009de3e3684021b64da90103d9d65c3f`  
		Last Modified: Wed, 26 Apr 2023 20:38:25 GMT  
		Size: 6.3 KB (6306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:8-slim`

```console
$ docker pull solr@sha256:123ec0e30b444b5a6a02dc2435efa4c987d4ea56e59096e2b9ef4f4cec29cd4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `solr:8-slim` - linux; amd64

```console
$ docker pull solr@sha256:7b77d4d3a0e9caf84e5e862e571bed8b9ca1331fc749d73f718d0eaeed6b46c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.9 MB (314902545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c927f6e7447da43ff7b242422647ceaa3fdd2f428714cd1c45eb7401037a3b7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:15:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:15:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:15:07 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:15:39 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:16:51 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 02:17:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:17:31 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:29:28 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 05:29:28 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:29:35 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 05:29:35 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 05:29:36 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:29:41 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 05:30:14 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 05:30:15 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 05:30:15 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:30:15 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:30:15 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:30:15 GMT
USER 8983
# Fri, 16 Jun 2023 05:30:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:30:15 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491508b827d83492c058d6e12e6ee1fe2f0e8328a6a5254f225537a15ef24bfe`  
		Last Modified: Fri, 16 Jun 2023 02:20:43 GMT  
		Size: 16.4 MB (16413378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1d6f5b86c355e0656c507178ce8f4719ba6d4640dd32454ae56a021577aff2`  
		Last Modified: Fri, 16 Jun 2023 02:22:39 GMT  
		Size: 46.7 MB (46664972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8c9ad9fc2c5ff99353581f54c02e5ccfc7a745f9d254b89b2a76ab4b5a1388`  
		Last Modified: Fri, 16 Jun 2023 02:22:33 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8875bfce5e356f6a6c69b048c0352efb474398130f74d3d4ba4dc7b9f442145b`  
		Last Modified: Fri, 16 Jun 2023 05:31:41 GMT  
		Size: 4.9 MB (4901233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7a509476958a6dae54a50468f11922b675ecc500508d78f8b6681279c296ba`  
		Last Modified: Fri, 16 Jun 2023 05:31:40 GMT  
		Size: 4.3 KB (4292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5463314ac566a3f0665b25ff19f588bb4c8b1b4018d6030b153925465b811b`  
		Last Modified: Fri, 16 Jun 2023 05:31:40 GMT  
		Size: 3.5 KB (3464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c63f7ff1fc39d233fb0b8d502c6c25e56f6a67d5c1c499de29b09fcb492250e`  
		Last Modified: Fri, 16 Jun 2023 05:31:50 GMT  
		Size: 218.3 MB (218328218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1ea8856e2cb8f18a8018967fcd79e03003b3f827d8a5d43ed6ee01d317403d`  
		Last Modified: Fri, 16 Jun 2023 05:31:40 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8-slim` - linux; arm variant v7

```console
$ docker pull solr@sha256:0c813cc7f3ec53209e6a37ae486a6310e52a49ab3fd115534c89f1d16bb0741e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.2 MB (307245039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b3ba4de150bda0840a7845811dbde7ce970246384bb4da34c971c7750a6bdf6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:24:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 01:24:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 01:24:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 01:24:49 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:26:23 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 01:27:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 01:27:04 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 02:41:14 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 02:41:14 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 02:41:15 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 02:41:21 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 02:41:21 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 02:41:21 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 02:41:31 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 02:42:09 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 02:42:10 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 02:42:10 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 02:42:10 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 02:42:10 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 02:42:10 GMT
USER 8983
# Fri, 16 Jun 2023 02:42:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 02:42:10 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:2d97abfcf215d35e8a846b390350fea9f455676b41221360fe8782163a1c46bb`  
		Last Modified: Thu, 15 Jun 2023 03:47:54 GMT  
		Size: 24.6 MB (24589116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9495a3be9c2c6747ed337799b868bba61986a721c67a700acfe6af4401aae5`  
		Last Modified: Fri, 16 Jun 2023 01:29:03 GMT  
		Size: 15.2 MB (15239860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa4be1a0221ca370894af24240ab41f02e9de16f9e2bcc3c291249e1a6f6e5b`  
		Last Modified: Fri, 16 Jun 2023 01:30:57 GMT  
		Size: 44.9 MB (44878070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9485255e1b5f7cd153d07a1b5898ee5e5bd85aa4a691daf554143ced7212c1`  
		Last Modified: Fri, 16 Jun 2023 01:30:50 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a7c708415525a81959edf16bc3d49f0f9a353a6ccbe62118f35a41d4badccb`  
		Last Modified: Fri, 16 Jun 2023 02:43:43 GMT  
		Size: 4.2 MB (4195564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef49861acb2439bd6a0a6f42a08da858a6dacef45c4b6b6d7c825973b22ee68`  
		Last Modified: Fri, 16 Jun 2023 02:43:42 GMT  
		Size: 4.2 KB (4227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184ca62e04698d0a2ce1cb95dba1910b5f5ac02f61355c24c5880a7c7be9eeb1`  
		Last Modified: Fri, 16 Jun 2023 02:43:43 GMT  
		Size: 3.5 KB (3468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9500fd7b0d4b665ed021c59c63e5b1dd2f1ad367bad3d01f7bc40900f851910`  
		Last Modified: Fri, 16 Jun 2023 02:43:54 GMT  
		Size: 218.3 MB (218328266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59dbadb77c53a247c461ee32ccfb2599ba7a1a573cd73de04c1f97630b61a67`  
		Last Modified: Fri, 16 Jun 2023 02:43:42 GMT  
		Size: 6.3 KB (6307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8-slim` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:1b4ea0e0e35837d0f6db13fb2a1e553d6a95adaff4852931281318d1f93d2ed2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.6 MB (311572971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:788806992a790f53caca77b9db76e2b2989ee188ed8ef3e767ba02d794c6b1da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:44:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:44:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:44:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:45:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:46:28 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 02:47:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:47:05 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:50:19 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 05:50:19 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:50:25 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 05:50:25 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 05:50:25 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:50:36 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 05:51:07 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 05:51:08 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 05:51:08 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:51:08 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:51:08 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:51:08 GMT
USER 8983
# Fri, 16 Jun 2023 05:51:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:51:09 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded85a30fdd137ed744a50296a089c18b7521b4a6423755763e7800084a35202`  
		Last Modified: Fri, 16 Jun 2023 02:49:42 GMT  
		Size: 16.3 MB (16269114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfc7474bf0993d4c615cd8ced7ac374026ba3ed62d57c6c3b883ddd60eeab1c`  
		Last Modified: Fri, 16 Jun 2023 02:51:23 GMT  
		Size: 45.0 MB (45009934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4224185bc45707d5ecf5e90b3d2f02b37a434000cac542530a00b3b48bfe3cc1`  
		Last Modified: Fri, 16 Jun 2023 02:51:18 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da95bc002c942fa9153e103b1a5d713d4d697a87cf89efc2dbabcf2f687582c9`  
		Last Modified: Fri, 16 Jun 2023 05:52:23 GMT  
		Size: 4.8 MB (4751007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea88f6087b1841d5b9307ee6b15a0d5181f2dfd7d72cf259b6324134d53ade6`  
		Last Modified: Fri, 16 Jun 2023 05:52:22 GMT  
		Size: 4.3 KB (4332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd91ceaa583a76bc85231b9ce41fd23fa35fb9256ee47d37ce5519525f1f4eab`  
		Last Modified: Fri, 16 Jun 2023 05:52:22 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed79fba284b4b35a82f34cdd8a083b228f925fe9d329c07e0f9d33c9607d2253`  
		Last Modified: Fri, 16 Jun 2023 05:52:30 GMT  
		Size: 218.3 MB (218328212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3106b45811e1338a0676a17f56cb843f09ca7f99f7780418d14da2e75efb0b`  
		Last Modified: Fri, 16 Jun 2023 05:52:22 GMT  
		Size: 6.3 KB (6309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8-slim` - linux; ppc64le

```console
$ docker pull solr@sha256:e5bf7de5f3a81916ba68d0803b2a20683c3f343526ac4504bf83ff58a3554e7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.2 MB (317172564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622e27233dfd4792c9d6f51e19e2c8549ad71521b3e68abd69f92eceb9ec6724`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:24 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:25 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:28 GMT
ADD file:0a2372ac4d43f0f4ada2b55dd0a359df73a828a9aa9426bfdd05a02b9c4b2bd9 in / 
# Mon, 05 Jun 2023 17:08:28 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:17:32 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:17:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:17:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:18:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:20:58 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 02:22:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:22:25 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 07:41:31 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 07:41:31 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 07:41:32 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 07:41:32 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 07:41:33 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 07:41:33 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 07:41:34 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 07:41:55 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 07:41:56 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 07:42:00 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 07:42:17 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 07:42:49 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 07:42:52 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 07:42:53 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 07:42:55 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 07:42:57 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 07:42:58 GMT
USER 8983
# Fri, 16 Jun 2023 07:42:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 07:42:59 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:1fbda4a01aa9e184a223c30ab58441354cde30fe3083bc1d8ca9f7823ab4fe68`  
		Last Modified: Fri, 16 Jun 2023 01:24:20 GMT  
		Size: 33.3 MB (33309776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb717f01d0b915280274134b467bc61cb1a7be1d9c6a9fe149dd3e9ab5d4d5`  
		Last Modified: Fri, 16 Jun 2023 02:26:38 GMT  
		Size: 17.6 MB (17648879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd6c33e350c331fd82a3898e4308740b9228a93a9bd1cfbf209b8ac158961d6`  
		Last Modified: Fri, 16 Jun 2023 02:29:11 GMT  
		Size: 42.1 MB (42093841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ce0cb194906f7f8bf1248463cbef057861d206d072004bad81d1784fdb4b54`  
		Last Modified: Fri, 16 Jun 2023 02:29:00 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17d3ac8d21a63094e82ec5c4dc8dfa1c0cbfd4a7108d667bbf3b154435fa7f5`  
		Last Modified: Fri, 16 Jun 2023 07:44:57 GMT  
		Size: 5.8 MB (5777612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d596f773882c647c8f31f469e949edc08d29108d6e9eb47e8c45fae8fe6b8720`  
		Last Modified: Fri, 16 Jun 2023 07:44:55 GMT  
		Size: 4.3 KB (4297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7413d7cf84cc22e166149d3b19012981e5bcf3d7de8c109d5331ed65b172585`  
		Last Modified: Fri, 16 Jun 2023 07:44:55 GMT  
		Size: 3.5 KB (3469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5dedd276de4704622c2f0ba1ccc9b716e2b2000dc8af1b59a94b4c3f7c66a3`  
		Last Modified: Fri, 16 Jun 2023 07:45:12 GMT  
		Size: 218.3 MB (218328223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba39db06026d8858274e3c4e59ed877a895145ee633b4585cc44b1f4c38115b`  
		Last Modified: Fri, 16 Jun 2023 07:44:55 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8-slim` - linux; s390x

```console
$ docker pull solr@sha256:3cb7e3eb537f722ef2d096a1cc9e90107d5a26a93eac004e2be96f7709fa7a7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.7 MB (306665402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc08946ca2b22de4fde16a15d59e3eb3989c0f8948b178b9440a9df20d36de60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:35 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:37 GMT
ADD file:44c66c03ba0afcc05de1b2078f83e8bfe04706b31491fcd3fdd93cfc88d5f06c in / 
# Thu, 13 Apr 2023 13:09:37 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:16:00 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:16:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:16:00 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:16:11 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:41:46 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:43:00 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:43:03 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:36:38 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 26 Apr 2023 20:36:38 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_VERSION=8.11.2
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:36:43 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 26 Apr 2023 20:36:44 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 26 Apr 2023 20:36:44 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:36:51 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 26 Apr 2023 20:37:07 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 26 Apr 2023 20:37:11 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 26 Apr 2023 20:37:11 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:37:12 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:37:12 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:37:12 GMT
USER 8983
# Wed, 26 Apr 2023 20:37:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:37:12 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:f11b609b1d63f2d37c0e3789823e7a7e62a078bddca7c46da8602655989c62d9`  
		Last Modified: Fri, 14 Apr 2023 09:38:39 GMT  
		Size: 27.0 MB (27016370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c307a57c5f07334cfab6db8f8324b0c9dff13121ec34d8db1d4a71e3529d4b5`  
		Last Modified: Tue, 18 Apr 2023 01:18:27 GMT  
		Size: 16.0 MB (16035272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f2464ae2b2cf26ad0951e353283a0faff6e21082c5b3ffc1ee96700cd352db8`  
		Last Modified: Wed, 26 Apr 2023 19:46:33 GMT  
		Size: 40.5 MB (40540743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2357373aba3b86e27f47b65c90b2c45aa55910d7a8e20ab95b0211c90ac0afc5`  
		Last Modified: Wed, 26 Apr 2023 19:46:28 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283aa23eb2725cd0f2f9e5627452bda5952b9f2b8279f3973cff4bc6bd8f2f8c`  
		Last Modified: Wed, 26 Apr 2023 20:38:26 GMT  
		Size: 4.7 MB (4730562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b9b134fa6b4ae6e10d35a150c618d122d72cb88c9c0def17080d179a2bc4fa`  
		Last Modified: Wed, 26 Apr 2023 20:38:25 GMT  
		Size: 4.3 KB (4333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b39ba054e26d24e3a1ea7e6e0fa808358921ad07e25bfe70ebde348e13891c`  
		Last Modified: Wed, 26 Apr 2023 20:38:25 GMT  
		Size: 3.5 KB (3468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a942f8f7937f22541141bb4ad17bd44e43cf1cbf39893673e50f572aa2f3fc27`  
		Last Modified: Wed, 26 Apr 2023 20:38:34 GMT  
		Size: 218.3 MB (218328187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3753012f9147597bbee82b53507c05d7009de3e3684021b64da90103d9d65c3f`  
		Last Modified: Wed, 26 Apr 2023 20:38:25 GMT  
		Size: 6.3 KB (6306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:8.11`

```console
$ docker pull solr@sha256:123ec0e30b444b5a6a02dc2435efa4c987d4ea56e59096e2b9ef4f4cec29cd4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `solr:8.11` - linux; amd64

```console
$ docker pull solr@sha256:7b77d4d3a0e9caf84e5e862e571bed8b9ca1331fc749d73f718d0eaeed6b46c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.9 MB (314902545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c927f6e7447da43ff7b242422647ceaa3fdd2f428714cd1c45eb7401037a3b7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:15:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:15:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:15:07 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:15:39 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:16:51 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 02:17:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:17:31 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:29:28 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 05:29:28 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:29:35 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 05:29:35 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 05:29:36 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:29:41 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 05:30:14 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 05:30:15 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 05:30:15 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:30:15 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:30:15 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:30:15 GMT
USER 8983
# Fri, 16 Jun 2023 05:30:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:30:15 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491508b827d83492c058d6e12e6ee1fe2f0e8328a6a5254f225537a15ef24bfe`  
		Last Modified: Fri, 16 Jun 2023 02:20:43 GMT  
		Size: 16.4 MB (16413378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1d6f5b86c355e0656c507178ce8f4719ba6d4640dd32454ae56a021577aff2`  
		Last Modified: Fri, 16 Jun 2023 02:22:39 GMT  
		Size: 46.7 MB (46664972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8c9ad9fc2c5ff99353581f54c02e5ccfc7a745f9d254b89b2a76ab4b5a1388`  
		Last Modified: Fri, 16 Jun 2023 02:22:33 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8875bfce5e356f6a6c69b048c0352efb474398130f74d3d4ba4dc7b9f442145b`  
		Last Modified: Fri, 16 Jun 2023 05:31:41 GMT  
		Size: 4.9 MB (4901233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7a509476958a6dae54a50468f11922b675ecc500508d78f8b6681279c296ba`  
		Last Modified: Fri, 16 Jun 2023 05:31:40 GMT  
		Size: 4.3 KB (4292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5463314ac566a3f0665b25ff19f588bb4c8b1b4018d6030b153925465b811b`  
		Last Modified: Fri, 16 Jun 2023 05:31:40 GMT  
		Size: 3.5 KB (3464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c63f7ff1fc39d233fb0b8d502c6c25e56f6a67d5c1c499de29b09fcb492250e`  
		Last Modified: Fri, 16 Jun 2023 05:31:50 GMT  
		Size: 218.3 MB (218328218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1ea8856e2cb8f18a8018967fcd79e03003b3f827d8a5d43ed6ee01d317403d`  
		Last Modified: Fri, 16 Jun 2023 05:31:40 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11` - linux; arm variant v7

```console
$ docker pull solr@sha256:0c813cc7f3ec53209e6a37ae486a6310e52a49ab3fd115534c89f1d16bb0741e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.2 MB (307245039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b3ba4de150bda0840a7845811dbde7ce970246384bb4da34c971c7750a6bdf6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:24:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 01:24:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 01:24:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 01:24:49 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:26:23 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 01:27:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 01:27:04 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 02:41:14 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 02:41:14 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 02:41:15 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 02:41:21 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 02:41:21 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 02:41:21 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 02:41:31 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 02:42:09 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 02:42:10 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 02:42:10 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 02:42:10 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 02:42:10 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 02:42:10 GMT
USER 8983
# Fri, 16 Jun 2023 02:42:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 02:42:10 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:2d97abfcf215d35e8a846b390350fea9f455676b41221360fe8782163a1c46bb`  
		Last Modified: Thu, 15 Jun 2023 03:47:54 GMT  
		Size: 24.6 MB (24589116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9495a3be9c2c6747ed337799b868bba61986a721c67a700acfe6af4401aae5`  
		Last Modified: Fri, 16 Jun 2023 01:29:03 GMT  
		Size: 15.2 MB (15239860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa4be1a0221ca370894af24240ab41f02e9de16f9e2bcc3c291249e1a6f6e5b`  
		Last Modified: Fri, 16 Jun 2023 01:30:57 GMT  
		Size: 44.9 MB (44878070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9485255e1b5f7cd153d07a1b5898ee5e5bd85aa4a691daf554143ced7212c1`  
		Last Modified: Fri, 16 Jun 2023 01:30:50 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a7c708415525a81959edf16bc3d49f0f9a353a6ccbe62118f35a41d4badccb`  
		Last Modified: Fri, 16 Jun 2023 02:43:43 GMT  
		Size: 4.2 MB (4195564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef49861acb2439bd6a0a6f42a08da858a6dacef45c4b6b6d7c825973b22ee68`  
		Last Modified: Fri, 16 Jun 2023 02:43:42 GMT  
		Size: 4.2 KB (4227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184ca62e04698d0a2ce1cb95dba1910b5f5ac02f61355c24c5880a7c7be9eeb1`  
		Last Modified: Fri, 16 Jun 2023 02:43:43 GMT  
		Size: 3.5 KB (3468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9500fd7b0d4b665ed021c59c63e5b1dd2f1ad367bad3d01f7bc40900f851910`  
		Last Modified: Fri, 16 Jun 2023 02:43:54 GMT  
		Size: 218.3 MB (218328266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59dbadb77c53a247c461ee32ccfb2599ba7a1a573cd73de04c1f97630b61a67`  
		Last Modified: Fri, 16 Jun 2023 02:43:42 GMT  
		Size: 6.3 KB (6307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:1b4ea0e0e35837d0f6db13fb2a1e553d6a95adaff4852931281318d1f93d2ed2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.6 MB (311572971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:788806992a790f53caca77b9db76e2b2989ee188ed8ef3e767ba02d794c6b1da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:44:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:44:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:44:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:45:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:46:28 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 02:47:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:47:05 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:50:19 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 05:50:19 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:50:25 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 05:50:25 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 05:50:25 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:50:36 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 05:51:07 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 05:51:08 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 05:51:08 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:51:08 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:51:08 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:51:08 GMT
USER 8983
# Fri, 16 Jun 2023 05:51:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:51:09 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded85a30fdd137ed744a50296a089c18b7521b4a6423755763e7800084a35202`  
		Last Modified: Fri, 16 Jun 2023 02:49:42 GMT  
		Size: 16.3 MB (16269114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfc7474bf0993d4c615cd8ced7ac374026ba3ed62d57c6c3b883ddd60eeab1c`  
		Last Modified: Fri, 16 Jun 2023 02:51:23 GMT  
		Size: 45.0 MB (45009934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4224185bc45707d5ecf5e90b3d2f02b37a434000cac542530a00b3b48bfe3cc1`  
		Last Modified: Fri, 16 Jun 2023 02:51:18 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da95bc002c942fa9153e103b1a5d713d4d697a87cf89efc2dbabcf2f687582c9`  
		Last Modified: Fri, 16 Jun 2023 05:52:23 GMT  
		Size: 4.8 MB (4751007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea88f6087b1841d5b9307ee6b15a0d5181f2dfd7d72cf259b6324134d53ade6`  
		Last Modified: Fri, 16 Jun 2023 05:52:22 GMT  
		Size: 4.3 KB (4332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd91ceaa583a76bc85231b9ce41fd23fa35fb9256ee47d37ce5519525f1f4eab`  
		Last Modified: Fri, 16 Jun 2023 05:52:22 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed79fba284b4b35a82f34cdd8a083b228f925fe9d329c07e0f9d33c9607d2253`  
		Last Modified: Fri, 16 Jun 2023 05:52:30 GMT  
		Size: 218.3 MB (218328212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3106b45811e1338a0676a17f56cb843f09ca7f99f7780418d14da2e75efb0b`  
		Last Modified: Fri, 16 Jun 2023 05:52:22 GMT  
		Size: 6.3 KB (6309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11` - linux; ppc64le

```console
$ docker pull solr@sha256:e5bf7de5f3a81916ba68d0803b2a20683c3f343526ac4504bf83ff58a3554e7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.2 MB (317172564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622e27233dfd4792c9d6f51e19e2c8549ad71521b3e68abd69f92eceb9ec6724`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:24 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:25 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:28 GMT
ADD file:0a2372ac4d43f0f4ada2b55dd0a359df73a828a9aa9426bfdd05a02b9c4b2bd9 in / 
# Mon, 05 Jun 2023 17:08:28 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:17:32 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:17:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:17:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:18:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:20:58 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 02:22:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:22:25 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 07:41:31 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 07:41:31 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 07:41:32 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 07:41:32 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 07:41:33 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 07:41:33 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 07:41:34 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 07:41:55 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 07:41:56 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 07:42:00 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 07:42:17 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 07:42:49 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 07:42:52 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 07:42:53 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 07:42:55 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 07:42:57 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 07:42:58 GMT
USER 8983
# Fri, 16 Jun 2023 07:42:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 07:42:59 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:1fbda4a01aa9e184a223c30ab58441354cde30fe3083bc1d8ca9f7823ab4fe68`  
		Last Modified: Fri, 16 Jun 2023 01:24:20 GMT  
		Size: 33.3 MB (33309776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb717f01d0b915280274134b467bc61cb1a7be1d9c6a9fe149dd3e9ab5d4d5`  
		Last Modified: Fri, 16 Jun 2023 02:26:38 GMT  
		Size: 17.6 MB (17648879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd6c33e350c331fd82a3898e4308740b9228a93a9bd1cfbf209b8ac158961d6`  
		Last Modified: Fri, 16 Jun 2023 02:29:11 GMT  
		Size: 42.1 MB (42093841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ce0cb194906f7f8bf1248463cbef057861d206d072004bad81d1784fdb4b54`  
		Last Modified: Fri, 16 Jun 2023 02:29:00 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17d3ac8d21a63094e82ec5c4dc8dfa1c0cbfd4a7108d667bbf3b154435fa7f5`  
		Last Modified: Fri, 16 Jun 2023 07:44:57 GMT  
		Size: 5.8 MB (5777612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d596f773882c647c8f31f469e949edc08d29108d6e9eb47e8c45fae8fe6b8720`  
		Last Modified: Fri, 16 Jun 2023 07:44:55 GMT  
		Size: 4.3 KB (4297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7413d7cf84cc22e166149d3b19012981e5bcf3d7de8c109d5331ed65b172585`  
		Last Modified: Fri, 16 Jun 2023 07:44:55 GMT  
		Size: 3.5 KB (3469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5dedd276de4704622c2f0ba1ccc9b716e2b2000dc8af1b59a94b4c3f7c66a3`  
		Last Modified: Fri, 16 Jun 2023 07:45:12 GMT  
		Size: 218.3 MB (218328223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba39db06026d8858274e3c4e59ed877a895145ee633b4585cc44b1f4c38115b`  
		Last Modified: Fri, 16 Jun 2023 07:44:55 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11` - linux; s390x

```console
$ docker pull solr@sha256:3cb7e3eb537f722ef2d096a1cc9e90107d5a26a93eac004e2be96f7709fa7a7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.7 MB (306665402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc08946ca2b22de4fde16a15d59e3eb3989c0f8948b178b9440a9df20d36de60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:35 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:37 GMT
ADD file:44c66c03ba0afcc05de1b2078f83e8bfe04706b31491fcd3fdd93cfc88d5f06c in / 
# Thu, 13 Apr 2023 13:09:37 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:16:00 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:16:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:16:00 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:16:11 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:41:46 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:43:00 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:43:03 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:36:38 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 26 Apr 2023 20:36:38 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_VERSION=8.11.2
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:36:43 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 26 Apr 2023 20:36:44 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 26 Apr 2023 20:36:44 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:36:51 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 26 Apr 2023 20:37:07 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 26 Apr 2023 20:37:11 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 26 Apr 2023 20:37:11 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:37:12 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:37:12 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:37:12 GMT
USER 8983
# Wed, 26 Apr 2023 20:37:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:37:12 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:f11b609b1d63f2d37c0e3789823e7a7e62a078bddca7c46da8602655989c62d9`  
		Last Modified: Fri, 14 Apr 2023 09:38:39 GMT  
		Size: 27.0 MB (27016370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c307a57c5f07334cfab6db8f8324b0c9dff13121ec34d8db1d4a71e3529d4b5`  
		Last Modified: Tue, 18 Apr 2023 01:18:27 GMT  
		Size: 16.0 MB (16035272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f2464ae2b2cf26ad0951e353283a0faff6e21082c5b3ffc1ee96700cd352db8`  
		Last Modified: Wed, 26 Apr 2023 19:46:33 GMT  
		Size: 40.5 MB (40540743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2357373aba3b86e27f47b65c90b2c45aa55910d7a8e20ab95b0211c90ac0afc5`  
		Last Modified: Wed, 26 Apr 2023 19:46:28 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283aa23eb2725cd0f2f9e5627452bda5952b9f2b8279f3973cff4bc6bd8f2f8c`  
		Last Modified: Wed, 26 Apr 2023 20:38:26 GMT  
		Size: 4.7 MB (4730562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b9b134fa6b4ae6e10d35a150c618d122d72cb88c9c0def17080d179a2bc4fa`  
		Last Modified: Wed, 26 Apr 2023 20:38:25 GMT  
		Size: 4.3 KB (4333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b39ba054e26d24e3a1ea7e6e0fa808358921ad07e25bfe70ebde348e13891c`  
		Last Modified: Wed, 26 Apr 2023 20:38:25 GMT  
		Size: 3.5 KB (3468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a942f8f7937f22541141bb4ad17bd44e43cf1cbf39893673e50f572aa2f3fc27`  
		Last Modified: Wed, 26 Apr 2023 20:38:34 GMT  
		Size: 218.3 MB (218328187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3753012f9147597bbee82b53507c05d7009de3e3684021b64da90103d9d65c3f`  
		Last Modified: Wed, 26 Apr 2023 20:38:25 GMT  
		Size: 6.3 KB (6306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:8.11-slim`

```console
$ docker pull solr@sha256:123ec0e30b444b5a6a02dc2435efa4c987d4ea56e59096e2b9ef4f4cec29cd4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `solr:8.11-slim` - linux; amd64

```console
$ docker pull solr@sha256:7b77d4d3a0e9caf84e5e862e571bed8b9ca1331fc749d73f718d0eaeed6b46c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.9 MB (314902545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c927f6e7447da43ff7b242422647ceaa3fdd2f428714cd1c45eb7401037a3b7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:15:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:15:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:15:07 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:15:39 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:16:51 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 02:17:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:17:31 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:29:28 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 05:29:28 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:29:35 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 05:29:35 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 05:29:36 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:29:41 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 05:30:14 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 05:30:15 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 05:30:15 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:30:15 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:30:15 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:30:15 GMT
USER 8983
# Fri, 16 Jun 2023 05:30:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:30:15 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491508b827d83492c058d6e12e6ee1fe2f0e8328a6a5254f225537a15ef24bfe`  
		Last Modified: Fri, 16 Jun 2023 02:20:43 GMT  
		Size: 16.4 MB (16413378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1d6f5b86c355e0656c507178ce8f4719ba6d4640dd32454ae56a021577aff2`  
		Last Modified: Fri, 16 Jun 2023 02:22:39 GMT  
		Size: 46.7 MB (46664972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8c9ad9fc2c5ff99353581f54c02e5ccfc7a745f9d254b89b2a76ab4b5a1388`  
		Last Modified: Fri, 16 Jun 2023 02:22:33 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8875bfce5e356f6a6c69b048c0352efb474398130f74d3d4ba4dc7b9f442145b`  
		Last Modified: Fri, 16 Jun 2023 05:31:41 GMT  
		Size: 4.9 MB (4901233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7a509476958a6dae54a50468f11922b675ecc500508d78f8b6681279c296ba`  
		Last Modified: Fri, 16 Jun 2023 05:31:40 GMT  
		Size: 4.3 KB (4292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5463314ac566a3f0665b25ff19f588bb4c8b1b4018d6030b153925465b811b`  
		Last Modified: Fri, 16 Jun 2023 05:31:40 GMT  
		Size: 3.5 KB (3464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c63f7ff1fc39d233fb0b8d502c6c25e56f6a67d5c1c499de29b09fcb492250e`  
		Last Modified: Fri, 16 Jun 2023 05:31:50 GMT  
		Size: 218.3 MB (218328218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1ea8856e2cb8f18a8018967fcd79e03003b3f827d8a5d43ed6ee01d317403d`  
		Last Modified: Fri, 16 Jun 2023 05:31:40 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11-slim` - linux; arm variant v7

```console
$ docker pull solr@sha256:0c813cc7f3ec53209e6a37ae486a6310e52a49ab3fd115534c89f1d16bb0741e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.2 MB (307245039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b3ba4de150bda0840a7845811dbde7ce970246384bb4da34c971c7750a6bdf6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:24:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 01:24:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 01:24:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 01:24:49 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:26:23 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 01:27:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 01:27:04 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 02:41:14 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 02:41:14 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 02:41:15 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 02:41:21 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 02:41:21 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 02:41:21 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 02:41:31 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 02:42:09 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 02:42:10 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 02:42:10 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 02:42:10 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 02:42:10 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 02:42:10 GMT
USER 8983
# Fri, 16 Jun 2023 02:42:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 02:42:10 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:2d97abfcf215d35e8a846b390350fea9f455676b41221360fe8782163a1c46bb`  
		Last Modified: Thu, 15 Jun 2023 03:47:54 GMT  
		Size: 24.6 MB (24589116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9495a3be9c2c6747ed337799b868bba61986a721c67a700acfe6af4401aae5`  
		Last Modified: Fri, 16 Jun 2023 01:29:03 GMT  
		Size: 15.2 MB (15239860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa4be1a0221ca370894af24240ab41f02e9de16f9e2bcc3c291249e1a6f6e5b`  
		Last Modified: Fri, 16 Jun 2023 01:30:57 GMT  
		Size: 44.9 MB (44878070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9485255e1b5f7cd153d07a1b5898ee5e5bd85aa4a691daf554143ced7212c1`  
		Last Modified: Fri, 16 Jun 2023 01:30:50 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a7c708415525a81959edf16bc3d49f0f9a353a6ccbe62118f35a41d4badccb`  
		Last Modified: Fri, 16 Jun 2023 02:43:43 GMT  
		Size: 4.2 MB (4195564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef49861acb2439bd6a0a6f42a08da858a6dacef45c4b6b6d7c825973b22ee68`  
		Last Modified: Fri, 16 Jun 2023 02:43:42 GMT  
		Size: 4.2 KB (4227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184ca62e04698d0a2ce1cb95dba1910b5f5ac02f61355c24c5880a7c7be9eeb1`  
		Last Modified: Fri, 16 Jun 2023 02:43:43 GMT  
		Size: 3.5 KB (3468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9500fd7b0d4b665ed021c59c63e5b1dd2f1ad367bad3d01f7bc40900f851910`  
		Last Modified: Fri, 16 Jun 2023 02:43:54 GMT  
		Size: 218.3 MB (218328266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59dbadb77c53a247c461ee32ccfb2599ba7a1a573cd73de04c1f97630b61a67`  
		Last Modified: Fri, 16 Jun 2023 02:43:42 GMT  
		Size: 6.3 KB (6307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11-slim` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:1b4ea0e0e35837d0f6db13fb2a1e553d6a95adaff4852931281318d1f93d2ed2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.6 MB (311572971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:788806992a790f53caca77b9db76e2b2989ee188ed8ef3e767ba02d794c6b1da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:44:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:44:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:44:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:45:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:46:28 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 02:47:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:47:05 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:50:19 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 05:50:19 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:50:25 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 05:50:25 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 05:50:25 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:50:36 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 05:51:07 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 05:51:08 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 05:51:08 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:51:08 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:51:08 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:51:08 GMT
USER 8983
# Fri, 16 Jun 2023 05:51:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:51:09 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded85a30fdd137ed744a50296a089c18b7521b4a6423755763e7800084a35202`  
		Last Modified: Fri, 16 Jun 2023 02:49:42 GMT  
		Size: 16.3 MB (16269114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfc7474bf0993d4c615cd8ced7ac374026ba3ed62d57c6c3b883ddd60eeab1c`  
		Last Modified: Fri, 16 Jun 2023 02:51:23 GMT  
		Size: 45.0 MB (45009934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4224185bc45707d5ecf5e90b3d2f02b37a434000cac542530a00b3b48bfe3cc1`  
		Last Modified: Fri, 16 Jun 2023 02:51:18 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da95bc002c942fa9153e103b1a5d713d4d697a87cf89efc2dbabcf2f687582c9`  
		Last Modified: Fri, 16 Jun 2023 05:52:23 GMT  
		Size: 4.8 MB (4751007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea88f6087b1841d5b9307ee6b15a0d5181f2dfd7d72cf259b6324134d53ade6`  
		Last Modified: Fri, 16 Jun 2023 05:52:22 GMT  
		Size: 4.3 KB (4332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd91ceaa583a76bc85231b9ce41fd23fa35fb9256ee47d37ce5519525f1f4eab`  
		Last Modified: Fri, 16 Jun 2023 05:52:22 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed79fba284b4b35a82f34cdd8a083b228f925fe9d329c07e0f9d33c9607d2253`  
		Last Modified: Fri, 16 Jun 2023 05:52:30 GMT  
		Size: 218.3 MB (218328212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3106b45811e1338a0676a17f56cb843f09ca7f99f7780418d14da2e75efb0b`  
		Last Modified: Fri, 16 Jun 2023 05:52:22 GMT  
		Size: 6.3 KB (6309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11-slim` - linux; ppc64le

```console
$ docker pull solr@sha256:e5bf7de5f3a81916ba68d0803b2a20683c3f343526ac4504bf83ff58a3554e7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.2 MB (317172564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622e27233dfd4792c9d6f51e19e2c8549ad71521b3e68abd69f92eceb9ec6724`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:24 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:25 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:28 GMT
ADD file:0a2372ac4d43f0f4ada2b55dd0a359df73a828a9aa9426bfdd05a02b9c4b2bd9 in / 
# Mon, 05 Jun 2023 17:08:28 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:17:32 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:17:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:17:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:18:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:20:58 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 02:22:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:22:25 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 07:41:31 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 07:41:31 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 07:41:32 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 07:41:32 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 07:41:33 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 07:41:33 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 07:41:34 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 07:41:55 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 07:41:56 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 07:42:00 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 07:42:17 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 07:42:49 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 07:42:52 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 07:42:53 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 07:42:55 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 07:42:57 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 07:42:58 GMT
USER 8983
# Fri, 16 Jun 2023 07:42:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 07:42:59 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:1fbda4a01aa9e184a223c30ab58441354cde30fe3083bc1d8ca9f7823ab4fe68`  
		Last Modified: Fri, 16 Jun 2023 01:24:20 GMT  
		Size: 33.3 MB (33309776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb717f01d0b915280274134b467bc61cb1a7be1d9c6a9fe149dd3e9ab5d4d5`  
		Last Modified: Fri, 16 Jun 2023 02:26:38 GMT  
		Size: 17.6 MB (17648879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd6c33e350c331fd82a3898e4308740b9228a93a9bd1cfbf209b8ac158961d6`  
		Last Modified: Fri, 16 Jun 2023 02:29:11 GMT  
		Size: 42.1 MB (42093841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ce0cb194906f7f8bf1248463cbef057861d206d072004bad81d1784fdb4b54`  
		Last Modified: Fri, 16 Jun 2023 02:29:00 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17d3ac8d21a63094e82ec5c4dc8dfa1c0cbfd4a7108d667bbf3b154435fa7f5`  
		Last Modified: Fri, 16 Jun 2023 07:44:57 GMT  
		Size: 5.8 MB (5777612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d596f773882c647c8f31f469e949edc08d29108d6e9eb47e8c45fae8fe6b8720`  
		Last Modified: Fri, 16 Jun 2023 07:44:55 GMT  
		Size: 4.3 KB (4297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7413d7cf84cc22e166149d3b19012981e5bcf3d7de8c109d5331ed65b172585`  
		Last Modified: Fri, 16 Jun 2023 07:44:55 GMT  
		Size: 3.5 KB (3469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5dedd276de4704622c2f0ba1ccc9b716e2b2000dc8af1b59a94b4c3f7c66a3`  
		Last Modified: Fri, 16 Jun 2023 07:45:12 GMT  
		Size: 218.3 MB (218328223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba39db06026d8858274e3c4e59ed877a895145ee633b4585cc44b1f4c38115b`  
		Last Modified: Fri, 16 Jun 2023 07:44:55 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11-slim` - linux; s390x

```console
$ docker pull solr@sha256:3cb7e3eb537f722ef2d096a1cc9e90107d5a26a93eac004e2be96f7709fa7a7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.7 MB (306665402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc08946ca2b22de4fde16a15d59e3eb3989c0f8948b178b9440a9df20d36de60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:35 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:37 GMT
ADD file:44c66c03ba0afcc05de1b2078f83e8bfe04706b31491fcd3fdd93cfc88d5f06c in / 
# Thu, 13 Apr 2023 13:09:37 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:16:00 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:16:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:16:00 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:16:11 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:41:46 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:43:00 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:43:03 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:36:38 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 26 Apr 2023 20:36:38 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_VERSION=8.11.2
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:36:43 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 26 Apr 2023 20:36:44 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 26 Apr 2023 20:36:44 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:36:51 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 26 Apr 2023 20:37:07 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 26 Apr 2023 20:37:11 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 26 Apr 2023 20:37:11 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:37:12 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:37:12 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:37:12 GMT
USER 8983
# Wed, 26 Apr 2023 20:37:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:37:12 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:f11b609b1d63f2d37c0e3789823e7a7e62a078bddca7c46da8602655989c62d9`  
		Last Modified: Fri, 14 Apr 2023 09:38:39 GMT  
		Size: 27.0 MB (27016370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c307a57c5f07334cfab6db8f8324b0c9dff13121ec34d8db1d4a71e3529d4b5`  
		Last Modified: Tue, 18 Apr 2023 01:18:27 GMT  
		Size: 16.0 MB (16035272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f2464ae2b2cf26ad0951e353283a0faff6e21082c5b3ffc1ee96700cd352db8`  
		Last Modified: Wed, 26 Apr 2023 19:46:33 GMT  
		Size: 40.5 MB (40540743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2357373aba3b86e27f47b65c90b2c45aa55910d7a8e20ab95b0211c90ac0afc5`  
		Last Modified: Wed, 26 Apr 2023 19:46:28 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283aa23eb2725cd0f2f9e5627452bda5952b9f2b8279f3973cff4bc6bd8f2f8c`  
		Last Modified: Wed, 26 Apr 2023 20:38:26 GMT  
		Size: 4.7 MB (4730562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b9b134fa6b4ae6e10d35a150c618d122d72cb88c9c0def17080d179a2bc4fa`  
		Last Modified: Wed, 26 Apr 2023 20:38:25 GMT  
		Size: 4.3 KB (4333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b39ba054e26d24e3a1ea7e6e0fa808358921ad07e25bfe70ebde348e13891c`  
		Last Modified: Wed, 26 Apr 2023 20:38:25 GMT  
		Size: 3.5 KB (3468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a942f8f7937f22541141bb4ad17bd44e43cf1cbf39893673e50f572aa2f3fc27`  
		Last Modified: Wed, 26 Apr 2023 20:38:34 GMT  
		Size: 218.3 MB (218328187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3753012f9147597bbee82b53507c05d7009de3e3684021b64da90103d9d65c3f`  
		Last Modified: Wed, 26 Apr 2023 20:38:25 GMT  
		Size: 6.3 KB (6306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:8.11.2`

```console
$ docker pull solr@sha256:123ec0e30b444b5a6a02dc2435efa4c987d4ea56e59096e2b9ef4f4cec29cd4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `solr:8.11.2` - linux; amd64

```console
$ docker pull solr@sha256:7b77d4d3a0e9caf84e5e862e571bed8b9ca1331fc749d73f718d0eaeed6b46c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.9 MB (314902545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c927f6e7447da43ff7b242422647ceaa3fdd2f428714cd1c45eb7401037a3b7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:15:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:15:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:15:07 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:15:39 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:16:51 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 02:17:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:17:31 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:29:28 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 05:29:28 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:29:35 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 05:29:35 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 05:29:36 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:29:41 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 05:30:14 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 05:30:15 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 05:30:15 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:30:15 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:30:15 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:30:15 GMT
USER 8983
# Fri, 16 Jun 2023 05:30:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:30:15 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491508b827d83492c058d6e12e6ee1fe2f0e8328a6a5254f225537a15ef24bfe`  
		Last Modified: Fri, 16 Jun 2023 02:20:43 GMT  
		Size: 16.4 MB (16413378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1d6f5b86c355e0656c507178ce8f4719ba6d4640dd32454ae56a021577aff2`  
		Last Modified: Fri, 16 Jun 2023 02:22:39 GMT  
		Size: 46.7 MB (46664972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8c9ad9fc2c5ff99353581f54c02e5ccfc7a745f9d254b89b2a76ab4b5a1388`  
		Last Modified: Fri, 16 Jun 2023 02:22:33 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8875bfce5e356f6a6c69b048c0352efb474398130f74d3d4ba4dc7b9f442145b`  
		Last Modified: Fri, 16 Jun 2023 05:31:41 GMT  
		Size: 4.9 MB (4901233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7a509476958a6dae54a50468f11922b675ecc500508d78f8b6681279c296ba`  
		Last Modified: Fri, 16 Jun 2023 05:31:40 GMT  
		Size: 4.3 KB (4292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5463314ac566a3f0665b25ff19f588bb4c8b1b4018d6030b153925465b811b`  
		Last Modified: Fri, 16 Jun 2023 05:31:40 GMT  
		Size: 3.5 KB (3464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c63f7ff1fc39d233fb0b8d502c6c25e56f6a67d5c1c499de29b09fcb492250e`  
		Last Modified: Fri, 16 Jun 2023 05:31:50 GMT  
		Size: 218.3 MB (218328218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1ea8856e2cb8f18a8018967fcd79e03003b3f827d8a5d43ed6ee01d317403d`  
		Last Modified: Fri, 16 Jun 2023 05:31:40 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11.2` - linux; arm variant v7

```console
$ docker pull solr@sha256:0c813cc7f3ec53209e6a37ae486a6310e52a49ab3fd115534c89f1d16bb0741e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.2 MB (307245039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b3ba4de150bda0840a7845811dbde7ce970246384bb4da34c971c7750a6bdf6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:24:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 01:24:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 01:24:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 01:24:49 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:26:23 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 01:27:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 01:27:04 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 02:41:14 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 02:41:14 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 02:41:15 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 02:41:21 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 02:41:21 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 02:41:21 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 02:41:31 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 02:42:09 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 02:42:10 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 02:42:10 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 02:42:10 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 02:42:10 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 02:42:10 GMT
USER 8983
# Fri, 16 Jun 2023 02:42:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 02:42:10 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:2d97abfcf215d35e8a846b390350fea9f455676b41221360fe8782163a1c46bb`  
		Last Modified: Thu, 15 Jun 2023 03:47:54 GMT  
		Size: 24.6 MB (24589116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9495a3be9c2c6747ed337799b868bba61986a721c67a700acfe6af4401aae5`  
		Last Modified: Fri, 16 Jun 2023 01:29:03 GMT  
		Size: 15.2 MB (15239860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa4be1a0221ca370894af24240ab41f02e9de16f9e2bcc3c291249e1a6f6e5b`  
		Last Modified: Fri, 16 Jun 2023 01:30:57 GMT  
		Size: 44.9 MB (44878070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9485255e1b5f7cd153d07a1b5898ee5e5bd85aa4a691daf554143ced7212c1`  
		Last Modified: Fri, 16 Jun 2023 01:30:50 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a7c708415525a81959edf16bc3d49f0f9a353a6ccbe62118f35a41d4badccb`  
		Last Modified: Fri, 16 Jun 2023 02:43:43 GMT  
		Size: 4.2 MB (4195564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef49861acb2439bd6a0a6f42a08da858a6dacef45c4b6b6d7c825973b22ee68`  
		Last Modified: Fri, 16 Jun 2023 02:43:42 GMT  
		Size: 4.2 KB (4227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184ca62e04698d0a2ce1cb95dba1910b5f5ac02f61355c24c5880a7c7be9eeb1`  
		Last Modified: Fri, 16 Jun 2023 02:43:43 GMT  
		Size: 3.5 KB (3468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9500fd7b0d4b665ed021c59c63e5b1dd2f1ad367bad3d01f7bc40900f851910`  
		Last Modified: Fri, 16 Jun 2023 02:43:54 GMT  
		Size: 218.3 MB (218328266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59dbadb77c53a247c461ee32ccfb2599ba7a1a573cd73de04c1f97630b61a67`  
		Last Modified: Fri, 16 Jun 2023 02:43:42 GMT  
		Size: 6.3 KB (6307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11.2` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:1b4ea0e0e35837d0f6db13fb2a1e553d6a95adaff4852931281318d1f93d2ed2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.6 MB (311572971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:788806992a790f53caca77b9db76e2b2989ee188ed8ef3e767ba02d794c6b1da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:44:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:44:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:44:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:45:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:46:28 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 02:47:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:47:05 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:50:19 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 05:50:19 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:50:25 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 05:50:25 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 05:50:25 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:50:36 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 05:51:07 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 05:51:08 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 05:51:08 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:51:08 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:51:08 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:51:08 GMT
USER 8983
# Fri, 16 Jun 2023 05:51:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:51:09 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded85a30fdd137ed744a50296a089c18b7521b4a6423755763e7800084a35202`  
		Last Modified: Fri, 16 Jun 2023 02:49:42 GMT  
		Size: 16.3 MB (16269114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfc7474bf0993d4c615cd8ced7ac374026ba3ed62d57c6c3b883ddd60eeab1c`  
		Last Modified: Fri, 16 Jun 2023 02:51:23 GMT  
		Size: 45.0 MB (45009934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4224185bc45707d5ecf5e90b3d2f02b37a434000cac542530a00b3b48bfe3cc1`  
		Last Modified: Fri, 16 Jun 2023 02:51:18 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da95bc002c942fa9153e103b1a5d713d4d697a87cf89efc2dbabcf2f687582c9`  
		Last Modified: Fri, 16 Jun 2023 05:52:23 GMT  
		Size: 4.8 MB (4751007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea88f6087b1841d5b9307ee6b15a0d5181f2dfd7d72cf259b6324134d53ade6`  
		Last Modified: Fri, 16 Jun 2023 05:52:22 GMT  
		Size: 4.3 KB (4332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd91ceaa583a76bc85231b9ce41fd23fa35fb9256ee47d37ce5519525f1f4eab`  
		Last Modified: Fri, 16 Jun 2023 05:52:22 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed79fba284b4b35a82f34cdd8a083b228f925fe9d329c07e0f9d33c9607d2253`  
		Last Modified: Fri, 16 Jun 2023 05:52:30 GMT  
		Size: 218.3 MB (218328212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3106b45811e1338a0676a17f56cb843f09ca7f99f7780418d14da2e75efb0b`  
		Last Modified: Fri, 16 Jun 2023 05:52:22 GMT  
		Size: 6.3 KB (6309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11.2` - linux; ppc64le

```console
$ docker pull solr@sha256:e5bf7de5f3a81916ba68d0803b2a20683c3f343526ac4504bf83ff58a3554e7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.2 MB (317172564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622e27233dfd4792c9d6f51e19e2c8549ad71521b3e68abd69f92eceb9ec6724`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:24 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:25 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:28 GMT
ADD file:0a2372ac4d43f0f4ada2b55dd0a359df73a828a9aa9426bfdd05a02b9c4b2bd9 in / 
# Mon, 05 Jun 2023 17:08:28 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:17:32 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:17:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:17:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:18:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:20:58 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 02:22:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:22:25 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 07:41:31 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 07:41:31 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 07:41:32 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 07:41:32 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 07:41:33 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 07:41:33 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 07:41:34 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 07:41:55 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 07:41:56 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 07:42:00 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 07:42:17 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 07:42:49 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 07:42:52 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 07:42:53 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 07:42:55 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 07:42:57 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 07:42:58 GMT
USER 8983
# Fri, 16 Jun 2023 07:42:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 07:42:59 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:1fbda4a01aa9e184a223c30ab58441354cde30fe3083bc1d8ca9f7823ab4fe68`  
		Last Modified: Fri, 16 Jun 2023 01:24:20 GMT  
		Size: 33.3 MB (33309776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb717f01d0b915280274134b467bc61cb1a7be1d9c6a9fe149dd3e9ab5d4d5`  
		Last Modified: Fri, 16 Jun 2023 02:26:38 GMT  
		Size: 17.6 MB (17648879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd6c33e350c331fd82a3898e4308740b9228a93a9bd1cfbf209b8ac158961d6`  
		Last Modified: Fri, 16 Jun 2023 02:29:11 GMT  
		Size: 42.1 MB (42093841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ce0cb194906f7f8bf1248463cbef057861d206d072004bad81d1784fdb4b54`  
		Last Modified: Fri, 16 Jun 2023 02:29:00 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17d3ac8d21a63094e82ec5c4dc8dfa1c0cbfd4a7108d667bbf3b154435fa7f5`  
		Last Modified: Fri, 16 Jun 2023 07:44:57 GMT  
		Size: 5.8 MB (5777612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d596f773882c647c8f31f469e949edc08d29108d6e9eb47e8c45fae8fe6b8720`  
		Last Modified: Fri, 16 Jun 2023 07:44:55 GMT  
		Size: 4.3 KB (4297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7413d7cf84cc22e166149d3b19012981e5bcf3d7de8c109d5331ed65b172585`  
		Last Modified: Fri, 16 Jun 2023 07:44:55 GMT  
		Size: 3.5 KB (3469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5dedd276de4704622c2f0ba1ccc9b716e2b2000dc8af1b59a94b4c3f7c66a3`  
		Last Modified: Fri, 16 Jun 2023 07:45:12 GMT  
		Size: 218.3 MB (218328223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba39db06026d8858274e3c4e59ed877a895145ee633b4585cc44b1f4c38115b`  
		Last Modified: Fri, 16 Jun 2023 07:44:55 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11.2` - linux; s390x

```console
$ docker pull solr@sha256:3cb7e3eb537f722ef2d096a1cc9e90107d5a26a93eac004e2be96f7709fa7a7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.7 MB (306665402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc08946ca2b22de4fde16a15d59e3eb3989c0f8948b178b9440a9df20d36de60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:35 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:37 GMT
ADD file:44c66c03ba0afcc05de1b2078f83e8bfe04706b31491fcd3fdd93cfc88d5f06c in / 
# Thu, 13 Apr 2023 13:09:37 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:16:00 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:16:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:16:00 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:16:11 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:41:46 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:43:00 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:43:03 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:36:38 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 26 Apr 2023 20:36:38 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_VERSION=8.11.2
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:36:43 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 26 Apr 2023 20:36:44 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 26 Apr 2023 20:36:44 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:36:51 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 26 Apr 2023 20:37:07 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 26 Apr 2023 20:37:11 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 26 Apr 2023 20:37:11 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:37:12 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:37:12 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:37:12 GMT
USER 8983
# Wed, 26 Apr 2023 20:37:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:37:12 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:f11b609b1d63f2d37c0e3789823e7a7e62a078bddca7c46da8602655989c62d9`  
		Last Modified: Fri, 14 Apr 2023 09:38:39 GMT  
		Size: 27.0 MB (27016370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c307a57c5f07334cfab6db8f8324b0c9dff13121ec34d8db1d4a71e3529d4b5`  
		Last Modified: Tue, 18 Apr 2023 01:18:27 GMT  
		Size: 16.0 MB (16035272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f2464ae2b2cf26ad0951e353283a0faff6e21082c5b3ffc1ee96700cd352db8`  
		Last Modified: Wed, 26 Apr 2023 19:46:33 GMT  
		Size: 40.5 MB (40540743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2357373aba3b86e27f47b65c90b2c45aa55910d7a8e20ab95b0211c90ac0afc5`  
		Last Modified: Wed, 26 Apr 2023 19:46:28 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283aa23eb2725cd0f2f9e5627452bda5952b9f2b8279f3973cff4bc6bd8f2f8c`  
		Last Modified: Wed, 26 Apr 2023 20:38:26 GMT  
		Size: 4.7 MB (4730562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b9b134fa6b4ae6e10d35a150c618d122d72cb88c9c0def17080d179a2bc4fa`  
		Last Modified: Wed, 26 Apr 2023 20:38:25 GMT  
		Size: 4.3 KB (4333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b39ba054e26d24e3a1ea7e6e0fa808358921ad07e25bfe70ebde348e13891c`  
		Last Modified: Wed, 26 Apr 2023 20:38:25 GMT  
		Size: 3.5 KB (3468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a942f8f7937f22541141bb4ad17bd44e43cf1cbf39893673e50f572aa2f3fc27`  
		Last Modified: Wed, 26 Apr 2023 20:38:34 GMT  
		Size: 218.3 MB (218328187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3753012f9147597bbee82b53507c05d7009de3e3684021b64da90103d9d65c3f`  
		Last Modified: Wed, 26 Apr 2023 20:38:25 GMT  
		Size: 6.3 KB (6306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:8.11.2-slim`

```console
$ docker pull solr@sha256:123ec0e30b444b5a6a02dc2435efa4c987d4ea56e59096e2b9ef4f4cec29cd4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `solr:8.11.2-slim` - linux; amd64

```console
$ docker pull solr@sha256:7b77d4d3a0e9caf84e5e862e571bed8b9ca1331fc749d73f718d0eaeed6b46c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.9 MB (314902545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c927f6e7447da43ff7b242422647ceaa3fdd2f428714cd1c45eb7401037a3b7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:15:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:15:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:15:07 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:15:39 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:16:51 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 02:17:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:17:31 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:29:28 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 05:29:28 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:29:28 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:29:35 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 05:29:35 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 05:29:36 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:29:41 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 05:30:14 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 05:30:15 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 05:30:15 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:30:15 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:30:15 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:30:15 GMT
USER 8983
# Fri, 16 Jun 2023 05:30:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:30:15 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491508b827d83492c058d6e12e6ee1fe2f0e8328a6a5254f225537a15ef24bfe`  
		Last Modified: Fri, 16 Jun 2023 02:20:43 GMT  
		Size: 16.4 MB (16413378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1d6f5b86c355e0656c507178ce8f4719ba6d4640dd32454ae56a021577aff2`  
		Last Modified: Fri, 16 Jun 2023 02:22:39 GMT  
		Size: 46.7 MB (46664972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8c9ad9fc2c5ff99353581f54c02e5ccfc7a745f9d254b89b2a76ab4b5a1388`  
		Last Modified: Fri, 16 Jun 2023 02:22:33 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8875bfce5e356f6a6c69b048c0352efb474398130f74d3d4ba4dc7b9f442145b`  
		Last Modified: Fri, 16 Jun 2023 05:31:41 GMT  
		Size: 4.9 MB (4901233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7a509476958a6dae54a50468f11922b675ecc500508d78f8b6681279c296ba`  
		Last Modified: Fri, 16 Jun 2023 05:31:40 GMT  
		Size: 4.3 KB (4292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5463314ac566a3f0665b25ff19f588bb4c8b1b4018d6030b153925465b811b`  
		Last Modified: Fri, 16 Jun 2023 05:31:40 GMT  
		Size: 3.5 KB (3464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c63f7ff1fc39d233fb0b8d502c6c25e56f6a67d5c1c499de29b09fcb492250e`  
		Last Modified: Fri, 16 Jun 2023 05:31:50 GMT  
		Size: 218.3 MB (218328218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1ea8856e2cb8f18a8018967fcd79e03003b3f827d8a5d43ed6ee01d317403d`  
		Last Modified: Fri, 16 Jun 2023 05:31:40 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11.2-slim` - linux; arm variant v7

```console
$ docker pull solr@sha256:0c813cc7f3ec53209e6a37ae486a6310e52a49ab3fd115534c89f1d16bb0741e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.2 MB (307245039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b3ba4de150bda0840a7845811dbde7ce970246384bb4da34c971c7750a6bdf6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:24:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 01:24:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 01:24:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 01:24:49 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:26:23 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 01:27:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 01:27:04 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 02:41:14 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 02:41:14 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 02:41:14 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 02:41:15 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 02:41:21 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 02:41:21 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 02:41:21 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 02:41:31 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 02:42:09 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 02:42:10 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 02:42:10 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 02:42:10 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 02:42:10 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 02:42:10 GMT
USER 8983
# Fri, 16 Jun 2023 02:42:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 02:42:10 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:2d97abfcf215d35e8a846b390350fea9f455676b41221360fe8782163a1c46bb`  
		Last Modified: Thu, 15 Jun 2023 03:47:54 GMT  
		Size: 24.6 MB (24589116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9495a3be9c2c6747ed337799b868bba61986a721c67a700acfe6af4401aae5`  
		Last Modified: Fri, 16 Jun 2023 01:29:03 GMT  
		Size: 15.2 MB (15239860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa4be1a0221ca370894af24240ab41f02e9de16f9e2bcc3c291249e1a6f6e5b`  
		Last Modified: Fri, 16 Jun 2023 01:30:57 GMT  
		Size: 44.9 MB (44878070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9485255e1b5f7cd153d07a1b5898ee5e5bd85aa4a691daf554143ced7212c1`  
		Last Modified: Fri, 16 Jun 2023 01:30:50 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a7c708415525a81959edf16bc3d49f0f9a353a6ccbe62118f35a41d4badccb`  
		Last Modified: Fri, 16 Jun 2023 02:43:43 GMT  
		Size: 4.2 MB (4195564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef49861acb2439bd6a0a6f42a08da858a6dacef45c4b6b6d7c825973b22ee68`  
		Last Modified: Fri, 16 Jun 2023 02:43:42 GMT  
		Size: 4.2 KB (4227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184ca62e04698d0a2ce1cb95dba1910b5f5ac02f61355c24c5880a7c7be9eeb1`  
		Last Modified: Fri, 16 Jun 2023 02:43:43 GMT  
		Size: 3.5 KB (3468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9500fd7b0d4b665ed021c59c63e5b1dd2f1ad367bad3d01f7bc40900f851910`  
		Last Modified: Fri, 16 Jun 2023 02:43:54 GMT  
		Size: 218.3 MB (218328266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59dbadb77c53a247c461ee32ccfb2599ba7a1a573cd73de04c1f97630b61a67`  
		Last Modified: Fri, 16 Jun 2023 02:43:42 GMT  
		Size: 6.3 KB (6307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11.2-slim` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:1b4ea0e0e35837d0f6db13fb2a1e553d6a95adaff4852931281318d1f93d2ed2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.6 MB (311572971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:788806992a790f53caca77b9db76e2b2989ee188ed8ef3e767ba02d794c6b1da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:44:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:44:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:44:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:45:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:46:28 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 02:47:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:47:05 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:50:19 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 05:50:19 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:50:19 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:50:25 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 05:50:25 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 05:50:25 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:50:36 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 05:51:07 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 05:51:08 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 05:51:08 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:51:08 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:51:08 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:51:08 GMT
USER 8983
# Fri, 16 Jun 2023 05:51:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:51:09 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded85a30fdd137ed744a50296a089c18b7521b4a6423755763e7800084a35202`  
		Last Modified: Fri, 16 Jun 2023 02:49:42 GMT  
		Size: 16.3 MB (16269114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfc7474bf0993d4c615cd8ced7ac374026ba3ed62d57c6c3b883ddd60eeab1c`  
		Last Modified: Fri, 16 Jun 2023 02:51:23 GMT  
		Size: 45.0 MB (45009934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4224185bc45707d5ecf5e90b3d2f02b37a434000cac542530a00b3b48bfe3cc1`  
		Last Modified: Fri, 16 Jun 2023 02:51:18 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da95bc002c942fa9153e103b1a5d713d4d697a87cf89efc2dbabcf2f687582c9`  
		Last Modified: Fri, 16 Jun 2023 05:52:23 GMT  
		Size: 4.8 MB (4751007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea88f6087b1841d5b9307ee6b15a0d5181f2dfd7d72cf259b6324134d53ade6`  
		Last Modified: Fri, 16 Jun 2023 05:52:22 GMT  
		Size: 4.3 KB (4332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd91ceaa583a76bc85231b9ce41fd23fa35fb9256ee47d37ce5519525f1f4eab`  
		Last Modified: Fri, 16 Jun 2023 05:52:22 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed79fba284b4b35a82f34cdd8a083b228f925fe9d329c07e0f9d33c9607d2253`  
		Last Modified: Fri, 16 Jun 2023 05:52:30 GMT  
		Size: 218.3 MB (218328212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3106b45811e1338a0676a17f56cb843f09ca7f99f7780418d14da2e75efb0b`  
		Last Modified: Fri, 16 Jun 2023 05:52:22 GMT  
		Size: 6.3 KB (6309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11.2-slim` - linux; ppc64le

```console
$ docker pull solr@sha256:e5bf7de5f3a81916ba68d0803b2a20683c3f343526ac4504bf83ff58a3554e7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.2 MB (317172564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622e27233dfd4792c9d6f51e19e2c8549ad71521b3e68abd69f92eceb9ec6724`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:24 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:25 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:28 GMT
ADD file:0a2372ac4d43f0f4ada2b55dd0a359df73a828a9aa9426bfdd05a02b9c4b2bd9 in / 
# Mon, 05 Jun 2023 17:08:28 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:17:32 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:17:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:17:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:18:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:20:58 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 02:22:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:22:25 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 07:41:31 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Fri, 16 Jun 2023 07:41:31 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 16 Jun 2023 07:41:32 GMT
ARG SOLR_VERSION=8.11.2
# Fri, 16 Jun 2023 07:41:32 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Fri, 16 Jun 2023 07:41:33 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Fri, 16 Jun 2023 07:41:33 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 07:41:34 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 07:41:55 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 16 Jun 2023 07:41:56 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 16 Jun 2023 07:42:00 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 07:42:17 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 16 Jun 2023 07:42:49 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 16 Jun 2023 07:42:52 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Fri, 16 Jun 2023 07:42:53 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 07:42:55 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 07:42:57 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 07:42:58 GMT
USER 8983
# Fri, 16 Jun 2023 07:42:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 07:42:59 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:1fbda4a01aa9e184a223c30ab58441354cde30fe3083bc1d8ca9f7823ab4fe68`  
		Last Modified: Fri, 16 Jun 2023 01:24:20 GMT  
		Size: 33.3 MB (33309776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb717f01d0b915280274134b467bc61cb1a7be1d9c6a9fe149dd3e9ab5d4d5`  
		Last Modified: Fri, 16 Jun 2023 02:26:38 GMT  
		Size: 17.6 MB (17648879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd6c33e350c331fd82a3898e4308740b9228a93a9bd1cfbf209b8ac158961d6`  
		Last Modified: Fri, 16 Jun 2023 02:29:11 GMT  
		Size: 42.1 MB (42093841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ce0cb194906f7f8bf1248463cbef057861d206d072004bad81d1784fdb4b54`  
		Last Modified: Fri, 16 Jun 2023 02:29:00 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17d3ac8d21a63094e82ec5c4dc8dfa1c0cbfd4a7108d667bbf3b154435fa7f5`  
		Last Modified: Fri, 16 Jun 2023 07:44:57 GMT  
		Size: 5.8 MB (5777612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d596f773882c647c8f31f469e949edc08d29108d6e9eb47e8c45fae8fe6b8720`  
		Last Modified: Fri, 16 Jun 2023 07:44:55 GMT  
		Size: 4.3 KB (4297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7413d7cf84cc22e166149d3b19012981e5bcf3d7de8c109d5331ed65b172585`  
		Last Modified: Fri, 16 Jun 2023 07:44:55 GMT  
		Size: 3.5 KB (3469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5dedd276de4704622c2f0ba1ccc9b716e2b2000dc8af1b59a94b4c3f7c66a3`  
		Last Modified: Fri, 16 Jun 2023 07:45:12 GMT  
		Size: 218.3 MB (218328223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba39db06026d8858274e3c4e59ed877a895145ee633b4585cc44b1f4c38115b`  
		Last Modified: Fri, 16 Jun 2023 07:44:55 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11.2-slim` - linux; s390x

```console
$ docker pull solr@sha256:3cb7e3eb537f722ef2d096a1cc9e90107d5a26a93eac004e2be96f7709fa7a7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.7 MB (306665402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc08946ca2b22de4fde16a15d59e3eb3989c0f8948b178b9440a9df20d36de60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:35 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:37 GMT
ADD file:44c66c03ba0afcc05de1b2078f83e8bfe04706b31491fcd3fdd93cfc88d5f06c in / 
# Thu, 13 Apr 2023 13:09:37 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:16:00 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:16:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:16:00 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:16:11 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:41:46 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:43:00 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:43:03 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:36:38 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 26 Apr 2023 20:36:38 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_VERSION=8.11.2
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:36:38 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:36:43 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 26 Apr 2023 20:36:44 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 26 Apr 2023 20:36:44 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:36:51 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 26 Apr 2023 20:37:07 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 26 Apr 2023 20:37:11 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 26 Apr 2023 20:37:11 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:37:12 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:37:12 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:37:12 GMT
USER 8983
# Wed, 26 Apr 2023 20:37:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:37:12 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:f11b609b1d63f2d37c0e3789823e7a7e62a078bddca7c46da8602655989c62d9`  
		Last Modified: Fri, 14 Apr 2023 09:38:39 GMT  
		Size: 27.0 MB (27016370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c307a57c5f07334cfab6db8f8324b0c9dff13121ec34d8db1d4a71e3529d4b5`  
		Last Modified: Tue, 18 Apr 2023 01:18:27 GMT  
		Size: 16.0 MB (16035272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f2464ae2b2cf26ad0951e353283a0faff6e21082c5b3ffc1ee96700cd352db8`  
		Last Modified: Wed, 26 Apr 2023 19:46:33 GMT  
		Size: 40.5 MB (40540743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2357373aba3b86e27f47b65c90b2c45aa55910d7a8e20ab95b0211c90ac0afc5`  
		Last Modified: Wed, 26 Apr 2023 19:46:28 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283aa23eb2725cd0f2f9e5627452bda5952b9f2b8279f3973cff4bc6bd8f2f8c`  
		Last Modified: Wed, 26 Apr 2023 20:38:26 GMT  
		Size: 4.7 MB (4730562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b9b134fa6b4ae6e10d35a150c618d122d72cb88c9c0def17080d179a2bc4fa`  
		Last Modified: Wed, 26 Apr 2023 20:38:25 GMT  
		Size: 4.3 KB (4333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b39ba054e26d24e3a1ea7e6e0fa808358921ad07e25bfe70ebde348e13891c`  
		Last Modified: Wed, 26 Apr 2023 20:38:25 GMT  
		Size: 3.5 KB (3468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a942f8f7937f22541141bb4ad17bd44e43cf1cbf39893673e50f572aa2f3fc27`  
		Last Modified: Wed, 26 Apr 2023 20:38:34 GMT  
		Size: 218.3 MB (218328187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3753012f9147597bbee82b53507c05d7009de3e3684021b64da90103d9d65c3f`  
		Last Modified: Wed, 26 Apr 2023 20:38:25 GMT  
		Size: 6.3 KB (6306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:9`

```console
$ docker pull solr@sha256:73f4afe26d489830e59bf8db6e1e29a1adb86e4946b19d3db73fbc3684a1748f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `solr:9` - linux; amd64

```console
$ docker pull solr@sha256:e29c8b80f1864d67f40d0fbf9cc2dc080479abffd9a5cb4fcf12eea2759898c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **375.3 MB (375313008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee92e4df31178121b908f977309aa653980c8ead4c00a6456d7ef802bbd01816`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:15:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:15:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:15:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:18:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:18:30 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:19:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:19:05 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:26:45 GMT
ARG SOLR_VERSION=9.2.1
# Fri, 16 Jun 2023 05:26:45 GMT
ARG SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:27:05 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.version=9.2.1
# Fri, 16 Jun 2023 05:27:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 05:27:07 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 05:27:07 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:27:08 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 05:27:08 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 05:27:16 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 05:27:16 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:27:17 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:27:17 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:27:17 GMT
USER 8983
# Fri, 16 Jun 2023 05:27:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:27:17 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857412f02e8d49bb7e247b45ce86ce6378bd0bc5e8533e1fffa2a6e7a93aab46`  
		Last Modified: Fri, 16 Jun 2023 02:23:30 GMT  
		Size: 17.0 MB (17040964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f618ea570e7708381040c3f1662a8ff625710ddd7b5e0145b46bdf5231985c`  
		Last Modified: Fri, 16 Jun 2023 02:24:16 GMT  
		Size: 47.0 MB (47006286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2665c89972dd3400540a4420904c1912a3990b0a3be38d49d50a94b9da26231`  
		Last Modified: Fri, 16 Jun 2023 02:24:10 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42b38db22e6b18b3bc85f4e165ec99d95cf616e24a46a16b202a4d250561d3c`  
		Last Modified: Fri, 16 Jun 2023 05:30:50 GMT  
		Size: 279.0 MB (278994099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb98ce87480dfd3e75ac21f048446ae8df10c8dedff32cd9f263d02d1a825bf8`  
		Last Modified: Fri, 16 Jun 2023 05:30:38 GMT  
		Size: 4.3 KB (4288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a37d4231e60e1d0dc230f2efc9d2560cdc8dedf9e4b250d0818da3cee7def5`  
		Last Modified: Fri, 16 Jun 2023 05:30:38 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8928bcc26c2ef972e3082782ab6af19d2073d8e99c35453e7442950937d4f2b`  
		Last Modified: Fri, 16 Jun 2023 05:30:38 GMT  
		Size: 8.3 KB (8268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a14db093f859ab0b789c47440b60c02aee9d6a13e83e9b650a7b142280b4452`  
		Last Modified: Fri, 16 Jun 2023 05:30:39 GMT  
		Size: 1.8 MB (1827683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9` - linux; arm variant v7

```console
$ docker pull solr@sha256:df5a4df27d6223472cdf39d015d0be71d2e3674169077c668259410ac9ed2f20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **369.4 MB (369434561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90d9b6bd34c3e1002a86e117f66e584a416854d27e7c66f806f1a01cf6d15fd8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 16:59:35 GMT
ARG RELEASE
# Mon, 05 Jun 2023 16:59:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 16:59:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 16:59:35 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 16:59:40 GMT
ADD file:5425962ced738173a50965fc5cd95c79d0a319323df4a34e9da3f5037a5264c3 in / 
# Mon, 05 Jun 2023 16:59:40 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:25:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 01:25:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 01:25:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 01:28:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:28:03 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 01:28:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 01:28:33 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 02:38:27 GMT
ARG SOLR_VERSION=9.2.1
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 02:38:52 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 02:38:55 GMT
LABEL org.opencontainers.image.version=9.2.1
# Fri, 16 Jun 2023 02:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 02:38:55 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 02:38:55 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 02:38:56 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 02:38:56 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 02:39:05 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 02:39:05 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 02:39:05 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 02:39:05 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 02:39:05 GMT
USER 8983
# Fri, 16 Jun 2023 02:39:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 02:39:06 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:de11f41b5c8ee0d3b259584977df4adb3e9b005f95756baecf491f70b498f301`  
		Last Modified: Wed, 07 Jun 2023 02:07:45 GMT  
		Size: 27.0 MB (27026252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88eb1b8897047cd0a4d969ca49bb4696512a41ef9d4466bc36e6bb42d97ca8dd`  
		Last Modified: Fri, 16 Jun 2023 01:31:49 GMT  
		Size: 17.2 MB (17168477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4e9b19cfde4210390e27af028b3821849f4637891e197e449641eb7824c5e1`  
		Last Modified: Fri, 16 Jun 2023 01:32:33 GMT  
		Size: 44.6 MB (44579970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69809a3884cff3cd2a14f35fede7e33256861cf01f1afb3f2fe52660b7fbfb72`  
		Last Modified: Fri, 16 Jun 2023 01:32:26 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15016717bbccbb8afaa8cd53f43070ec0fc4ccd1229c858a599c76179c0fee9`  
		Last Modified: Fri, 16 Jun 2023 02:42:49 GMT  
		Size: 279.0 MB (278994307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df6c3913894e2b72c13f2694b8975504ad21fcec95c266e2f9b3fe81c6c7846`  
		Last Modified: Fri, 16 Jun 2023 02:42:34 GMT  
		Size: 4.2 KB (4223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e043faaa195146204f1395ba9ffff82c7db8ad8bceb6342ba54add360a69a15c`  
		Last Modified: Fri, 16 Jun 2023 02:42:34 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a294eea0d8dce46694f985b5876d7480e52e3ab622133cca6771a36dcb330c`  
		Last Modified: Fri, 16 Jun 2023 02:42:34 GMT  
		Size: 8.3 KB (8265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32ce8d699bbfad8bd6eb33cb5bcbbe23ce1c33711b92eb2055125082aeda9d8`  
		Last Modified: Fri, 16 Jun 2023 02:42:35 GMT  
		Size: 1.7 MB (1652690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:66509e3fc448ac1d4772e7d726c2cf22fe0d4967714e3c65afe9c65c4a495621
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.0 MB (374038205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd904f26d14316cf21764a5752c2ec1106c1a2bd920731c901a018585999f16d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:45:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:45:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:45:39 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:47:57 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:47:57 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:48:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:48:26 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:47:48 GMT
ARG SOLR_VERSION=9.2.1
# Fri, 16 Jun 2023 05:47:48 GMT
ARG SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:48:04 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.version=9.2.1
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 05:48:06 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 05:48:07 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:48:07 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 05:48:08 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 05:48:16 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 05:48:16 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:48:16 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:48:16 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:48:16 GMT
USER 8983
# Fri, 16 Jun 2023 05:48:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:48:16 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5168066327b37e44f2a0ef7f788219bdbcd9013e4320cf4b9229ea9dfb73b561`  
		Last Modified: Fri, 16 Jun 2023 02:52:08 GMT  
		Size: 18.5 MB (18465563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78b269707ca01885483219b119ab6f03209c4c452696f1dcf105d191a7115cb`  
		Last Modified: Fri, 16 Jun 2023 02:52:47 GMT  
		Size: 46.5 MB (46488623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb861b98c25f139f6cf3783bb0c0c5a4810ad99eaba8cf8695eefe7f8614a8b`  
		Last Modified: Fri, 16 Jun 2023 02:52:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3400a3f980bb2b3adf154d3fc86f306788ac6cff76728fde865037e3ede88b68`  
		Last Modified: Fri, 16 Jun 2023 05:51:36 GMT  
		Size: 279.0 MB (278994703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11950a4bc9f97d203c1476552d153fcc683e3957621da8768cd3fa39ee02d0eb`  
		Last Modified: Fri, 16 Jun 2023 05:51:26 GMT  
		Size: 4.3 KB (4331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042db7dc8c2d6e3b53376afc669becc9ca9910f7044388ce3d98ff880351321f`  
		Last Modified: Fri, 16 Jun 2023 05:51:26 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fec7819b9a55bdc72dd442a462e31fbe1414cadd44f1bcd765716dd6b4e3c622`  
		Last Modified: Fri, 16 Jun 2023 05:51:26 GMT  
		Size: 8.3 KB (8269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da205b415c9da2bcf6f1d7532f914f0bd453728f8ec6beba5eb09cfd86cb27f`  
		Last Modified: Fri, 16 Jun 2023 05:51:27 GMT  
		Size: 1.7 MB (1687137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9` - linux; ppc64le

```console
$ docker pull solr@sha256:7237335d603e527c83ab9545e0865684521980f5c406a28d58969c7c6e58e70b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.7 MB (381748792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3b61810d471dd4c39d87767e32a88170d6f0d0a3cf37eb7eb200614ba8e14db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:01:00 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:01:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:01:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:01:01 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:01:03 GMT
ADD file:00c4f44b35b683caef54d5b8b0e0b1e68872f45eae17dd7543adaf6c54512447 in / 
# Mon, 05 Jun 2023 17:01:04 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:19:12 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:19:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:19:13 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:24:42 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:24:43 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:25:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:25:43 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 07:36:03 GMT
ARG SOLR_VERSION=9.2.1
# Fri, 16 Jun 2023 07:36:04 GMT
ARG SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb
# Fri, 16 Jun 2023 07:36:04 GMT
ARG SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271
# Fri, 16 Jun 2023 07:36:05 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 07:36:05 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 07:36:05 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 07:36:06 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 07:36:06 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 07:37:24 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 16 Jun 2023 07:37:29 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 07:37:29 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 07:37:30 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 07:37:30 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 07:37:31 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 07:37:32 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 07:37:35 GMT
LABEL org.opencontainers.image.version=9.2.1
# Fri, 16 Jun 2023 07:37:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 07:37:37 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 07:37:39 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 07:37:41 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 07:37:43 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 07:38:00 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 07:38:00 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 07:38:01 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 07:38:01 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 07:38:02 GMT
USER 8983
# Fri, 16 Jun 2023 07:38:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 07:38:03 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:a02dd69d9a8a1e6f4fc2ccb509fb8efd6014b00ff932a757d23b4b012a2bec49`  
		Last Modified: Fri, 16 Jun 2023 00:44:52 GMT  
		Size: 35.7 MB (35711397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bd55325dd69030064f13098489df6ef8e45b2d52baffb366675c06f6e94418`  
		Last Modified: Fri, 16 Jun 2023 02:30:20 GMT  
		Size: 18.3 MB (18322826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef75c435e36e0d0cb9911afc443c4bf6c1769b56642390039838f6017497b2f`  
		Last Modified: Fri, 16 Jun 2023 02:31:24 GMT  
		Size: 46.9 MB (46872498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edff0610bd2e6e17f260f10d236a0fad32db564c59f810b5e30eaee37ef5faf8`  
		Last Modified: Fri, 16 Jun 2023 02:31:13 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d7ebdacee82ac6455d940b19d21bf659f1cf53c3aaa3f3e1577135b8802d3e`  
		Last Modified: Fri, 16 Jun 2023 07:43:45 GMT  
		Size: 279.0 MB (278994934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64708f76d121ff3c1262875272f841e9c3bb2244f1d305672fed751d7c638df1`  
		Last Modified: Fri, 16 Jun 2023 07:43:24 GMT  
		Size: 4.3 KB (4297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495b3eb13c2abbf80d9c705cdb460f2f939de60c92c610848a2c4defab47dd11`  
		Last Modified: Fri, 16 Jun 2023 07:43:24 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8695e9bc13470e29cd835a938319952511edd7c991fecadf3ed9d64c89a727b`  
		Last Modified: Fri, 16 Jun 2023 07:43:24 GMT  
		Size: 8.3 KB (8273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3227aa649395d114eef9c32c931462d8a75c9fe23aa39081891ddc6dc3c31c74`  
		Last Modified: Fri, 16 Jun 2023 07:43:25 GMT  
		Size: 1.8 MB (1834188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9` - linux; s390x

```console
$ docker pull solr@sha256:2e2e1090eeb5e9008c115e614650f992c607ac460b8d848c6bcf4c5fbdfa2f09
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **370.0 MB (370021779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f06f08b94cb5330a7ff42794eee64cc602fd8b2713258fcdb3ca2001d12c0e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 22 May 2023 17:46:45 GMT
ARG RELEASE
# Mon, 22 May 2023 17:46:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 22 May 2023 17:46:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 22 May 2023 17:46:45 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 22 May 2023 17:46:47 GMT
ADD file:7bf1b7a1484e37f289d40f5c1c1cbe321ef337f898dd3d5809193c848a9a3dc2 in / 
# Mon, 22 May 2023 17:46:47 GMT
CMD ["/bin/bash"]
# Thu, 01 Jun 2023 23:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 01 Jun 2023 23:33:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Jun 2023 23:33:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 01 Jun 2023 23:34:41 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 01 Jun 2023 23:34:43 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Thu, 01 Jun 2023 23:35:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 01 Jun 2023 23:35:21 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_VERSION=9.2.1
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 02 Jun 2023 15:53:16 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 02 Jun 2023 15:53:20 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 02 Jun 2023 15:53:20 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.version=9.2.1
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 02 Jun 2023 15:53:21 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 02 Jun 2023 15:53:21 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 02 Jun 2023 15:53:22 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 02 Jun 2023 15:53:22 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 02 Jun 2023 15:53:27 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 02 Jun 2023 15:53:27 GMT
VOLUME [/var/solr]
# Fri, 02 Jun 2023 15:53:27 GMT
EXPOSE 8983
# Fri, 02 Jun 2023 15:53:27 GMT
WORKDIR /opt/solr
# Fri, 02 Jun 2023 15:53:28 GMT
USER 8983
# Fri, 02 Jun 2023 15:53:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Jun 2023 15:53:28 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:f2957179c3a13374d05630725d1d996f8083efadf7d2da999c9b4ca53ab7c98f`  
		Last Modified: Thu, 01 Jun 2023 23:19:06 GMT  
		Size: 28.6 MB (28648005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff49023eb8231a4489c04787627471c943342afea6aed42b66e0bd17f75307a`  
		Last Modified: Thu, 01 Jun 2023 23:36:33 GMT  
		Size: 16.8 MB (16817675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58123ce9cafda91814be25f8b9b9f99431886cfbee190fc6ba7f6be9abdfe781`  
		Last Modified: Thu, 01 Jun 2023 23:36:56 GMT  
		Size: 43.8 MB (43774489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c27d78a58220d69494be2a17dffa9c4de667bdcf0f6e85c869482d832b8af8f`  
		Last Modified: Thu, 01 Jun 2023 23:36:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeab0826386b334263843df3860f46ec4cb1baa7490d55f653630de11aefecb2`  
		Last Modified: Fri, 02 Jun 2023 15:54:19 GMT  
		Size: 279.0 MB (278994275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5f2afb9fbda66fff0a22400f8df154060d0f1d74944a07653c6466fb541622`  
		Last Modified: Fri, 02 Jun 2023 15:54:08 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b24eb5989fbe19cfbfa7fade0c611dd880bd9f279f3960ce96ca5a35e4188ad`  
		Last Modified: Fri, 02 Jun 2023 15:54:08 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fbd279dbd567d795f616c80182d1ea59f0584002dcd56265accfa296ec81551`  
		Last Modified: Fri, 02 Jun 2023 15:54:08 GMT  
		Size: 8.3 KB (8265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf0d1005aca634a3af1af7d7165552463412e8d705e08a29aec622534e2987f`  
		Last Modified: Fri, 02 Jun 2023 15:54:08 GMT  
		Size: 1.8 MB (1774360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:9.0`

```console
$ docker pull solr@sha256:841f338a3bcecc639e8b91d2a60b969291b75302cfd9e60557a3114551735083
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `solr:9.0` - linux; amd64

```console
$ docker pull solr@sha256:ba29b8ae61f4ce848ae73e1551e2579275e0ed2f67eca020d668001e4a27eb67
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.0 MB (325001013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:041e99479c566ea4f86ba84a59925a305dbbf6c9aa3cda6d3f8a1c514fbe0caa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground","-a","-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:15:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:15:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:15:07 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:18:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:18:03 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:18:57 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:18:57 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:28:30 GMT
ARG SOLR_VERSION=9.0.0
# Fri, 16 Jun 2023 05:28:30 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Fri, 16 Jun 2023 05:28:30 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Fri, 16 Jun 2023 05:28:30 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:28:30 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:28:30 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 05:28:30 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 05:28:30 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 05:29:10 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Fri, 16 Jun 2023 05:29:11 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 05:29:11 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 05:29:11 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 05:29:11 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 05:29:11 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 05:29:11 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 05:29:11 GMT
LABEL org.opencontainers.image.version=9.0.0
# Fri, 16 Jun 2023 05:29:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 05:29:11 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 05:29:12 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:29:13 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 05:29:13 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 05:29:18 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 05:29:18 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:29:18 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:29:18 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:29:18 GMT
USER solr
# Fri, 16 Jun 2023 05:29:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:29:19 GMT
CMD ["solr-foreground" "-a" "-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddf068c018154ad6aca69d7f48df2e3b365cdc9b1c644b1b5028cd5eb9bd6e6`  
		Last Modified: Fri, 16 Jun 2023 02:23:07 GMT  
		Size: 20.2 MB (20155613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f36b29c57a33222ba78883e5ed33c006782a2a67d2d8c8c6f86a802b2f0cbc`  
		Last Modified: Fri, 16 Jun 2023 02:24:01 GMT  
		Size: 47.0 MB (47008144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335c545c513d061d6056747d8e8c0c84214f8f360b2ab59f7aff587ad4a78aa5`  
		Last Modified: Fri, 16 Jun 2023 02:23:54 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db7e2105a0ff19967362b372bbc5ab1c2a124dda0e83855bb5b2a3575121df0`  
		Last Modified: Fri, 16 Jun 2023 05:31:32 GMT  
		Size: 227.7 MB (227662292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376e9e514a2f645dc5e2c11a9d798ed96a6cbbad7c62a55203dbb8ce62b0d1e0`  
		Last Modified: Fri, 16 Jun 2023 05:31:22 GMT  
		Size: 4.3 KB (4297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d819684bb3f2818aec12a9d047f99408a57d9f2c1ef27f26c308e8d4b3b5be5`  
		Last Modified: Fri, 16 Jun 2023 05:31:21 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13d5059d19860bcca599063e339ed1495bcf5ff54d6e711e634b365309c3a0c`  
		Last Modified: Fri, 16 Jun 2023 05:31:21 GMT  
		Size: 7.9 KB (7903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77af3f5378228800445111fbf6d2f2c43c461672e1d4acbfb4b2762a1ce8e9a3`  
		Last Modified: Fri, 16 Jun 2023 05:31:22 GMT  
		Size: 1.6 MB (1581865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.0` - linux; arm variant v7

```console
$ docker pull solr@sha256:c2a17f2900e5837f0342dcb69b81247aeba1e86a3cb9cff82fdac95e2170ba53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.3 MB (317256893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e1668565a5de5e786f1a228c97922e334372c2cf2a40769882b1df3b5dc8c18`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground","-a","-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:24:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 01:24:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 01:24:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 01:27:26 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:27:27 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 01:28:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 01:28:26 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 02:40:16 GMT
ARG SOLR_VERSION=9.0.0
# Fri, 16 Jun 2023 02:40:17 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Fri, 16 Jun 2023 02:40:17 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Fri, 16 Jun 2023 02:40:17 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 02:40:17 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 02:40:17 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 02:40:17 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 02:40:17 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 02:41:03 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Fri, 16 Jun 2023 02:41:04 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 02:41:04 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 02:41:04 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 02:41:04 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 02:41:04 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 02:41:05 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 02:41:05 GMT
LABEL org.opencontainers.image.version=9.0.0
# Fri, 16 Jun 2023 02:41:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 02:41:05 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 02:41:05 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 02:41:06 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 02:41:06 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 02:41:11 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 02:41:11 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 02:41:11 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 02:41:11 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 02:41:11 GMT
USER solr
# Fri, 16 Jun 2023 02:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 02:41:11 GMT
CMD ["solr-foreground" "-a" "-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]
```

-	Layers:
	-	`sha256:2d97abfcf215d35e8a846b390350fea9f455676b41221360fe8782163a1c46bb`  
		Last Modified: Thu, 15 Jun 2023 03:47:54 GMT  
		Size: 24.6 MB (24589116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9067cc6505509e2b7bb16e7f0c09847b2c08d84d194afcfb81a01431688d9b`  
		Last Modified: Fri, 16 Jun 2023 01:31:24 GMT  
		Size: 19.5 MB (19538930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86d0b9906f1a7659a745219e2b7904d2163c1dfd34153ace3b55af0b6b04886`  
		Last Modified: Fri, 16 Jun 2023 01:32:18 GMT  
		Size: 44.6 MB (44580468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c125e36293ea372de7eadc3701d2baa0ca1dee5a05b508373e71bd6617591282`  
		Last Modified: Fri, 16 Jun 2023 01:32:11 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5fd60f5d32b48fcae29d7f46ce988d999211298b99e5123909b9446d574c5d`  
		Last Modified: Fri, 16 Jun 2023 02:43:34 GMT  
		Size: 227.1 MB (227140908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d193ff1e197716eafa247f0c0993b411357495405e1feddf132599d1887d62b`  
		Last Modified: Fri, 16 Jun 2023 02:43:22 GMT  
		Size: 4.2 KB (4226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d9a73dc9169103c9826a9716888bc521cac248ced4ff4ad535ff6cf06c41fb`  
		Last Modified: Fri, 16 Jun 2023 02:43:22 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f822dcd48c971c8c2e39e0a7896b8e1f1110de98d88b518a447414a59b5e94c3`  
		Last Modified: Fri, 16 Jun 2023 02:43:22 GMT  
		Size: 7.9 KB (7902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c47cfe6b7abfdf57d12ad57e81898d25ae674b12d9d6c8aedf2833cb6d8560b`  
		Last Modified: Fri, 16 Jun 2023 02:43:22 GMT  
		Size: 1.4 MB (1394965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.0` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:f1b643c535db31f1f7be948899b280d7c66f78c8f08067c8802de83d4bff1e16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.7 MB (323669126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23bd26753089058f54f25a3f7d769bbcc13b70fbf7caafc30f45fab32d764ba1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground","-a","-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:44:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:44:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:44:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:47:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:47:29 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:48:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:48:20 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:49:31 GMT
ARG SOLR_VERSION=9.0.0
# Fri, 16 Jun 2023 05:49:31 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Fri, 16 Jun 2023 05:49:31 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Fri, 16 Jun 2023 05:49:31 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:49:31 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:49:31 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 05:49:31 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 05:49:31 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 05:50:09 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Fri, 16 Jun 2023 05:50:11 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 05:50:11 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 05:50:11 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 05:50:11 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 05:50:11 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 05:50:11 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 05:50:11 GMT
LABEL org.opencontainers.image.version=9.0.0
# Fri, 16 Jun 2023 05:50:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 05:50:11 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 05:50:12 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:50:12 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 05:50:13 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 05:50:17 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 05:50:17 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:50:17 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:50:17 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:50:17 GMT
USER solr
# Fri, 16 Jun 2023 05:50:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:50:17 GMT
CMD ["solr-foreground" "-a" "-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7df34455c6332518666f21f4f050fc1d28e48de7b568f21125226b340db412`  
		Last Modified: Fri, 16 Jun 2023 02:51:47 GMT  
		Size: 20.9 MB (20872989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ec1a7145e9007907e6ba14f6070da444e90e283473ce2acfc7660172adf406`  
		Last Modified: Fri, 16 Jun 2023 02:52:34 GMT  
		Size: 46.5 MB (46488208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c3796b9578230135cc26bb899903ad68b0e918bda0dfa6070fcbb531472c42`  
		Last Modified: Fri, 16 Jun 2023 02:52:29 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8dc857281bdfa707bee590511b3c8d01491e3368f2e27cb3c26b03f070bc6e`  
		Last Modified: Fri, 16 Jun 2023 05:52:14 GMT  
		Size: 227.7 MB (227650870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda7593f125900d97f4208fe9e758b3a62532a411416919c1ab15cba243c9760`  
		Last Modified: Fri, 16 Jun 2023 05:52:05 GMT  
		Size: 4.3 KB (4332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7aff61e3aff2b9d2f9b98d93d168f047c38f0e068ea5f78763f026261e5a1b`  
		Last Modified: Fri, 16 Jun 2023 05:52:05 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e81fc6f56c7a240243de4d7db4d6677aa61ba9292a1378ca191b6a1b6cc507c`  
		Last Modified: Fri, 16 Jun 2023 05:52:05 GMT  
		Size: 7.9 KB (7903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7b4a441ef4ca83260564ab7c907d6d17304f0b36fea822003b27cfa527ea0f`  
		Last Modified: Fri, 16 Jun 2023 05:52:06 GMT  
		Size: 1.4 MB (1444010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.0` - linux; ppc64le

```console
$ docker pull solr@sha256:af9f7da073aafa8738d21911f4bff3c20f4f8473444a5f7aa37703650d489098
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.4 MB (332448638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3c07a3d6bd0bc9774127034806633f3a23b83d67e17ef13474737ba42b2febb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground","-a","-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:24 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:25 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:28 GMT
ADD file:0a2372ac4d43f0f4ada2b55dd0a359df73a828a9aa9426bfdd05a02b9c4b2bd9 in / 
# Mon, 05 Jun 2023 17:08:28 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:17:32 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:17:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:17:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:23:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:23:32 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:25:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:25:29 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 07:39:51 GMT
ARG SOLR_VERSION=9.0.0
# Fri, 16 Jun 2023 07:39:52 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Fri, 16 Jun 2023 07:39:53 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Fri, 16 Jun 2023 07:39:53 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 07:39:53 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 07:39:54 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 07:39:54 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 07:39:54 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 07:40:40 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Fri, 16 Jun 2023 07:40:44 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 07:40:44 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 07:40:45 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 07:40:45 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 07:40:46 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 07:40:47 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 07:40:48 GMT
LABEL org.opencontainers.image.version=9.0.0
# Fri, 16 Jun 2023 07:40:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 07:40:49 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 07:40:52 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 07:40:53 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 07:40:54 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 07:41:08 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 07:41:09 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 07:41:10 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 07:41:12 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 07:41:13 GMT
USER solr
# Fri, 16 Jun 2023 07:41:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 07:41:13 GMT
CMD ["solr-foreground" "-a" "-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]
```

-	Layers:
	-	`sha256:1fbda4a01aa9e184a223c30ab58441354cde30fe3083bc1d8ca9f7823ab4fe68`  
		Last Modified: Fri, 16 Jun 2023 01:24:20 GMT  
		Size: 33.3 MB (33309776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ad609b0dd14d25a533bad107d7d80f6a0143d184f80e43339a78811d5d58f6`  
		Last Modified: Fri, 16 Jun 2023 02:29:46 GMT  
		Size: 22.1 MB (22128326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11320ad109f515402d5d72270e3d40edc4ede3c81e18e8ffd54fb4f52f8e5e9`  
		Last Modified: Fri, 16 Jun 2023 02:31:04 GMT  
		Size: 46.9 MB (46872353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479808ab83f741c9d71794d5fcdf2fa889239fb3a46acdd165d94e11a2660437`  
		Last Modified: Fri, 16 Jun 2023 02:30:53 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a458172172b4ec2836251bd351b3491cc91ec0fdc94bf175ca346a234a55c5`  
		Last Modified: Fri, 16 Jun 2023 07:44:46 GMT  
		Size: 228.5 MB (228521289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65967de8c282a7e6aac3e501a66ce523b19c66a634abf2ffb736e1c6fbf24a0b`  
		Last Modified: Fri, 16 Jun 2023 07:44:28 GMT  
		Size: 4.3 KB (4297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b4097a29a801c59a3f6019e7ba9930c9fe425d41b80783ac2deea4bebab10b`  
		Last Modified: Fri, 16 Jun 2023 07:44:28 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dff7506cc1849699154fd04ee0cd4eb12f16f749f6666b5e21d44e73cd393ca`  
		Last Modified: Fri, 16 Jun 2023 07:44:28 GMT  
		Size: 7.9 KB (7902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afd58592d4625542897b738be14349bca7dca2a870052d7811da6a5560b7978`  
		Last Modified: Fri, 16 Jun 2023 07:44:28 GMT  
		Size: 1.6 MB (1604316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.0` - linux; s390x

```console
$ docker pull solr@sha256:c6cbecab43252ee2804b957c04be33e28627c8a67a533eba5691a92c889c9419
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.4 MB (319408887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:726844ff7d881d7a1ad6d81acfb72ee764c69a7a42e1804c2ab86f88bb5e4087`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground","-a","-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:35 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:37 GMT
ADD file:44c66c03ba0afcc05de1b2078f83e8bfe04706b31491fcd3fdd93cfc88d5f06c in / 
# Thu, 13 Apr 2023 13:09:37 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:16:00 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:16:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:16:00 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:17:09 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:43:29 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:44:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:44:40 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:35:57 GMT
ARG SOLR_VERSION=9.0.0
# Wed, 26 Apr 2023 20:35:57 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Wed, 26 Apr 2023 20:35:57 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Wed, 26 Apr 2023 20:35:57 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:35:57 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:35:57 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Wed, 26 Apr 2023 20:35:57 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Wed, 26 Apr 2023 20:35:57 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Wed, 26 Apr 2023 20:36:18 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Wed, 26 Apr 2023 20:36:23 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:36:23 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:36:23 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:36:23 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:36:23 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:36:23 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:36:24 GMT
LABEL org.opencontainers.image.version=9.0.0
# Wed, 26 Apr 2023 20:36:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:36:24 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:36:24 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:36:25 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:36:25 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:36:29 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:36:29 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:36:29 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:36:29 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:36:29 GMT
USER solr
# Wed, 26 Apr 2023 20:36:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:36:30 GMT
CMD ["solr-foreground" "-a" "-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]
```

-	Layers:
	-	`sha256:f11b609b1d63f2d37c0e3789823e7a7e62a078bddca7c46da8602655989c62d9`  
		Last Modified: Fri, 14 Apr 2023 09:38:39 GMT  
		Size: 27.0 MB (27016370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf6c28f706c8f54c079ff27fe5409527f68c7463df6adf843d835f265547cf5`  
		Last Modified: Tue, 18 Apr 2023 01:19:02 GMT  
		Size: 19.5 MB (19532693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75157323f95569e14c082fe3aac39ef8f2f30ca3ad7d03107404eedde5396dbd`  
		Last Modified: Wed, 26 Apr 2023 19:48:03 GMT  
		Size: 43.8 MB (43775512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019b37c50f3b2d15194e9d039c46d5cd37c3f563d0a937909910fb7449a6430a`  
		Last Modified: Wed, 26 Apr 2023 19:47:57 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52c90854ff982e9cfd0b4c637adf726dfeefb50d36cb1645b524e272e51fedf`  
		Last Modified: Wed, 26 Apr 2023 20:38:20 GMT  
		Size: 227.6 MB (227575747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec756c0d1ba4e173d5858e8d7b88d8527d869b5255f625667d373a98b57bb3f`  
		Last Modified: Wed, 26 Apr 2023 20:38:11 GMT  
		Size: 4.3 KB (4331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076cffae83076991c5a36985e1b6208e9a72f786d9a7402f7b86e6d3c660f5e9`  
		Last Modified: Wed, 26 Apr 2023 20:38:11 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6899a5cc36b887d092d47d35a3c788281aa3740bf7413fa0c7c7f4a80c6037c`  
		Last Modified: Wed, 26 Apr 2023 20:38:11 GMT  
		Size: 7.9 KB (7900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068e2f4d886f85c8165ecb4c3ae55d2e4f9fbe5184d93cabe547dd8f4921678a`  
		Last Modified: Wed, 26 Apr 2023 20:38:11 GMT  
		Size: 1.5 MB (1495954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:9.0.0`

```console
$ docker pull solr@sha256:841f338a3bcecc639e8b91d2a60b969291b75302cfd9e60557a3114551735083
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `solr:9.0.0` - linux; amd64

```console
$ docker pull solr@sha256:ba29b8ae61f4ce848ae73e1551e2579275e0ed2f67eca020d668001e4a27eb67
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.0 MB (325001013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:041e99479c566ea4f86ba84a59925a305dbbf6c9aa3cda6d3f8a1c514fbe0caa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground","-a","-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:15:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:15:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:15:07 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:18:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:18:03 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:18:57 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:18:57 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:28:30 GMT
ARG SOLR_VERSION=9.0.0
# Fri, 16 Jun 2023 05:28:30 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Fri, 16 Jun 2023 05:28:30 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Fri, 16 Jun 2023 05:28:30 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:28:30 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:28:30 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 05:28:30 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 05:28:30 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 05:29:10 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Fri, 16 Jun 2023 05:29:11 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 05:29:11 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 05:29:11 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 05:29:11 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 05:29:11 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 05:29:11 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 05:29:11 GMT
LABEL org.opencontainers.image.version=9.0.0
# Fri, 16 Jun 2023 05:29:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 05:29:11 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 05:29:12 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:29:13 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 05:29:13 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 05:29:18 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 05:29:18 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:29:18 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:29:18 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:29:18 GMT
USER solr
# Fri, 16 Jun 2023 05:29:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:29:19 GMT
CMD ["solr-foreground" "-a" "-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddf068c018154ad6aca69d7f48df2e3b365cdc9b1c644b1b5028cd5eb9bd6e6`  
		Last Modified: Fri, 16 Jun 2023 02:23:07 GMT  
		Size: 20.2 MB (20155613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f36b29c57a33222ba78883e5ed33c006782a2a67d2d8c8c6f86a802b2f0cbc`  
		Last Modified: Fri, 16 Jun 2023 02:24:01 GMT  
		Size: 47.0 MB (47008144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335c545c513d061d6056747d8e8c0c84214f8f360b2ab59f7aff587ad4a78aa5`  
		Last Modified: Fri, 16 Jun 2023 02:23:54 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db7e2105a0ff19967362b372bbc5ab1c2a124dda0e83855bb5b2a3575121df0`  
		Last Modified: Fri, 16 Jun 2023 05:31:32 GMT  
		Size: 227.7 MB (227662292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376e9e514a2f645dc5e2c11a9d798ed96a6cbbad7c62a55203dbb8ce62b0d1e0`  
		Last Modified: Fri, 16 Jun 2023 05:31:22 GMT  
		Size: 4.3 KB (4297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d819684bb3f2818aec12a9d047f99408a57d9f2c1ef27f26c308e8d4b3b5be5`  
		Last Modified: Fri, 16 Jun 2023 05:31:21 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13d5059d19860bcca599063e339ed1495bcf5ff54d6e711e634b365309c3a0c`  
		Last Modified: Fri, 16 Jun 2023 05:31:21 GMT  
		Size: 7.9 KB (7903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77af3f5378228800445111fbf6d2f2c43c461672e1d4acbfb4b2762a1ce8e9a3`  
		Last Modified: Fri, 16 Jun 2023 05:31:22 GMT  
		Size: 1.6 MB (1581865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.0.0` - linux; arm variant v7

```console
$ docker pull solr@sha256:c2a17f2900e5837f0342dcb69b81247aeba1e86a3cb9cff82fdac95e2170ba53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.3 MB (317256893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e1668565a5de5e786f1a228c97922e334372c2cf2a40769882b1df3b5dc8c18`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground","-a","-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:24:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 01:24:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 01:24:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 01:27:26 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:27:27 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 01:28:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 01:28:26 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 02:40:16 GMT
ARG SOLR_VERSION=9.0.0
# Fri, 16 Jun 2023 02:40:17 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Fri, 16 Jun 2023 02:40:17 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Fri, 16 Jun 2023 02:40:17 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 02:40:17 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 02:40:17 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 02:40:17 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 02:40:17 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 02:41:03 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Fri, 16 Jun 2023 02:41:04 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 02:41:04 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 02:41:04 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 02:41:04 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 02:41:04 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 02:41:05 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 02:41:05 GMT
LABEL org.opencontainers.image.version=9.0.0
# Fri, 16 Jun 2023 02:41:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 02:41:05 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 02:41:05 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 02:41:06 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 02:41:06 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 02:41:11 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 02:41:11 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 02:41:11 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 02:41:11 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 02:41:11 GMT
USER solr
# Fri, 16 Jun 2023 02:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 02:41:11 GMT
CMD ["solr-foreground" "-a" "-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]
```

-	Layers:
	-	`sha256:2d97abfcf215d35e8a846b390350fea9f455676b41221360fe8782163a1c46bb`  
		Last Modified: Thu, 15 Jun 2023 03:47:54 GMT  
		Size: 24.6 MB (24589116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9067cc6505509e2b7bb16e7f0c09847b2c08d84d194afcfb81a01431688d9b`  
		Last Modified: Fri, 16 Jun 2023 01:31:24 GMT  
		Size: 19.5 MB (19538930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86d0b9906f1a7659a745219e2b7904d2163c1dfd34153ace3b55af0b6b04886`  
		Last Modified: Fri, 16 Jun 2023 01:32:18 GMT  
		Size: 44.6 MB (44580468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c125e36293ea372de7eadc3701d2baa0ca1dee5a05b508373e71bd6617591282`  
		Last Modified: Fri, 16 Jun 2023 01:32:11 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5fd60f5d32b48fcae29d7f46ce988d999211298b99e5123909b9446d574c5d`  
		Last Modified: Fri, 16 Jun 2023 02:43:34 GMT  
		Size: 227.1 MB (227140908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d193ff1e197716eafa247f0c0993b411357495405e1feddf132599d1887d62b`  
		Last Modified: Fri, 16 Jun 2023 02:43:22 GMT  
		Size: 4.2 KB (4226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d9a73dc9169103c9826a9716888bc521cac248ced4ff4ad535ff6cf06c41fb`  
		Last Modified: Fri, 16 Jun 2023 02:43:22 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f822dcd48c971c8c2e39e0a7896b8e1f1110de98d88b518a447414a59b5e94c3`  
		Last Modified: Fri, 16 Jun 2023 02:43:22 GMT  
		Size: 7.9 KB (7902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c47cfe6b7abfdf57d12ad57e81898d25ae674b12d9d6c8aedf2833cb6d8560b`  
		Last Modified: Fri, 16 Jun 2023 02:43:22 GMT  
		Size: 1.4 MB (1394965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.0.0` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:f1b643c535db31f1f7be948899b280d7c66f78c8f08067c8802de83d4bff1e16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.7 MB (323669126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23bd26753089058f54f25a3f7d769bbcc13b70fbf7caafc30f45fab32d764ba1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground","-a","-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:44:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:44:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:44:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:47:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:47:29 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:48:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:48:20 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:49:31 GMT
ARG SOLR_VERSION=9.0.0
# Fri, 16 Jun 2023 05:49:31 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Fri, 16 Jun 2023 05:49:31 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Fri, 16 Jun 2023 05:49:31 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:49:31 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:49:31 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 05:49:31 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 05:49:31 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 05:50:09 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Fri, 16 Jun 2023 05:50:11 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 05:50:11 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 05:50:11 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 05:50:11 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 05:50:11 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 05:50:11 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 05:50:11 GMT
LABEL org.opencontainers.image.version=9.0.0
# Fri, 16 Jun 2023 05:50:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 05:50:11 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 05:50:12 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:50:12 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 05:50:13 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 05:50:17 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 05:50:17 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:50:17 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:50:17 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:50:17 GMT
USER solr
# Fri, 16 Jun 2023 05:50:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:50:17 GMT
CMD ["solr-foreground" "-a" "-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7df34455c6332518666f21f4f050fc1d28e48de7b568f21125226b340db412`  
		Last Modified: Fri, 16 Jun 2023 02:51:47 GMT  
		Size: 20.9 MB (20872989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ec1a7145e9007907e6ba14f6070da444e90e283473ce2acfc7660172adf406`  
		Last Modified: Fri, 16 Jun 2023 02:52:34 GMT  
		Size: 46.5 MB (46488208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c3796b9578230135cc26bb899903ad68b0e918bda0dfa6070fcbb531472c42`  
		Last Modified: Fri, 16 Jun 2023 02:52:29 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8dc857281bdfa707bee590511b3c8d01491e3368f2e27cb3c26b03f070bc6e`  
		Last Modified: Fri, 16 Jun 2023 05:52:14 GMT  
		Size: 227.7 MB (227650870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda7593f125900d97f4208fe9e758b3a62532a411416919c1ab15cba243c9760`  
		Last Modified: Fri, 16 Jun 2023 05:52:05 GMT  
		Size: 4.3 KB (4332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7aff61e3aff2b9d2f9b98d93d168f047c38f0e068ea5f78763f026261e5a1b`  
		Last Modified: Fri, 16 Jun 2023 05:52:05 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e81fc6f56c7a240243de4d7db4d6677aa61ba9292a1378ca191b6a1b6cc507c`  
		Last Modified: Fri, 16 Jun 2023 05:52:05 GMT  
		Size: 7.9 KB (7903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7b4a441ef4ca83260564ab7c907d6d17304f0b36fea822003b27cfa527ea0f`  
		Last Modified: Fri, 16 Jun 2023 05:52:06 GMT  
		Size: 1.4 MB (1444010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.0.0` - linux; ppc64le

```console
$ docker pull solr@sha256:af9f7da073aafa8738d21911f4bff3c20f4f8473444a5f7aa37703650d489098
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.4 MB (332448638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3c07a3d6bd0bc9774127034806633f3a23b83d67e17ef13474737ba42b2febb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground","-a","-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:24 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:25 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:28 GMT
ADD file:0a2372ac4d43f0f4ada2b55dd0a359df73a828a9aa9426bfdd05a02b9c4b2bd9 in / 
# Mon, 05 Jun 2023 17:08:28 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:17:32 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:17:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:17:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:23:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:23:32 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:25:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:25:29 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 07:39:51 GMT
ARG SOLR_VERSION=9.0.0
# Fri, 16 Jun 2023 07:39:52 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Fri, 16 Jun 2023 07:39:53 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Fri, 16 Jun 2023 07:39:53 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 07:39:53 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 07:39:54 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 07:39:54 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 07:39:54 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 16 Jun 2023 07:40:40 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Fri, 16 Jun 2023 07:40:44 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 07:40:44 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 07:40:45 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 07:40:45 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 07:40:46 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 07:40:47 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 07:40:48 GMT
LABEL org.opencontainers.image.version=9.0.0
# Fri, 16 Jun 2023 07:40:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 07:40:49 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 07:40:52 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 07:40:53 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 07:40:54 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 07:41:08 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 07:41:09 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 07:41:10 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 07:41:12 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 07:41:13 GMT
USER solr
# Fri, 16 Jun 2023 07:41:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 07:41:13 GMT
CMD ["solr-foreground" "-a" "-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]
```

-	Layers:
	-	`sha256:1fbda4a01aa9e184a223c30ab58441354cde30fe3083bc1d8ca9f7823ab4fe68`  
		Last Modified: Fri, 16 Jun 2023 01:24:20 GMT  
		Size: 33.3 MB (33309776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ad609b0dd14d25a533bad107d7d80f6a0143d184f80e43339a78811d5d58f6`  
		Last Modified: Fri, 16 Jun 2023 02:29:46 GMT  
		Size: 22.1 MB (22128326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11320ad109f515402d5d72270e3d40edc4ede3c81e18e8ffd54fb4f52f8e5e9`  
		Last Modified: Fri, 16 Jun 2023 02:31:04 GMT  
		Size: 46.9 MB (46872353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479808ab83f741c9d71794d5fcdf2fa889239fb3a46acdd165d94e11a2660437`  
		Last Modified: Fri, 16 Jun 2023 02:30:53 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a458172172b4ec2836251bd351b3491cc91ec0fdc94bf175ca346a234a55c5`  
		Last Modified: Fri, 16 Jun 2023 07:44:46 GMT  
		Size: 228.5 MB (228521289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65967de8c282a7e6aac3e501a66ce523b19c66a634abf2ffb736e1c6fbf24a0b`  
		Last Modified: Fri, 16 Jun 2023 07:44:28 GMT  
		Size: 4.3 KB (4297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b4097a29a801c59a3f6019e7ba9930c9fe425d41b80783ac2deea4bebab10b`  
		Last Modified: Fri, 16 Jun 2023 07:44:28 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dff7506cc1849699154fd04ee0cd4eb12f16f749f6666b5e21d44e73cd393ca`  
		Last Modified: Fri, 16 Jun 2023 07:44:28 GMT  
		Size: 7.9 KB (7902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afd58592d4625542897b738be14349bca7dca2a870052d7811da6a5560b7978`  
		Last Modified: Fri, 16 Jun 2023 07:44:28 GMT  
		Size: 1.6 MB (1604316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.0.0` - linux; s390x

```console
$ docker pull solr@sha256:c6cbecab43252ee2804b957c04be33e28627c8a67a533eba5691a92c889c9419
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.4 MB (319408887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:726844ff7d881d7a1ad6d81acfb72ee764c69a7a42e1804c2ab86f88bb5e4087`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground","-a","-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:35 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:37 GMT
ADD file:44c66c03ba0afcc05de1b2078f83e8bfe04706b31491fcd3fdd93cfc88d5f06c in / 
# Thu, 13 Apr 2023 13:09:37 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:16:00 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:16:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:16:00 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:17:09 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:43:29 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:44:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:44:40 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:35:57 GMT
ARG SOLR_VERSION=9.0.0
# Wed, 26 Apr 2023 20:35:57 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Wed, 26 Apr 2023 20:35:57 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Wed, 26 Apr 2023 20:35:57 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:35:57 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:35:57 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Wed, 26 Apr 2023 20:35:57 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Wed, 26 Apr 2023 20:35:57 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Wed, 26 Apr 2023 20:36:18 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Wed, 26 Apr 2023 20:36:23 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:36:23 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:36:23 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:36:23 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:36:23 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:36:23 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:36:24 GMT
LABEL org.opencontainers.image.version=9.0.0
# Wed, 26 Apr 2023 20:36:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:36:24 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:36:24 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:36:25 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:36:25 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:36:29 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:36:29 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:36:29 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:36:29 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:36:29 GMT
USER solr
# Wed, 26 Apr 2023 20:36:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:36:30 GMT
CMD ["solr-foreground" "-a" "-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]
```

-	Layers:
	-	`sha256:f11b609b1d63f2d37c0e3789823e7a7e62a078bddca7c46da8602655989c62d9`  
		Last Modified: Fri, 14 Apr 2023 09:38:39 GMT  
		Size: 27.0 MB (27016370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf6c28f706c8f54c079ff27fe5409527f68c7463df6adf843d835f265547cf5`  
		Last Modified: Tue, 18 Apr 2023 01:19:02 GMT  
		Size: 19.5 MB (19532693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75157323f95569e14c082fe3aac39ef8f2f30ca3ad7d03107404eedde5396dbd`  
		Last Modified: Wed, 26 Apr 2023 19:48:03 GMT  
		Size: 43.8 MB (43775512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019b37c50f3b2d15194e9d039c46d5cd37c3f563d0a937909910fb7449a6430a`  
		Last Modified: Wed, 26 Apr 2023 19:47:57 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52c90854ff982e9cfd0b4c637adf726dfeefb50d36cb1645b524e272e51fedf`  
		Last Modified: Wed, 26 Apr 2023 20:38:20 GMT  
		Size: 227.6 MB (227575747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec756c0d1ba4e173d5858e8d7b88d8527d869b5255f625667d373a98b57bb3f`  
		Last Modified: Wed, 26 Apr 2023 20:38:11 GMT  
		Size: 4.3 KB (4331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076cffae83076991c5a36985e1b6208e9a72f786d9a7402f7b86e6d3c660f5e9`  
		Last Modified: Wed, 26 Apr 2023 20:38:11 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6899a5cc36b887d092d47d35a3c788281aa3740bf7413fa0c7c7f4a80c6037c`  
		Last Modified: Wed, 26 Apr 2023 20:38:11 GMT  
		Size: 7.9 KB (7900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068e2f4d886f85c8165ecb4c3ae55d2e4f9fbe5184d93cabe547dd8f4921678a`  
		Last Modified: Wed, 26 Apr 2023 20:38:11 GMT  
		Size: 1.5 MB (1495954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:9.1`

```console
$ docker pull solr@sha256:8b0706eb7d846153ebc86636ffa6d881f1d309d94ffbfbf274b2986b76ba5b47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `solr:9.1` - linux; amd64

```console
$ docker pull solr@sha256:7310141881795663d09220b412b3fdbd6e7c2c088c677e0df8d471f4f69ac7d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.1 MB (331080101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74c7d9936c5dbdf22246292069a2eaf3d5411531a2b5f1176012d0dbaee18ef0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:15:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:15:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:15:07 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:18:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:18:03 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:18:57 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:18:57 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:27:20 GMT
ARG SOLR_VERSION=9.1.1
# Fri, 16 Jun 2023 05:27:20 GMT
ARG SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f
# Fri, 16 Jun 2023 05:27:20 GMT
ARG SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763
# Fri, 16 Jun 2023 05:27:20 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:27:20 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:27:20 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 05:27:20 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 05:27:20 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 05:28:07 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Fri, 16 Jun 2023 05:28:07 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 05:28:07 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 05:28:07 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 05:28:08 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 05:28:08 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 05:28:08 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 05:28:08 GMT
LABEL org.opencontainers.image.version=9.1.1
# Fri, 16 Jun 2023 05:28:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 05:28:08 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 05:28:09 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:28:09 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 05:28:10 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 05:28:18 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 05:28:18 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:28:18 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:28:18 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:28:18 GMT
USER 8983
# Fri, 16 Jun 2023 05:28:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:28:18 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddf068c018154ad6aca69d7f48df2e3b365cdc9b1c644b1b5028cd5eb9bd6e6`  
		Last Modified: Fri, 16 Jun 2023 02:23:07 GMT  
		Size: 20.2 MB (20155613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f36b29c57a33222ba78883e5ed33c006782a2a67d2d8c8c6f86a802b2f0cbc`  
		Last Modified: Fri, 16 Jun 2023 02:24:01 GMT  
		Size: 47.0 MB (47008144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335c545c513d061d6056747d8e8c0c84214f8f360b2ab59f7aff587ad4a78aa5`  
		Last Modified: Fri, 16 Jun 2023 02:23:54 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3b09b23e7233f1d8e14bae10872265ec4a5b2d52f631b1d82420039f82ccf5`  
		Last Modified: Fri, 16 Jun 2023 05:31:13 GMT  
		Size: 233.7 MB (233741212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cfce5f3fa8e9175ea6d5563557519eadb38fb8901f62e15968abc2b416528f`  
		Last Modified: Fri, 16 Jun 2023 05:31:03 GMT  
		Size: 4.3 KB (4295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8289b3c2cc2c84eef7fcea43f9032f4f4912a3e5deca4ef926c813c14b43e4`  
		Last Modified: Fri, 16 Jun 2023 05:31:03 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4dac0da5df6c8857e1c3cfd1fbbb9b70253a3a8d113661cfa1ba88eecf236c`  
		Last Modified: Fri, 16 Jun 2023 05:31:03 GMT  
		Size: 8.1 KB (8083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5c352ed833844fd696c4b9a16a8f000a4c782a8e50ee5ee768f33142f797da`  
		Last Modified: Fri, 16 Jun 2023 05:31:03 GMT  
		Size: 1.6 MB (1581855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.1` - linux; arm variant v7

```console
$ docker pull solr@sha256:496bb5472837adeeb4340a957f6d69b242153bb33a1664405417172cd2e63647
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.3 MB (323337139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87d7a8646db8fc2da95b22da10da8a7cd5f8208457b49d7f5b82ba989d869f57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:24:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 01:24:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 01:24:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 01:27:26 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:27:27 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 01:28:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 01:28:26 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 02:39:07 GMT
ARG SOLR_VERSION=9.1.1
# Fri, 16 Jun 2023 02:39:08 GMT
ARG SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f
# Fri, 16 Jun 2023 02:39:08 GMT
ARG SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763
# Fri, 16 Jun 2023 02:39:08 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 02:39:08 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 02:39:08 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 02:39:08 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 02:39:08 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 02:39:55 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Fri, 16 Jun 2023 02:39:56 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 02:39:56 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 02:39:56 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 02:39:56 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 02:39:56 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 02:39:57 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 02:39:57 GMT
LABEL org.opencontainers.image.version=9.1.1
# Fri, 16 Jun 2023 02:39:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 02:39:57 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 02:39:57 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 02:39:58 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 02:39:58 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 02:40:06 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 02:40:06 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 02:40:06 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 02:40:06 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 02:40:06 GMT
USER 8983
# Fri, 16 Jun 2023 02:40:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 02:40:07 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:2d97abfcf215d35e8a846b390350fea9f455676b41221360fe8782163a1c46bb`  
		Last Modified: Thu, 15 Jun 2023 03:47:54 GMT  
		Size: 24.6 MB (24589116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9067cc6505509e2b7bb16e7f0c09847b2c08d84d194afcfb81a01431688d9b`  
		Last Modified: Fri, 16 Jun 2023 01:31:24 GMT  
		Size: 19.5 MB (19538930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86d0b9906f1a7659a745219e2b7904d2163c1dfd34153ace3b55af0b6b04886`  
		Last Modified: Fri, 16 Jun 2023 01:32:18 GMT  
		Size: 44.6 MB (44580468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c125e36293ea372de7eadc3701d2baa0ca1dee5a05b508373e71bd6617591282`  
		Last Modified: Fri, 16 Jun 2023 01:32:11 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0daa7e3e9110a7802c2ba7b0b22ca85a3696ae274fef00216999fdba8b7d1489`  
		Last Modified: Fri, 16 Jun 2023 02:43:13 GMT  
		Size: 233.2 MB (233220928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b5b478c7b072b48c7c355c583ba5755d98781852d2a3d5adb43e9ad463ce08`  
		Last Modified: Fri, 16 Jun 2023 02:43:01 GMT  
		Size: 4.2 KB (4223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2747812eff566c171186c399b59ba542c8ff56fa33009dcc87b0682727e0320`  
		Last Modified: Fri, 16 Jun 2023 02:43:01 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aef2c4be8352ff77f18d16377e689d5ab4e117a12a2538956a7f22c9f65d01a`  
		Last Modified: Fri, 16 Jun 2023 02:43:01 GMT  
		Size: 8.1 KB (8080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe42c3d0c5e95f7071c557e5c178af147a0ddca219450dcda6b26c63715fced`  
		Last Modified: Fri, 16 Jun 2023 02:43:01 GMT  
		Size: 1.4 MB (1395014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.1` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:ae9c8c1b915e54e4b3448a3b62d78346c93ba1a5af2062b9f11a16c3c4b165dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.8 MB (329750760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:796d13c6b076c672476e743fad10318b9d35367908c1f576bc2a5728f2eafa46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:44:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:44:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:44:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:47:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:47:29 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:48:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:48:20 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:48:22 GMT
ARG SOLR_VERSION=9.1.1
# Fri, 16 Jun 2023 05:48:22 GMT
ARG SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f
# Fri, 16 Jun 2023 05:48:22 GMT
ARG SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763
# Fri, 16 Jun 2023 05:48:22 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:48:22 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:48:22 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 05:48:22 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 05:48:22 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 05:49:09 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Fri, 16 Jun 2023 05:49:10 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 05:49:10 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 05:49:11 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 05:49:11 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 05:49:11 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 05:49:11 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 05:49:11 GMT
LABEL org.opencontainers.image.version=9.1.1
# Fri, 16 Jun 2023 05:49:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 05:49:11 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 05:49:12 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:49:12 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 05:49:13 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 05:49:19 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 05:49:19 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:49:20 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:49:20 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:49:20 GMT
USER 8983
# Fri, 16 Jun 2023 05:49:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:49:20 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7df34455c6332518666f21f4f050fc1d28e48de7b568f21125226b340db412`  
		Last Modified: Fri, 16 Jun 2023 02:51:47 GMT  
		Size: 20.9 MB (20872989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ec1a7145e9007907e6ba14f6070da444e90e283473ce2acfc7660172adf406`  
		Last Modified: Fri, 16 Jun 2023 02:52:34 GMT  
		Size: 46.5 MB (46488208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c3796b9578230135cc26bb899903ad68b0e918bda0dfa6070fcbb531472c42`  
		Last Modified: Fri, 16 Jun 2023 02:52:29 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312342ee3138b43b79d439dd69b91b51041cbf11d2916ef062d8d12c2cad8ee0`  
		Last Modified: Fri, 16 Jun 2023 05:51:57 GMT  
		Size: 233.7 MB (233732325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5612ff1d143fd5a97472ba8959c9a4da1f9db05cb0bca4f0baa7d43b2397c13`  
		Last Modified: Fri, 16 Jun 2023 05:51:48 GMT  
		Size: 4.3 KB (4334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabc9010d20e8019f412d0f2490fbf9605936d0eb8986ed5a4b8f498f289e3e7`  
		Last Modified: Fri, 16 Jun 2023 05:51:48 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bbae7a52b4721b7831fe3ea9659ba565f4ed7d01059285c914e18ccf10bfd6`  
		Last Modified: Fri, 16 Jun 2023 05:51:48 GMT  
		Size: 8.1 KB (8084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca77244d065f72458950fce89e5a6f6403da3d7b130c89bb9fe36881178e2ed6`  
		Last Modified: Fri, 16 Jun 2023 05:51:48 GMT  
		Size: 1.4 MB (1444005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.1` - linux; ppc64le

```console
$ docker pull solr@sha256:3d475a832984e044bb63c7d70a9b21d27cdc94447d2b9fb4d91d080a1fce8724
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.5 MB (338528985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:998c28a09a30f0c1858a1f6a14e389fc6f9c0378fcdac96f28b5dc18b40add2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:24 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:25 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:28 GMT
ADD file:0a2372ac4d43f0f4ada2b55dd0a359df73a828a9aa9426bfdd05a02b9c4b2bd9 in / 
# Mon, 05 Jun 2023 17:08:28 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:17:32 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:17:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:17:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:23:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:23:32 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:25:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:25:29 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 07:38:12 GMT
ARG SOLR_VERSION=9.1.1
# Fri, 16 Jun 2023 07:38:12 GMT
ARG SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f
# Fri, 16 Jun 2023 07:38:13 GMT
ARG SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763
# Fri, 16 Jun 2023 07:38:14 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 07:38:14 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 07:38:16 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 07:38:16 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 07:38:17 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 07:39:09 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Fri, 16 Jun 2023 07:39:13 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 07:39:13 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 07:39:14 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 07:39:14 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 07:39:14 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 07:39:15 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 07:39:15 GMT
LABEL org.opencontainers.image.version=9.1.1
# Fri, 16 Jun 2023 07:39:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 07:39:16 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 07:39:19 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 07:39:20 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 07:39:22 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 07:39:35 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 07:39:36 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 07:39:37 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 07:39:38 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 07:39:38 GMT
USER 8983
# Fri, 16 Jun 2023 07:39:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 07:39:39 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:1fbda4a01aa9e184a223c30ab58441354cde30fe3083bc1d8ca9f7823ab4fe68`  
		Last Modified: Fri, 16 Jun 2023 01:24:20 GMT  
		Size: 33.3 MB (33309776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ad609b0dd14d25a533bad107d7d80f6a0143d184f80e43339a78811d5d58f6`  
		Last Modified: Fri, 16 Jun 2023 02:29:46 GMT  
		Size: 22.1 MB (22128326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11320ad109f515402d5d72270e3d40edc4ede3c81e18e8ffd54fb4f52f8e5e9`  
		Last Modified: Fri, 16 Jun 2023 02:31:04 GMT  
		Size: 46.9 MB (46872353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479808ab83f741c9d71794d5fcdf2fa889239fb3a46acdd165d94e11a2660437`  
		Last Modified: Fri, 16 Jun 2023 02:30:53 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3cefb506513f1817b42d49d48ef1360a4fb676a1d67decebb9a1a4c305b1348`  
		Last Modified: Fri, 16 Jun 2023 07:44:18 GMT  
		Size: 234.6 MB (234601456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6cff7bbc9114849bfffd3ff2844feef0da0f7cac82a0c4762e112bfcb4d3a6`  
		Last Modified: Fri, 16 Jun 2023 07:43:59 GMT  
		Size: 4.3 KB (4302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112c62e18932edc5d28d8afe0b1e7f9557d8b01bf3780db93f0ca157d8d54298`  
		Last Modified: Fri, 16 Jun 2023 07:43:59 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2134ceca5a4d10557e90ee4a622db03959055abb6b1f8d0651c1703a8d40464`  
		Last Modified: Fri, 16 Jun 2023 07:43:59 GMT  
		Size: 8.1 KB (8082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23143a1cb26656f63484c091ae88ef1c2a475c8581fb14d5db252cfbe933747`  
		Last Modified: Fri, 16 Jun 2023 07:43:59 GMT  
		Size: 1.6 MB (1604311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.1` - linux; s390x

```console
$ docker pull solr@sha256:e56a6fff2aa8bbc6fa79b57922f3443215b46e090999cd73c422572adf0a8b5b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.5 MB (325490601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9ed519da34ebadd2d4bce0da97eee7b903c08762396541e436095ee885829c9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:35 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:37 GMT
ADD file:44c66c03ba0afcc05de1b2078f83e8bfe04706b31491fcd3fdd93cfc88d5f06c in / 
# Thu, 13 Apr 2023 13:09:37 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:16:00 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:16:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:16:00 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:17:09 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:43:29 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:44:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:44:40 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:35:00 GMT
ARG SOLR_VERSION=9.1.1
# Wed, 26 Apr 2023 20:35:00 GMT
ARG SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f
# Wed, 26 Apr 2023 20:35:00 GMT
ARG SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763
# Wed, 26 Apr 2023 20:35:00 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:35:00 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:35:00 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz
# Wed, 26 Apr 2023 20:35:00 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Wed, 26 Apr 2023 20:35:01 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Wed, 26 Apr 2023 20:35:36 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Wed, 26 Apr 2023 20:35:41 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:35:41 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:35:41 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:35:41 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:35:41 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:35:42 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:35:42 GMT
LABEL org.opencontainers.image.version=9.1.1
# Wed, 26 Apr 2023 20:35:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:35:42 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:35:42 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:35:43 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:35:43 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:35:48 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:35:48 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:35:48 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:35:48 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:35:49 GMT
USER 8983
# Wed, 26 Apr 2023 20:35:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:35:49 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:f11b609b1d63f2d37c0e3789823e7a7e62a078bddca7c46da8602655989c62d9`  
		Last Modified: Fri, 14 Apr 2023 09:38:39 GMT  
		Size: 27.0 MB (27016370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf6c28f706c8f54c079ff27fe5409527f68c7463df6adf843d835f265547cf5`  
		Last Modified: Tue, 18 Apr 2023 01:19:02 GMT  
		Size: 19.5 MB (19532693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75157323f95569e14c082fe3aac39ef8f2f30ca3ad7d03107404eedde5396dbd`  
		Last Modified: Wed, 26 Apr 2023 19:48:03 GMT  
		Size: 43.8 MB (43775512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019b37c50f3b2d15194e9d039c46d5cd37c3f563d0a937909910fb7449a6430a`  
		Last Modified: Wed, 26 Apr 2023 19:47:57 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d94818969d07fed3dcf5a2ac39ac93d9dff860ec94f26640729a1bbd11d096e`  
		Last Modified: Wed, 26 Apr 2023 20:38:05 GMT  
		Size: 233.7 MB (233657251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911c96e0a2127384038700755982837f01f9814778a959e01b9f1f3f10aee4ac`  
		Last Modified: Wed, 26 Apr 2023 20:37:55 GMT  
		Size: 4.3 KB (4332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf10f7de9abf15f66ef7ffb2690123a6c55d2c264c29dd143b70e3d86b4befc0`  
		Last Modified: Wed, 26 Apr 2023 20:37:55 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c7e17cb3734a80d62f85e6e55dc722e83c2917e50fa3f29e27b6cd0b606ee2`  
		Last Modified: Wed, 26 Apr 2023 20:37:55 GMT  
		Size: 8.1 KB (8082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95125298d64bf04b588602df40d51bcd817b1cc5434864fd6c6273fcd0f0f924`  
		Last Modified: Wed, 26 Apr 2023 20:37:56 GMT  
		Size: 1.5 MB (1495981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:9.1.1`

```console
$ docker pull solr@sha256:8b0706eb7d846153ebc86636ffa6d881f1d309d94ffbfbf274b2986b76ba5b47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `solr:9.1.1` - linux; amd64

```console
$ docker pull solr@sha256:7310141881795663d09220b412b3fdbd6e7c2c088c677e0df8d471f4f69ac7d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.1 MB (331080101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74c7d9936c5dbdf22246292069a2eaf3d5411531a2b5f1176012d0dbaee18ef0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:15:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:15:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:15:07 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:18:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:18:03 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:18:57 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:18:57 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:27:20 GMT
ARG SOLR_VERSION=9.1.1
# Fri, 16 Jun 2023 05:27:20 GMT
ARG SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f
# Fri, 16 Jun 2023 05:27:20 GMT
ARG SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763
# Fri, 16 Jun 2023 05:27:20 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:27:20 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:27:20 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 05:27:20 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 05:27:20 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 05:28:07 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Fri, 16 Jun 2023 05:28:07 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 05:28:07 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 05:28:07 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 05:28:08 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 05:28:08 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 05:28:08 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 05:28:08 GMT
LABEL org.opencontainers.image.version=9.1.1
# Fri, 16 Jun 2023 05:28:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 05:28:08 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 05:28:09 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:28:09 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 05:28:10 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 05:28:18 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 05:28:18 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:28:18 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:28:18 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:28:18 GMT
USER 8983
# Fri, 16 Jun 2023 05:28:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:28:18 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddf068c018154ad6aca69d7f48df2e3b365cdc9b1c644b1b5028cd5eb9bd6e6`  
		Last Modified: Fri, 16 Jun 2023 02:23:07 GMT  
		Size: 20.2 MB (20155613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f36b29c57a33222ba78883e5ed33c006782a2a67d2d8c8c6f86a802b2f0cbc`  
		Last Modified: Fri, 16 Jun 2023 02:24:01 GMT  
		Size: 47.0 MB (47008144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335c545c513d061d6056747d8e8c0c84214f8f360b2ab59f7aff587ad4a78aa5`  
		Last Modified: Fri, 16 Jun 2023 02:23:54 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3b09b23e7233f1d8e14bae10872265ec4a5b2d52f631b1d82420039f82ccf5`  
		Last Modified: Fri, 16 Jun 2023 05:31:13 GMT  
		Size: 233.7 MB (233741212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cfce5f3fa8e9175ea6d5563557519eadb38fb8901f62e15968abc2b416528f`  
		Last Modified: Fri, 16 Jun 2023 05:31:03 GMT  
		Size: 4.3 KB (4295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8289b3c2cc2c84eef7fcea43f9032f4f4912a3e5deca4ef926c813c14b43e4`  
		Last Modified: Fri, 16 Jun 2023 05:31:03 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4dac0da5df6c8857e1c3cfd1fbbb9b70253a3a8d113661cfa1ba88eecf236c`  
		Last Modified: Fri, 16 Jun 2023 05:31:03 GMT  
		Size: 8.1 KB (8083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5c352ed833844fd696c4b9a16a8f000a4c782a8e50ee5ee768f33142f797da`  
		Last Modified: Fri, 16 Jun 2023 05:31:03 GMT  
		Size: 1.6 MB (1581855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.1.1` - linux; arm variant v7

```console
$ docker pull solr@sha256:496bb5472837adeeb4340a957f6d69b242153bb33a1664405417172cd2e63647
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.3 MB (323337139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87d7a8646db8fc2da95b22da10da8a7cd5f8208457b49d7f5b82ba989d869f57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:24:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 01:24:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 01:24:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 01:27:26 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:27:27 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 01:28:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 01:28:26 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 02:39:07 GMT
ARG SOLR_VERSION=9.1.1
# Fri, 16 Jun 2023 02:39:08 GMT
ARG SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f
# Fri, 16 Jun 2023 02:39:08 GMT
ARG SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763
# Fri, 16 Jun 2023 02:39:08 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 02:39:08 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 02:39:08 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 02:39:08 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 02:39:08 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 02:39:55 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Fri, 16 Jun 2023 02:39:56 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 02:39:56 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 02:39:56 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 02:39:56 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 02:39:56 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 02:39:57 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 02:39:57 GMT
LABEL org.opencontainers.image.version=9.1.1
# Fri, 16 Jun 2023 02:39:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 02:39:57 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 02:39:57 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 02:39:58 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 02:39:58 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 02:40:06 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 02:40:06 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 02:40:06 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 02:40:06 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 02:40:06 GMT
USER 8983
# Fri, 16 Jun 2023 02:40:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 02:40:07 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:2d97abfcf215d35e8a846b390350fea9f455676b41221360fe8782163a1c46bb`  
		Last Modified: Thu, 15 Jun 2023 03:47:54 GMT  
		Size: 24.6 MB (24589116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9067cc6505509e2b7bb16e7f0c09847b2c08d84d194afcfb81a01431688d9b`  
		Last Modified: Fri, 16 Jun 2023 01:31:24 GMT  
		Size: 19.5 MB (19538930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86d0b9906f1a7659a745219e2b7904d2163c1dfd34153ace3b55af0b6b04886`  
		Last Modified: Fri, 16 Jun 2023 01:32:18 GMT  
		Size: 44.6 MB (44580468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c125e36293ea372de7eadc3701d2baa0ca1dee5a05b508373e71bd6617591282`  
		Last Modified: Fri, 16 Jun 2023 01:32:11 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0daa7e3e9110a7802c2ba7b0b22ca85a3696ae274fef00216999fdba8b7d1489`  
		Last Modified: Fri, 16 Jun 2023 02:43:13 GMT  
		Size: 233.2 MB (233220928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b5b478c7b072b48c7c355c583ba5755d98781852d2a3d5adb43e9ad463ce08`  
		Last Modified: Fri, 16 Jun 2023 02:43:01 GMT  
		Size: 4.2 KB (4223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2747812eff566c171186c399b59ba542c8ff56fa33009dcc87b0682727e0320`  
		Last Modified: Fri, 16 Jun 2023 02:43:01 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aef2c4be8352ff77f18d16377e689d5ab4e117a12a2538956a7f22c9f65d01a`  
		Last Modified: Fri, 16 Jun 2023 02:43:01 GMT  
		Size: 8.1 KB (8080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe42c3d0c5e95f7071c557e5c178af147a0ddca219450dcda6b26c63715fced`  
		Last Modified: Fri, 16 Jun 2023 02:43:01 GMT  
		Size: 1.4 MB (1395014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.1.1` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:ae9c8c1b915e54e4b3448a3b62d78346c93ba1a5af2062b9f11a16c3c4b165dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.8 MB (329750760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:796d13c6b076c672476e743fad10318b9d35367908c1f576bc2a5728f2eafa46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:44:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:44:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:44:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:47:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:47:29 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:48:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:48:20 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:48:22 GMT
ARG SOLR_VERSION=9.1.1
# Fri, 16 Jun 2023 05:48:22 GMT
ARG SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f
# Fri, 16 Jun 2023 05:48:22 GMT
ARG SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763
# Fri, 16 Jun 2023 05:48:22 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:48:22 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:48:22 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 05:48:22 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 05:48:22 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 05:49:09 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Fri, 16 Jun 2023 05:49:10 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 05:49:10 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 05:49:11 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 05:49:11 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 05:49:11 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 05:49:11 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 05:49:11 GMT
LABEL org.opencontainers.image.version=9.1.1
# Fri, 16 Jun 2023 05:49:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 05:49:11 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 05:49:12 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:49:12 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 05:49:13 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 05:49:19 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 05:49:19 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:49:20 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:49:20 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:49:20 GMT
USER 8983
# Fri, 16 Jun 2023 05:49:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:49:20 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7df34455c6332518666f21f4f050fc1d28e48de7b568f21125226b340db412`  
		Last Modified: Fri, 16 Jun 2023 02:51:47 GMT  
		Size: 20.9 MB (20872989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ec1a7145e9007907e6ba14f6070da444e90e283473ce2acfc7660172adf406`  
		Last Modified: Fri, 16 Jun 2023 02:52:34 GMT  
		Size: 46.5 MB (46488208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c3796b9578230135cc26bb899903ad68b0e918bda0dfa6070fcbb531472c42`  
		Last Modified: Fri, 16 Jun 2023 02:52:29 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312342ee3138b43b79d439dd69b91b51041cbf11d2916ef062d8d12c2cad8ee0`  
		Last Modified: Fri, 16 Jun 2023 05:51:57 GMT  
		Size: 233.7 MB (233732325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5612ff1d143fd5a97472ba8959c9a4da1f9db05cb0bca4f0baa7d43b2397c13`  
		Last Modified: Fri, 16 Jun 2023 05:51:48 GMT  
		Size: 4.3 KB (4334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabc9010d20e8019f412d0f2490fbf9605936d0eb8986ed5a4b8f498f289e3e7`  
		Last Modified: Fri, 16 Jun 2023 05:51:48 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bbae7a52b4721b7831fe3ea9659ba565f4ed7d01059285c914e18ccf10bfd6`  
		Last Modified: Fri, 16 Jun 2023 05:51:48 GMT  
		Size: 8.1 KB (8084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca77244d065f72458950fce89e5a6f6403da3d7b130c89bb9fe36881178e2ed6`  
		Last Modified: Fri, 16 Jun 2023 05:51:48 GMT  
		Size: 1.4 MB (1444005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.1.1` - linux; ppc64le

```console
$ docker pull solr@sha256:3d475a832984e044bb63c7d70a9b21d27cdc94447d2b9fb4d91d080a1fce8724
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.5 MB (338528985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:998c28a09a30f0c1858a1f6a14e389fc6f9c0378fcdac96f28b5dc18b40add2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:24 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:25 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:28 GMT
ADD file:0a2372ac4d43f0f4ada2b55dd0a359df73a828a9aa9426bfdd05a02b9c4b2bd9 in / 
# Mon, 05 Jun 2023 17:08:28 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:17:32 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:17:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:17:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:23:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:23:32 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:25:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:25:29 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 07:38:12 GMT
ARG SOLR_VERSION=9.1.1
# Fri, 16 Jun 2023 07:38:12 GMT
ARG SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f
# Fri, 16 Jun 2023 07:38:13 GMT
ARG SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763
# Fri, 16 Jun 2023 07:38:14 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 07:38:14 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 07:38:16 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 07:38:16 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 07:38:17 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Fri, 16 Jun 2023 07:39:09 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Fri, 16 Jun 2023 07:39:13 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 07:39:13 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 07:39:14 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 07:39:14 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 07:39:14 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 07:39:15 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 07:39:15 GMT
LABEL org.opencontainers.image.version=9.1.1
# Fri, 16 Jun 2023 07:39:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 07:39:16 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 07:39:19 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 07:39:20 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 07:39:22 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 07:39:35 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 07:39:36 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 07:39:37 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 07:39:38 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 07:39:38 GMT
USER 8983
# Fri, 16 Jun 2023 07:39:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 07:39:39 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:1fbda4a01aa9e184a223c30ab58441354cde30fe3083bc1d8ca9f7823ab4fe68`  
		Last Modified: Fri, 16 Jun 2023 01:24:20 GMT  
		Size: 33.3 MB (33309776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ad609b0dd14d25a533bad107d7d80f6a0143d184f80e43339a78811d5d58f6`  
		Last Modified: Fri, 16 Jun 2023 02:29:46 GMT  
		Size: 22.1 MB (22128326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11320ad109f515402d5d72270e3d40edc4ede3c81e18e8ffd54fb4f52f8e5e9`  
		Last Modified: Fri, 16 Jun 2023 02:31:04 GMT  
		Size: 46.9 MB (46872353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479808ab83f741c9d71794d5fcdf2fa889239fb3a46acdd165d94e11a2660437`  
		Last Modified: Fri, 16 Jun 2023 02:30:53 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3cefb506513f1817b42d49d48ef1360a4fb676a1d67decebb9a1a4c305b1348`  
		Last Modified: Fri, 16 Jun 2023 07:44:18 GMT  
		Size: 234.6 MB (234601456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6cff7bbc9114849bfffd3ff2844feef0da0f7cac82a0c4762e112bfcb4d3a6`  
		Last Modified: Fri, 16 Jun 2023 07:43:59 GMT  
		Size: 4.3 KB (4302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112c62e18932edc5d28d8afe0b1e7f9557d8b01bf3780db93f0ca157d8d54298`  
		Last Modified: Fri, 16 Jun 2023 07:43:59 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2134ceca5a4d10557e90ee4a622db03959055abb6b1f8d0651c1703a8d40464`  
		Last Modified: Fri, 16 Jun 2023 07:43:59 GMT  
		Size: 8.1 KB (8082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23143a1cb26656f63484c091ae88ef1c2a475c8581fb14d5db252cfbe933747`  
		Last Modified: Fri, 16 Jun 2023 07:43:59 GMT  
		Size: 1.6 MB (1604311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.1.1` - linux; s390x

```console
$ docker pull solr@sha256:e56a6fff2aa8bbc6fa79b57922f3443215b46e090999cd73c422572adf0a8b5b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.5 MB (325490601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9ed519da34ebadd2d4bce0da97eee7b903c08762396541e436095ee885829c9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:35 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:37 GMT
ADD file:44c66c03ba0afcc05de1b2078f83e8bfe04706b31491fcd3fdd93cfc88d5f06c in / 
# Thu, 13 Apr 2023 13:09:37 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:16:00 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:16:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:16:00 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:17:09 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:43:29 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:44:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:44:40 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:35:00 GMT
ARG SOLR_VERSION=9.1.1
# Wed, 26 Apr 2023 20:35:00 GMT
ARG SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f
# Wed, 26 Apr 2023 20:35:00 GMT
ARG SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763
# Wed, 26 Apr 2023 20:35:00 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:35:00 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:35:00 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz
# Wed, 26 Apr 2023 20:35:00 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Wed, 26 Apr 2023 20:35:01 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Wed, 26 Apr 2023 20:35:36 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Wed, 26 Apr 2023 20:35:41 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:35:41 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:35:41 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:35:41 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:35:41 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:35:42 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:35:42 GMT
LABEL org.opencontainers.image.version=9.1.1
# Wed, 26 Apr 2023 20:35:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:35:42 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:35:42 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:35:43 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:35:43 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:35:48 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:35:48 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:35:48 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:35:48 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:35:49 GMT
USER 8983
# Wed, 26 Apr 2023 20:35:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:35:49 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:f11b609b1d63f2d37c0e3789823e7a7e62a078bddca7c46da8602655989c62d9`  
		Last Modified: Fri, 14 Apr 2023 09:38:39 GMT  
		Size: 27.0 MB (27016370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf6c28f706c8f54c079ff27fe5409527f68c7463df6adf843d835f265547cf5`  
		Last Modified: Tue, 18 Apr 2023 01:19:02 GMT  
		Size: 19.5 MB (19532693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75157323f95569e14c082fe3aac39ef8f2f30ca3ad7d03107404eedde5396dbd`  
		Last Modified: Wed, 26 Apr 2023 19:48:03 GMT  
		Size: 43.8 MB (43775512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019b37c50f3b2d15194e9d039c46d5cd37c3f563d0a937909910fb7449a6430a`  
		Last Modified: Wed, 26 Apr 2023 19:47:57 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d94818969d07fed3dcf5a2ac39ac93d9dff860ec94f26640729a1bbd11d096e`  
		Last Modified: Wed, 26 Apr 2023 20:38:05 GMT  
		Size: 233.7 MB (233657251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911c96e0a2127384038700755982837f01f9814778a959e01b9f1f3f10aee4ac`  
		Last Modified: Wed, 26 Apr 2023 20:37:55 GMT  
		Size: 4.3 KB (4332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf10f7de9abf15f66ef7ffb2690123a6c55d2c264c29dd143b70e3d86b4befc0`  
		Last Modified: Wed, 26 Apr 2023 20:37:55 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c7e17cb3734a80d62f85e6e55dc722e83c2917e50fa3f29e27b6cd0b606ee2`  
		Last Modified: Wed, 26 Apr 2023 20:37:55 GMT  
		Size: 8.1 KB (8082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95125298d64bf04b588602df40d51bcd817b1cc5434864fd6c6273fcd0f0f924`  
		Last Modified: Wed, 26 Apr 2023 20:37:56 GMT  
		Size: 1.5 MB (1495981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:9.2`

```console
$ docker pull solr@sha256:73f4afe26d489830e59bf8db6e1e29a1adb86e4946b19d3db73fbc3684a1748f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `solr:9.2` - linux; amd64

```console
$ docker pull solr@sha256:e29c8b80f1864d67f40d0fbf9cc2dc080479abffd9a5cb4fcf12eea2759898c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **375.3 MB (375313008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee92e4df31178121b908f977309aa653980c8ead4c00a6456d7ef802bbd01816`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:15:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:15:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:15:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:18:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:18:30 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:19:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:19:05 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:26:45 GMT
ARG SOLR_VERSION=9.2.1
# Fri, 16 Jun 2023 05:26:45 GMT
ARG SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:27:05 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.version=9.2.1
# Fri, 16 Jun 2023 05:27:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 05:27:07 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 05:27:07 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:27:08 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 05:27:08 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 05:27:16 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 05:27:16 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:27:17 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:27:17 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:27:17 GMT
USER 8983
# Fri, 16 Jun 2023 05:27:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:27:17 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857412f02e8d49bb7e247b45ce86ce6378bd0bc5e8533e1fffa2a6e7a93aab46`  
		Last Modified: Fri, 16 Jun 2023 02:23:30 GMT  
		Size: 17.0 MB (17040964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f618ea570e7708381040c3f1662a8ff625710ddd7b5e0145b46bdf5231985c`  
		Last Modified: Fri, 16 Jun 2023 02:24:16 GMT  
		Size: 47.0 MB (47006286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2665c89972dd3400540a4420904c1912a3990b0a3be38d49d50a94b9da26231`  
		Last Modified: Fri, 16 Jun 2023 02:24:10 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42b38db22e6b18b3bc85f4e165ec99d95cf616e24a46a16b202a4d250561d3c`  
		Last Modified: Fri, 16 Jun 2023 05:30:50 GMT  
		Size: 279.0 MB (278994099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb98ce87480dfd3e75ac21f048446ae8df10c8dedff32cd9f263d02d1a825bf8`  
		Last Modified: Fri, 16 Jun 2023 05:30:38 GMT  
		Size: 4.3 KB (4288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a37d4231e60e1d0dc230f2efc9d2560cdc8dedf9e4b250d0818da3cee7def5`  
		Last Modified: Fri, 16 Jun 2023 05:30:38 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8928bcc26c2ef972e3082782ab6af19d2073d8e99c35453e7442950937d4f2b`  
		Last Modified: Fri, 16 Jun 2023 05:30:38 GMT  
		Size: 8.3 KB (8268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a14db093f859ab0b789c47440b60c02aee9d6a13e83e9b650a7b142280b4452`  
		Last Modified: Fri, 16 Jun 2023 05:30:39 GMT  
		Size: 1.8 MB (1827683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.2` - linux; arm variant v7

```console
$ docker pull solr@sha256:df5a4df27d6223472cdf39d015d0be71d2e3674169077c668259410ac9ed2f20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **369.4 MB (369434561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90d9b6bd34c3e1002a86e117f66e584a416854d27e7c66f806f1a01cf6d15fd8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 16:59:35 GMT
ARG RELEASE
# Mon, 05 Jun 2023 16:59:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 16:59:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 16:59:35 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 16:59:40 GMT
ADD file:5425962ced738173a50965fc5cd95c79d0a319323df4a34e9da3f5037a5264c3 in / 
# Mon, 05 Jun 2023 16:59:40 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:25:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 01:25:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 01:25:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 01:28:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:28:03 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 01:28:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 01:28:33 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 02:38:27 GMT
ARG SOLR_VERSION=9.2.1
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 02:38:52 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 02:38:55 GMT
LABEL org.opencontainers.image.version=9.2.1
# Fri, 16 Jun 2023 02:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 02:38:55 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 02:38:55 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 02:38:56 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 02:38:56 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 02:39:05 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 02:39:05 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 02:39:05 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 02:39:05 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 02:39:05 GMT
USER 8983
# Fri, 16 Jun 2023 02:39:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 02:39:06 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:de11f41b5c8ee0d3b259584977df4adb3e9b005f95756baecf491f70b498f301`  
		Last Modified: Wed, 07 Jun 2023 02:07:45 GMT  
		Size: 27.0 MB (27026252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88eb1b8897047cd0a4d969ca49bb4696512a41ef9d4466bc36e6bb42d97ca8dd`  
		Last Modified: Fri, 16 Jun 2023 01:31:49 GMT  
		Size: 17.2 MB (17168477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4e9b19cfde4210390e27af028b3821849f4637891e197e449641eb7824c5e1`  
		Last Modified: Fri, 16 Jun 2023 01:32:33 GMT  
		Size: 44.6 MB (44579970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69809a3884cff3cd2a14f35fede7e33256861cf01f1afb3f2fe52660b7fbfb72`  
		Last Modified: Fri, 16 Jun 2023 01:32:26 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15016717bbccbb8afaa8cd53f43070ec0fc4ccd1229c858a599c76179c0fee9`  
		Last Modified: Fri, 16 Jun 2023 02:42:49 GMT  
		Size: 279.0 MB (278994307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df6c3913894e2b72c13f2694b8975504ad21fcec95c266e2f9b3fe81c6c7846`  
		Last Modified: Fri, 16 Jun 2023 02:42:34 GMT  
		Size: 4.2 KB (4223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e043faaa195146204f1395ba9ffff82c7db8ad8bceb6342ba54add360a69a15c`  
		Last Modified: Fri, 16 Jun 2023 02:42:34 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a294eea0d8dce46694f985b5876d7480e52e3ab622133cca6771a36dcb330c`  
		Last Modified: Fri, 16 Jun 2023 02:42:34 GMT  
		Size: 8.3 KB (8265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32ce8d699bbfad8bd6eb33cb5bcbbe23ce1c33711b92eb2055125082aeda9d8`  
		Last Modified: Fri, 16 Jun 2023 02:42:35 GMT  
		Size: 1.7 MB (1652690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.2` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:66509e3fc448ac1d4772e7d726c2cf22fe0d4967714e3c65afe9c65c4a495621
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.0 MB (374038205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd904f26d14316cf21764a5752c2ec1106c1a2bd920731c901a018585999f16d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:45:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:45:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:45:39 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:47:57 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:47:57 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:48:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:48:26 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:47:48 GMT
ARG SOLR_VERSION=9.2.1
# Fri, 16 Jun 2023 05:47:48 GMT
ARG SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:48:04 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.version=9.2.1
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 05:48:06 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 05:48:07 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:48:07 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 05:48:08 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 05:48:16 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 05:48:16 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:48:16 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:48:16 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:48:16 GMT
USER 8983
# Fri, 16 Jun 2023 05:48:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:48:16 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5168066327b37e44f2a0ef7f788219bdbcd9013e4320cf4b9229ea9dfb73b561`  
		Last Modified: Fri, 16 Jun 2023 02:52:08 GMT  
		Size: 18.5 MB (18465563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78b269707ca01885483219b119ab6f03209c4c452696f1dcf105d191a7115cb`  
		Last Modified: Fri, 16 Jun 2023 02:52:47 GMT  
		Size: 46.5 MB (46488623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb861b98c25f139f6cf3783bb0c0c5a4810ad99eaba8cf8695eefe7f8614a8b`  
		Last Modified: Fri, 16 Jun 2023 02:52:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3400a3f980bb2b3adf154d3fc86f306788ac6cff76728fde865037e3ede88b68`  
		Last Modified: Fri, 16 Jun 2023 05:51:36 GMT  
		Size: 279.0 MB (278994703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11950a4bc9f97d203c1476552d153fcc683e3957621da8768cd3fa39ee02d0eb`  
		Last Modified: Fri, 16 Jun 2023 05:51:26 GMT  
		Size: 4.3 KB (4331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042db7dc8c2d6e3b53376afc669becc9ca9910f7044388ce3d98ff880351321f`  
		Last Modified: Fri, 16 Jun 2023 05:51:26 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fec7819b9a55bdc72dd442a462e31fbe1414cadd44f1bcd765716dd6b4e3c622`  
		Last Modified: Fri, 16 Jun 2023 05:51:26 GMT  
		Size: 8.3 KB (8269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da205b415c9da2bcf6f1d7532f914f0bd453728f8ec6beba5eb09cfd86cb27f`  
		Last Modified: Fri, 16 Jun 2023 05:51:27 GMT  
		Size: 1.7 MB (1687137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.2` - linux; ppc64le

```console
$ docker pull solr@sha256:7237335d603e527c83ab9545e0865684521980f5c406a28d58969c7c6e58e70b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.7 MB (381748792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3b61810d471dd4c39d87767e32a88170d6f0d0a3cf37eb7eb200614ba8e14db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:01:00 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:01:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:01:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:01:01 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:01:03 GMT
ADD file:00c4f44b35b683caef54d5b8b0e0b1e68872f45eae17dd7543adaf6c54512447 in / 
# Mon, 05 Jun 2023 17:01:04 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:19:12 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:19:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:19:13 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:24:42 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:24:43 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:25:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:25:43 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 07:36:03 GMT
ARG SOLR_VERSION=9.2.1
# Fri, 16 Jun 2023 07:36:04 GMT
ARG SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb
# Fri, 16 Jun 2023 07:36:04 GMT
ARG SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271
# Fri, 16 Jun 2023 07:36:05 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 07:36:05 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 07:36:05 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 07:36:06 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 07:36:06 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 07:37:24 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 16 Jun 2023 07:37:29 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 07:37:29 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 07:37:30 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 07:37:30 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 07:37:31 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 07:37:32 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 07:37:35 GMT
LABEL org.opencontainers.image.version=9.2.1
# Fri, 16 Jun 2023 07:37:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 07:37:37 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 07:37:39 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 07:37:41 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 07:37:43 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 07:38:00 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 07:38:00 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 07:38:01 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 07:38:01 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 07:38:02 GMT
USER 8983
# Fri, 16 Jun 2023 07:38:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 07:38:03 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:a02dd69d9a8a1e6f4fc2ccb509fb8efd6014b00ff932a757d23b4b012a2bec49`  
		Last Modified: Fri, 16 Jun 2023 00:44:52 GMT  
		Size: 35.7 MB (35711397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bd55325dd69030064f13098489df6ef8e45b2d52baffb366675c06f6e94418`  
		Last Modified: Fri, 16 Jun 2023 02:30:20 GMT  
		Size: 18.3 MB (18322826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef75c435e36e0d0cb9911afc443c4bf6c1769b56642390039838f6017497b2f`  
		Last Modified: Fri, 16 Jun 2023 02:31:24 GMT  
		Size: 46.9 MB (46872498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edff0610bd2e6e17f260f10d236a0fad32db564c59f810b5e30eaee37ef5faf8`  
		Last Modified: Fri, 16 Jun 2023 02:31:13 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d7ebdacee82ac6455d940b19d21bf659f1cf53c3aaa3f3e1577135b8802d3e`  
		Last Modified: Fri, 16 Jun 2023 07:43:45 GMT  
		Size: 279.0 MB (278994934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64708f76d121ff3c1262875272f841e9c3bb2244f1d305672fed751d7c638df1`  
		Last Modified: Fri, 16 Jun 2023 07:43:24 GMT  
		Size: 4.3 KB (4297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495b3eb13c2abbf80d9c705cdb460f2f939de60c92c610848a2c4defab47dd11`  
		Last Modified: Fri, 16 Jun 2023 07:43:24 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8695e9bc13470e29cd835a938319952511edd7c991fecadf3ed9d64c89a727b`  
		Last Modified: Fri, 16 Jun 2023 07:43:24 GMT  
		Size: 8.3 KB (8273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3227aa649395d114eef9c32c931462d8a75c9fe23aa39081891ddc6dc3c31c74`  
		Last Modified: Fri, 16 Jun 2023 07:43:25 GMT  
		Size: 1.8 MB (1834188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.2` - linux; s390x

```console
$ docker pull solr@sha256:2e2e1090eeb5e9008c115e614650f992c607ac460b8d848c6bcf4c5fbdfa2f09
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **370.0 MB (370021779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f06f08b94cb5330a7ff42794eee64cc602fd8b2713258fcdb3ca2001d12c0e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 22 May 2023 17:46:45 GMT
ARG RELEASE
# Mon, 22 May 2023 17:46:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 22 May 2023 17:46:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 22 May 2023 17:46:45 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 22 May 2023 17:46:47 GMT
ADD file:7bf1b7a1484e37f289d40f5c1c1cbe321ef337f898dd3d5809193c848a9a3dc2 in / 
# Mon, 22 May 2023 17:46:47 GMT
CMD ["/bin/bash"]
# Thu, 01 Jun 2023 23:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 01 Jun 2023 23:33:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Jun 2023 23:33:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 01 Jun 2023 23:34:41 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 01 Jun 2023 23:34:43 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Thu, 01 Jun 2023 23:35:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 01 Jun 2023 23:35:21 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_VERSION=9.2.1
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 02 Jun 2023 15:53:16 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 02 Jun 2023 15:53:20 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 02 Jun 2023 15:53:20 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.version=9.2.1
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 02 Jun 2023 15:53:21 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 02 Jun 2023 15:53:21 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 02 Jun 2023 15:53:22 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 02 Jun 2023 15:53:22 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 02 Jun 2023 15:53:27 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 02 Jun 2023 15:53:27 GMT
VOLUME [/var/solr]
# Fri, 02 Jun 2023 15:53:27 GMT
EXPOSE 8983
# Fri, 02 Jun 2023 15:53:27 GMT
WORKDIR /opt/solr
# Fri, 02 Jun 2023 15:53:28 GMT
USER 8983
# Fri, 02 Jun 2023 15:53:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Jun 2023 15:53:28 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:f2957179c3a13374d05630725d1d996f8083efadf7d2da999c9b4ca53ab7c98f`  
		Last Modified: Thu, 01 Jun 2023 23:19:06 GMT  
		Size: 28.6 MB (28648005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff49023eb8231a4489c04787627471c943342afea6aed42b66e0bd17f75307a`  
		Last Modified: Thu, 01 Jun 2023 23:36:33 GMT  
		Size: 16.8 MB (16817675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58123ce9cafda91814be25f8b9b9f99431886cfbee190fc6ba7f6be9abdfe781`  
		Last Modified: Thu, 01 Jun 2023 23:36:56 GMT  
		Size: 43.8 MB (43774489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c27d78a58220d69494be2a17dffa9c4de667bdcf0f6e85c869482d832b8af8f`  
		Last Modified: Thu, 01 Jun 2023 23:36:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeab0826386b334263843df3860f46ec4cb1baa7490d55f653630de11aefecb2`  
		Last Modified: Fri, 02 Jun 2023 15:54:19 GMT  
		Size: 279.0 MB (278994275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5f2afb9fbda66fff0a22400f8df154060d0f1d74944a07653c6466fb541622`  
		Last Modified: Fri, 02 Jun 2023 15:54:08 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b24eb5989fbe19cfbfa7fade0c611dd880bd9f279f3960ce96ca5a35e4188ad`  
		Last Modified: Fri, 02 Jun 2023 15:54:08 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fbd279dbd567d795f616c80182d1ea59f0584002dcd56265accfa296ec81551`  
		Last Modified: Fri, 02 Jun 2023 15:54:08 GMT  
		Size: 8.3 KB (8265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf0d1005aca634a3af1af7d7165552463412e8d705e08a29aec622534e2987f`  
		Last Modified: Fri, 02 Jun 2023 15:54:08 GMT  
		Size: 1.8 MB (1774360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:9.2.1`

```console
$ docker pull solr@sha256:73f4afe26d489830e59bf8db6e1e29a1adb86e4946b19d3db73fbc3684a1748f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `solr:9.2.1` - linux; amd64

```console
$ docker pull solr@sha256:e29c8b80f1864d67f40d0fbf9cc2dc080479abffd9a5cb4fcf12eea2759898c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **375.3 MB (375313008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee92e4df31178121b908f977309aa653980c8ead4c00a6456d7ef802bbd01816`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:15:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:15:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:15:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:18:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:18:30 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:19:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:19:05 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:26:45 GMT
ARG SOLR_VERSION=9.2.1
# Fri, 16 Jun 2023 05:26:45 GMT
ARG SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:27:05 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.version=9.2.1
# Fri, 16 Jun 2023 05:27:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 05:27:07 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 05:27:07 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:27:08 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 05:27:08 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 05:27:16 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 05:27:16 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:27:17 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:27:17 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:27:17 GMT
USER 8983
# Fri, 16 Jun 2023 05:27:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:27:17 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857412f02e8d49bb7e247b45ce86ce6378bd0bc5e8533e1fffa2a6e7a93aab46`  
		Last Modified: Fri, 16 Jun 2023 02:23:30 GMT  
		Size: 17.0 MB (17040964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f618ea570e7708381040c3f1662a8ff625710ddd7b5e0145b46bdf5231985c`  
		Last Modified: Fri, 16 Jun 2023 02:24:16 GMT  
		Size: 47.0 MB (47006286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2665c89972dd3400540a4420904c1912a3990b0a3be38d49d50a94b9da26231`  
		Last Modified: Fri, 16 Jun 2023 02:24:10 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42b38db22e6b18b3bc85f4e165ec99d95cf616e24a46a16b202a4d250561d3c`  
		Last Modified: Fri, 16 Jun 2023 05:30:50 GMT  
		Size: 279.0 MB (278994099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb98ce87480dfd3e75ac21f048446ae8df10c8dedff32cd9f263d02d1a825bf8`  
		Last Modified: Fri, 16 Jun 2023 05:30:38 GMT  
		Size: 4.3 KB (4288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a37d4231e60e1d0dc230f2efc9d2560cdc8dedf9e4b250d0818da3cee7def5`  
		Last Modified: Fri, 16 Jun 2023 05:30:38 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8928bcc26c2ef972e3082782ab6af19d2073d8e99c35453e7442950937d4f2b`  
		Last Modified: Fri, 16 Jun 2023 05:30:38 GMT  
		Size: 8.3 KB (8268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a14db093f859ab0b789c47440b60c02aee9d6a13e83e9b650a7b142280b4452`  
		Last Modified: Fri, 16 Jun 2023 05:30:39 GMT  
		Size: 1.8 MB (1827683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.2.1` - linux; arm variant v7

```console
$ docker pull solr@sha256:df5a4df27d6223472cdf39d015d0be71d2e3674169077c668259410ac9ed2f20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **369.4 MB (369434561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90d9b6bd34c3e1002a86e117f66e584a416854d27e7c66f806f1a01cf6d15fd8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 16:59:35 GMT
ARG RELEASE
# Mon, 05 Jun 2023 16:59:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 16:59:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 16:59:35 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 16:59:40 GMT
ADD file:5425962ced738173a50965fc5cd95c79d0a319323df4a34e9da3f5037a5264c3 in / 
# Mon, 05 Jun 2023 16:59:40 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:25:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 01:25:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 01:25:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 01:28:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:28:03 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 01:28:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 01:28:33 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 02:38:27 GMT
ARG SOLR_VERSION=9.2.1
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 02:38:52 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 02:38:55 GMT
LABEL org.opencontainers.image.version=9.2.1
# Fri, 16 Jun 2023 02:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 02:38:55 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 02:38:55 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 02:38:56 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 02:38:56 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 02:39:05 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 02:39:05 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 02:39:05 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 02:39:05 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 02:39:05 GMT
USER 8983
# Fri, 16 Jun 2023 02:39:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 02:39:06 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:de11f41b5c8ee0d3b259584977df4adb3e9b005f95756baecf491f70b498f301`  
		Last Modified: Wed, 07 Jun 2023 02:07:45 GMT  
		Size: 27.0 MB (27026252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88eb1b8897047cd0a4d969ca49bb4696512a41ef9d4466bc36e6bb42d97ca8dd`  
		Last Modified: Fri, 16 Jun 2023 01:31:49 GMT  
		Size: 17.2 MB (17168477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4e9b19cfde4210390e27af028b3821849f4637891e197e449641eb7824c5e1`  
		Last Modified: Fri, 16 Jun 2023 01:32:33 GMT  
		Size: 44.6 MB (44579970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69809a3884cff3cd2a14f35fede7e33256861cf01f1afb3f2fe52660b7fbfb72`  
		Last Modified: Fri, 16 Jun 2023 01:32:26 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15016717bbccbb8afaa8cd53f43070ec0fc4ccd1229c858a599c76179c0fee9`  
		Last Modified: Fri, 16 Jun 2023 02:42:49 GMT  
		Size: 279.0 MB (278994307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df6c3913894e2b72c13f2694b8975504ad21fcec95c266e2f9b3fe81c6c7846`  
		Last Modified: Fri, 16 Jun 2023 02:42:34 GMT  
		Size: 4.2 KB (4223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e043faaa195146204f1395ba9ffff82c7db8ad8bceb6342ba54add360a69a15c`  
		Last Modified: Fri, 16 Jun 2023 02:42:34 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a294eea0d8dce46694f985b5876d7480e52e3ab622133cca6771a36dcb330c`  
		Last Modified: Fri, 16 Jun 2023 02:42:34 GMT  
		Size: 8.3 KB (8265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32ce8d699bbfad8bd6eb33cb5bcbbe23ce1c33711b92eb2055125082aeda9d8`  
		Last Modified: Fri, 16 Jun 2023 02:42:35 GMT  
		Size: 1.7 MB (1652690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.2.1` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:66509e3fc448ac1d4772e7d726c2cf22fe0d4967714e3c65afe9c65c4a495621
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.0 MB (374038205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd904f26d14316cf21764a5752c2ec1106c1a2bd920731c901a018585999f16d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:45:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:45:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:45:39 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:47:57 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:47:57 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:48:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:48:26 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:47:48 GMT
ARG SOLR_VERSION=9.2.1
# Fri, 16 Jun 2023 05:47:48 GMT
ARG SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:48:04 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.version=9.2.1
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 05:48:06 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 05:48:07 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:48:07 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 05:48:08 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 05:48:16 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 05:48:16 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:48:16 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:48:16 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:48:16 GMT
USER 8983
# Fri, 16 Jun 2023 05:48:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:48:16 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5168066327b37e44f2a0ef7f788219bdbcd9013e4320cf4b9229ea9dfb73b561`  
		Last Modified: Fri, 16 Jun 2023 02:52:08 GMT  
		Size: 18.5 MB (18465563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78b269707ca01885483219b119ab6f03209c4c452696f1dcf105d191a7115cb`  
		Last Modified: Fri, 16 Jun 2023 02:52:47 GMT  
		Size: 46.5 MB (46488623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb861b98c25f139f6cf3783bb0c0c5a4810ad99eaba8cf8695eefe7f8614a8b`  
		Last Modified: Fri, 16 Jun 2023 02:52:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3400a3f980bb2b3adf154d3fc86f306788ac6cff76728fde865037e3ede88b68`  
		Last Modified: Fri, 16 Jun 2023 05:51:36 GMT  
		Size: 279.0 MB (278994703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11950a4bc9f97d203c1476552d153fcc683e3957621da8768cd3fa39ee02d0eb`  
		Last Modified: Fri, 16 Jun 2023 05:51:26 GMT  
		Size: 4.3 KB (4331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042db7dc8c2d6e3b53376afc669becc9ca9910f7044388ce3d98ff880351321f`  
		Last Modified: Fri, 16 Jun 2023 05:51:26 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fec7819b9a55bdc72dd442a462e31fbe1414cadd44f1bcd765716dd6b4e3c622`  
		Last Modified: Fri, 16 Jun 2023 05:51:26 GMT  
		Size: 8.3 KB (8269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da205b415c9da2bcf6f1d7532f914f0bd453728f8ec6beba5eb09cfd86cb27f`  
		Last Modified: Fri, 16 Jun 2023 05:51:27 GMT  
		Size: 1.7 MB (1687137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.2.1` - linux; ppc64le

```console
$ docker pull solr@sha256:7237335d603e527c83ab9545e0865684521980f5c406a28d58969c7c6e58e70b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.7 MB (381748792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3b61810d471dd4c39d87767e32a88170d6f0d0a3cf37eb7eb200614ba8e14db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:01:00 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:01:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:01:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:01:01 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:01:03 GMT
ADD file:00c4f44b35b683caef54d5b8b0e0b1e68872f45eae17dd7543adaf6c54512447 in / 
# Mon, 05 Jun 2023 17:01:04 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:19:12 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:19:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:19:13 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:24:42 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:24:43 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:25:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:25:43 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 07:36:03 GMT
ARG SOLR_VERSION=9.2.1
# Fri, 16 Jun 2023 07:36:04 GMT
ARG SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb
# Fri, 16 Jun 2023 07:36:04 GMT
ARG SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271
# Fri, 16 Jun 2023 07:36:05 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 07:36:05 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 07:36:05 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 07:36:06 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 07:36:06 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 07:37:24 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 16 Jun 2023 07:37:29 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 07:37:29 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 07:37:30 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 07:37:30 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 07:37:31 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 07:37:32 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 07:37:35 GMT
LABEL org.opencontainers.image.version=9.2.1
# Fri, 16 Jun 2023 07:37:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 07:37:37 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 07:37:39 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 07:37:41 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 07:37:43 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 07:38:00 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 07:38:00 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 07:38:01 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 07:38:01 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 07:38:02 GMT
USER 8983
# Fri, 16 Jun 2023 07:38:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 07:38:03 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:a02dd69d9a8a1e6f4fc2ccb509fb8efd6014b00ff932a757d23b4b012a2bec49`  
		Last Modified: Fri, 16 Jun 2023 00:44:52 GMT  
		Size: 35.7 MB (35711397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bd55325dd69030064f13098489df6ef8e45b2d52baffb366675c06f6e94418`  
		Last Modified: Fri, 16 Jun 2023 02:30:20 GMT  
		Size: 18.3 MB (18322826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef75c435e36e0d0cb9911afc443c4bf6c1769b56642390039838f6017497b2f`  
		Last Modified: Fri, 16 Jun 2023 02:31:24 GMT  
		Size: 46.9 MB (46872498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edff0610bd2e6e17f260f10d236a0fad32db564c59f810b5e30eaee37ef5faf8`  
		Last Modified: Fri, 16 Jun 2023 02:31:13 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d7ebdacee82ac6455d940b19d21bf659f1cf53c3aaa3f3e1577135b8802d3e`  
		Last Modified: Fri, 16 Jun 2023 07:43:45 GMT  
		Size: 279.0 MB (278994934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64708f76d121ff3c1262875272f841e9c3bb2244f1d305672fed751d7c638df1`  
		Last Modified: Fri, 16 Jun 2023 07:43:24 GMT  
		Size: 4.3 KB (4297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495b3eb13c2abbf80d9c705cdb460f2f939de60c92c610848a2c4defab47dd11`  
		Last Modified: Fri, 16 Jun 2023 07:43:24 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8695e9bc13470e29cd835a938319952511edd7c991fecadf3ed9d64c89a727b`  
		Last Modified: Fri, 16 Jun 2023 07:43:24 GMT  
		Size: 8.3 KB (8273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3227aa649395d114eef9c32c931462d8a75c9fe23aa39081891ddc6dc3c31c74`  
		Last Modified: Fri, 16 Jun 2023 07:43:25 GMT  
		Size: 1.8 MB (1834188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.2.1` - linux; s390x

```console
$ docker pull solr@sha256:2e2e1090eeb5e9008c115e614650f992c607ac460b8d848c6bcf4c5fbdfa2f09
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **370.0 MB (370021779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f06f08b94cb5330a7ff42794eee64cc602fd8b2713258fcdb3ca2001d12c0e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 22 May 2023 17:46:45 GMT
ARG RELEASE
# Mon, 22 May 2023 17:46:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 22 May 2023 17:46:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 22 May 2023 17:46:45 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 22 May 2023 17:46:47 GMT
ADD file:7bf1b7a1484e37f289d40f5c1c1cbe321ef337f898dd3d5809193c848a9a3dc2 in / 
# Mon, 22 May 2023 17:46:47 GMT
CMD ["/bin/bash"]
# Thu, 01 Jun 2023 23:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 01 Jun 2023 23:33:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Jun 2023 23:33:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 01 Jun 2023 23:34:41 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 01 Jun 2023 23:34:43 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Thu, 01 Jun 2023 23:35:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 01 Jun 2023 23:35:21 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_VERSION=9.2.1
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 02 Jun 2023 15:53:16 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 02 Jun 2023 15:53:20 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 02 Jun 2023 15:53:20 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.version=9.2.1
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 02 Jun 2023 15:53:21 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 02 Jun 2023 15:53:21 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 02 Jun 2023 15:53:22 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 02 Jun 2023 15:53:22 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 02 Jun 2023 15:53:27 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 02 Jun 2023 15:53:27 GMT
VOLUME [/var/solr]
# Fri, 02 Jun 2023 15:53:27 GMT
EXPOSE 8983
# Fri, 02 Jun 2023 15:53:27 GMT
WORKDIR /opt/solr
# Fri, 02 Jun 2023 15:53:28 GMT
USER 8983
# Fri, 02 Jun 2023 15:53:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Jun 2023 15:53:28 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:f2957179c3a13374d05630725d1d996f8083efadf7d2da999c9b4ca53ab7c98f`  
		Last Modified: Thu, 01 Jun 2023 23:19:06 GMT  
		Size: 28.6 MB (28648005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff49023eb8231a4489c04787627471c943342afea6aed42b66e0bd17f75307a`  
		Last Modified: Thu, 01 Jun 2023 23:36:33 GMT  
		Size: 16.8 MB (16817675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58123ce9cafda91814be25f8b9b9f99431886cfbee190fc6ba7f6be9abdfe781`  
		Last Modified: Thu, 01 Jun 2023 23:36:56 GMT  
		Size: 43.8 MB (43774489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c27d78a58220d69494be2a17dffa9c4de667bdcf0f6e85c869482d832b8af8f`  
		Last Modified: Thu, 01 Jun 2023 23:36:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeab0826386b334263843df3860f46ec4cb1baa7490d55f653630de11aefecb2`  
		Last Modified: Fri, 02 Jun 2023 15:54:19 GMT  
		Size: 279.0 MB (278994275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5f2afb9fbda66fff0a22400f8df154060d0f1d74944a07653c6466fb541622`  
		Last Modified: Fri, 02 Jun 2023 15:54:08 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b24eb5989fbe19cfbfa7fade0c611dd880bd9f279f3960ce96ca5a35e4188ad`  
		Last Modified: Fri, 02 Jun 2023 15:54:08 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fbd279dbd567d795f616c80182d1ea59f0584002dcd56265accfa296ec81551`  
		Last Modified: Fri, 02 Jun 2023 15:54:08 GMT  
		Size: 8.3 KB (8265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf0d1005aca634a3af1af7d7165552463412e8d705e08a29aec622534e2987f`  
		Last Modified: Fri, 02 Jun 2023 15:54:08 GMT  
		Size: 1.8 MB (1774360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:latest`

```console
$ docker pull solr@sha256:73f4afe26d489830e59bf8db6e1e29a1adb86e4946b19d3db73fbc3684a1748f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `solr:latest` - linux; amd64

```console
$ docker pull solr@sha256:e29c8b80f1864d67f40d0fbf9cc2dc080479abffd9a5cb4fcf12eea2759898c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **375.3 MB (375313008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee92e4df31178121b908f977309aa653980c8ead4c00a6456d7ef802bbd01816`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:15:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:15:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:15:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:18:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:18:30 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:19:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:19:05 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:26:45 GMT
ARG SOLR_VERSION=9.2.1
# Fri, 16 Jun 2023 05:26:45 GMT
ARG SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:26:46 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:27:05 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 05:27:06 GMT
LABEL org.opencontainers.image.version=9.2.1
# Fri, 16 Jun 2023 05:27:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 05:27:07 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 05:27:07 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:27:08 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 05:27:08 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 05:27:16 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 05:27:16 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:27:17 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:27:17 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:27:17 GMT
USER 8983
# Fri, 16 Jun 2023 05:27:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:27:17 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857412f02e8d49bb7e247b45ce86ce6378bd0bc5e8533e1fffa2a6e7a93aab46`  
		Last Modified: Fri, 16 Jun 2023 02:23:30 GMT  
		Size: 17.0 MB (17040964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f618ea570e7708381040c3f1662a8ff625710ddd7b5e0145b46bdf5231985c`  
		Last Modified: Fri, 16 Jun 2023 02:24:16 GMT  
		Size: 47.0 MB (47006286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2665c89972dd3400540a4420904c1912a3990b0a3be38d49d50a94b9da26231`  
		Last Modified: Fri, 16 Jun 2023 02:24:10 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42b38db22e6b18b3bc85f4e165ec99d95cf616e24a46a16b202a4d250561d3c`  
		Last Modified: Fri, 16 Jun 2023 05:30:50 GMT  
		Size: 279.0 MB (278994099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb98ce87480dfd3e75ac21f048446ae8df10c8dedff32cd9f263d02d1a825bf8`  
		Last Modified: Fri, 16 Jun 2023 05:30:38 GMT  
		Size: 4.3 KB (4288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a37d4231e60e1d0dc230f2efc9d2560cdc8dedf9e4b250d0818da3cee7def5`  
		Last Modified: Fri, 16 Jun 2023 05:30:38 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8928bcc26c2ef972e3082782ab6af19d2073d8e99c35453e7442950937d4f2b`  
		Last Modified: Fri, 16 Jun 2023 05:30:38 GMT  
		Size: 8.3 KB (8268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a14db093f859ab0b789c47440b60c02aee9d6a13e83e9b650a7b142280b4452`  
		Last Modified: Fri, 16 Jun 2023 05:30:39 GMT  
		Size: 1.8 MB (1827683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:latest` - linux; arm variant v7

```console
$ docker pull solr@sha256:df5a4df27d6223472cdf39d015d0be71d2e3674169077c668259410ac9ed2f20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **369.4 MB (369434561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90d9b6bd34c3e1002a86e117f66e584a416854d27e7c66f806f1a01cf6d15fd8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 16:59:35 GMT
ARG RELEASE
# Mon, 05 Jun 2023 16:59:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 16:59:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 16:59:35 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 16:59:40 GMT
ADD file:5425962ced738173a50965fc5cd95c79d0a319323df4a34e9da3f5037a5264c3 in / 
# Mon, 05 Jun 2023 16:59:40 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:25:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 01:25:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 01:25:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 01:28:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:28:03 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 01:28:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 01:28:33 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 02:38:27 GMT
ARG SOLR_VERSION=9.2.1
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 02:38:28 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 02:38:52 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 02:38:54 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 02:38:55 GMT
LABEL org.opencontainers.image.version=9.2.1
# Fri, 16 Jun 2023 02:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 02:38:55 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 02:38:55 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 02:38:56 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 02:38:56 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 02:39:05 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 02:39:05 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 02:39:05 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 02:39:05 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 02:39:05 GMT
USER 8983
# Fri, 16 Jun 2023 02:39:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 02:39:06 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:de11f41b5c8ee0d3b259584977df4adb3e9b005f95756baecf491f70b498f301`  
		Last Modified: Wed, 07 Jun 2023 02:07:45 GMT  
		Size: 27.0 MB (27026252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88eb1b8897047cd0a4d969ca49bb4696512a41ef9d4466bc36e6bb42d97ca8dd`  
		Last Modified: Fri, 16 Jun 2023 01:31:49 GMT  
		Size: 17.2 MB (17168477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4e9b19cfde4210390e27af028b3821849f4637891e197e449641eb7824c5e1`  
		Last Modified: Fri, 16 Jun 2023 01:32:33 GMT  
		Size: 44.6 MB (44579970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69809a3884cff3cd2a14f35fede7e33256861cf01f1afb3f2fe52660b7fbfb72`  
		Last Modified: Fri, 16 Jun 2023 01:32:26 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15016717bbccbb8afaa8cd53f43070ec0fc4ccd1229c858a599c76179c0fee9`  
		Last Modified: Fri, 16 Jun 2023 02:42:49 GMT  
		Size: 279.0 MB (278994307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df6c3913894e2b72c13f2694b8975504ad21fcec95c266e2f9b3fe81c6c7846`  
		Last Modified: Fri, 16 Jun 2023 02:42:34 GMT  
		Size: 4.2 KB (4223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e043faaa195146204f1395ba9ffff82c7db8ad8bceb6342ba54add360a69a15c`  
		Last Modified: Fri, 16 Jun 2023 02:42:34 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a294eea0d8dce46694f985b5876d7480e52e3ab622133cca6771a36dcb330c`  
		Last Modified: Fri, 16 Jun 2023 02:42:34 GMT  
		Size: 8.3 KB (8265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32ce8d699bbfad8bd6eb33cb5bcbbe23ce1c33711b92eb2055125082aeda9d8`  
		Last Modified: Fri, 16 Jun 2023 02:42:35 GMT  
		Size: 1.7 MB (1652690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:latest` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:66509e3fc448ac1d4772e7d726c2cf22fe0d4967714e3c65afe9c65c4a495621
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.0 MB (374038205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd904f26d14316cf21764a5752c2ec1106c1a2bd920731c901a018585999f16d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:45:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:45:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:45:39 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:47:57 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:47:57 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:48:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:48:26 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 05:47:48 GMT
ARG SOLR_VERSION=9.2.1
# Fri, 16 Jun 2023 05:47:48 GMT
ARG SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:47:49 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 05:48:04 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.version=9.2.1
# Fri, 16 Jun 2023 05:48:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 05:48:06 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 05:48:07 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 05:48:07 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 05:48:08 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 05:48:16 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 05:48:16 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 05:48:16 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 05:48:16 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 05:48:16 GMT
USER 8983
# Fri, 16 Jun 2023 05:48:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 05:48:16 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5168066327b37e44f2a0ef7f788219bdbcd9013e4320cf4b9229ea9dfb73b561`  
		Last Modified: Fri, 16 Jun 2023 02:52:08 GMT  
		Size: 18.5 MB (18465563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78b269707ca01885483219b119ab6f03209c4c452696f1dcf105d191a7115cb`  
		Last Modified: Fri, 16 Jun 2023 02:52:47 GMT  
		Size: 46.5 MB (46488623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb861b98c25f139f6cf3783bb0c0c5a4810ad99eaba8cf8695eefe7f8614a8b`  
		Last Modified: Fri, 16 Jun 2023 02:52:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3400a3f980bb2b3adf154d3fc86f306788ac6cff76728fde865037e3ede88b68`  
		Last Modified: Fri, 16 Jun 2023 05:51:36 GMT  
		Size: 279.0 MB (278994703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11950a4bc9f97d203c1476552d153fcc683e3957621da8768cd3fa39ee02d0eb`  
		Last Modified: Fri, 16 Jun 2023 05:51:26 GMT  
		Size: 4.3 KB (4331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042db7dc8c2d6e3b53376afc669becc9ca9910f7044388ce3d98ff880351321f`  
		Last Modified: Fri, 16 Jun 2023 05:51:26 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fec7819b9a55bdc72dd442a462e31fbe1414cadd44f1bcd765716dd6b4e3c622`  
		Last Modified: Fri, 16 Jun 2023 05:51:26 GMT  
		Size: 8.3 KB (8269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da205b415c9da2bcf6f1d7532f914f0bd453728f8ec6beba5eb09cfd86cb27f`  
		Last Modified: Fri, 16 Jun 2023 05:51:27 GMT  
		Size: 1.7 MB (1687137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:latest` - linux; ppc64le

```console
$ docker pull solr@sha256:7237335d603e527c83ab9545e0865684521980f5c406a28d58969c7c6e58e70b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.7 MB (381748792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3b61810d471dd4c39d87767e32a88170d6f0d0a3cf37eb7eb200614ba8e14db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 05 Jun 2023 17:01:00 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:01:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:01:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:01:01 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:01:03 GMT
ADD file:00c4f44b35b683caef54d5b8b0e0b1e68872f45eae17dd7543adaf6c54512447 in / 
# Mon, 05 Jun 2023 17:01:04 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:19:12 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:19:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:19:13 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:24:42 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:24:43 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:25:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:25:43 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 07:36:03 GMT
ARG SOLR_VERSION=9.2.1
# Fri, 16 Jun 2023 07:36:04 GMT
ARG SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb
# Fri, 16 Jun 2023 07:36:04 GMT
ARG SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271
# Fri, 16 Jun 2023 07:36:05 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 16 Jun 2023 07:36:05 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 16 Jun 2023 07:36:05 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 07:36:06 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 07:36:06 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 16 Jun 2023 07:37:24 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 16 Jun 2023 07:37:29 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 16 Jun 2023 07:37:29 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 16 Jun 2023 07:37:30 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 16 Jun 2023 07:37:30 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 16 Jun 2023 07:37:31 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 16 Jun 2023 07:37:32 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 16 Jun 2023 07:37:35 GMT
LABEL org.opencontainers.image.version=9.2.1
# Fri, 16 Jun 2023 07:37:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 16 Jun 2023 07:37:37 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 16 Jun 2023 07:37:39 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 16 Jun 2023 07:37:41 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 16 Jun 2023 07:37:43 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 16 Jun 2023 07:38:00 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 16 Jun 2023 07:38:00 GMT
VOLUME [/var/solr]
# Fri, 16 Jun 2023 07:38:01 GMT
EXPOSE 8983
# Fri, 16 Jun 2023 07:38:01 GMT
WORKDIR /opt/solr
# Fri, 16 Jun 2023 07:38:02 GMT
USER 8983
# Fri, 16 Jun 2023 07:38:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 07:38:03 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:a02dd69d9a8a1e6f4fc2ccb509fb8efd6014b00ff932a757d23b4b012a2bec49`  
		Last Modified: Fri, 16 Jun 2023 00:44:52 GMT  
		Size: 35.7 MB (35711397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bd55325dd69030064f13098489df6ef8e45b2d52baffb366675c06f6e94418`  
		Last Modified: Fri, 16 Jun 2023 02:30:20 GMT  
		Size: 18.3 MB (18322826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef75c435e36e0d0cb9911afc443c4bf6c1769b56642390039838f6017497b2f`  
		Last Modified: Fri, 16 Jun 2023 02:31:24 GMT  
		Size: 46.9 MB (46872498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edff0610bd2e6e17f260f10d236a0fad32db564c59f810b5e30eaee37ef5faf8`  
		Last Modified: Fri, 16 Jun 2023 02:31:13 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d7ebdacee82ac6455d940b19d21bf659f1cf53c3aaa3f3e1577135b8802d3e`  
		Last Modified: Fri, 16 Jun 2023 07:43:45 GMT  
		Size: 279.0 MB (278994934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64708f76d121ff3c1262875272f841e9c3bb2244f1d305672fed751d7c638df1`  
		Last Modified: Fri, 16 Jun 2023 07:43:24 GMT  
		Size: 4.3 KB (4297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495b3eb13c2abbf80d9c705cdb460f2f939de60c92c610848a2c4defab47dd11`  
		Last Modified: Fri, 16 Jun 2023 07:43:24 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8695e9bc13470e29cd835a938319952511edd7c991fecadf3ed9d64c89a727b`  
		Last Modified: Fri, 16 Jun 2023 07:43:24 GMT  
		Size: 8.3 KB (8273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3227aa649395d114eef9c32c931462d8a75c9fe23aa39081891ddc6dc3c31c74`  
		Last Modified: Fri, 16 Jun 2023 07:43:25 GMT  
		Size: 1.8 MB (1834188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:latest` - linux; s390x

```console
$ docker pull solr@sha256:2e2e1090eeb5e9008c115e614650f992c607ac460b8d848c6bcf4c5fbdfa2f09
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **370.0 MB (370021779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f06f08b94cb5330a7ff42794eee64cc602fd8b2713258fcdb3ca2001d12c0e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 22 May 2023 17:46:45 GMT
ARG RELEASE
# Mon, 22 May 2023 17:46:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 22 May 2023 17:46:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 22 May 2023 17:46:45 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 22 May 2023 17:46:47 GMT
ADD file:7bf1b7a1484e37f289d40f5c1c1cbe321ef337f898dd3d5809193c848a9a3dc2 in / 
# Mon, 22 May 2023 17:46:47 GMT
CMD ["/bin/bash"]
# Thu, 01 Jun 2023 23:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 01 Jun 2023 23:33:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Jun 2023 23:33:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 01 Jun 2023 23:34:41 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 01 Jun 2023 23:34:43 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Thu, 01 Jun 2023 23:35:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 01 Jun 2023 23:35:21 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_VERSION=9.2.1
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 02 Jun 2023 15:52:55 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz
# Fri, 02 Jun 2023 15:53:16 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 02 Jun 2023 15:53:20 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 02 Jun 2023 15:53:20 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.version=9.2.1
# Fri, 02 Jun 2023 15:53:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 02 Jun 2023 15:53:21 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 02 Jun 2023 15:53:21 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 02 Jun 2023 15:53:22 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 02 Jun 2023 15:53:22 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 02 Jun 2023 15:53:27 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.1/solr-9.2.1.tgz SOLR_KEYS=FDB3D11D716BB32ACF8C93AB919B21537AA80271 SOLR_SHA512=1ff1bd22255b0ae5a1ade1d03596c1f35d4fa69fa1a16e823eaa554b30ba1311f031af6e1f95a94dbdd3a1dbf308eeb068e7303b74f83584a8bb443505078cbb SOLR_VERSION=9.2.1
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 02 Jun 2023 15:53:27 GMT
VOLUME [/var/solr]
# Fri, 02 Jun 2023 15:53:27 GMT
EXPOSE 8983
# Fri, 02 Jun 2023 15:53:27 GMT
WORKDIR /opt/solr
# Fri, 02 Jun 2023 15:53:28 GMT
USER 8983
# Fri, 02 Jun 2023 15:53:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Jun 2023 15:53:28 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:f2957179c3a13374d05630725d1d996f8083efadf7d2da999c9b4ca53ab7c98f`  
		Last Modified: Thu, 01 Jun 2023 23:19:06 GMT  
		Size: 28.6 MB (28648005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff49023eb8231a4489c04787627471c943342afea6aed42b66e0bd17f75307a`  
		Last Modified: Thu, 01 Jun 2023 23:36:33 GMT  
		Size: 16.8 MB (16817675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58123ce9cafda91814be25f8b9b9f99431886cfbee190fc6ba7f6be9abdfe781`  
		Last Modified: Thu, 01 Jun 2023 23:36:56 GMT  
		Size: 43.8 MB (43774489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c27d78a58220d69494be2a17dffa9c4de667bdcf0f6e85c869482d832b8af8f`  
		Last Modified: Thu, 01 Jun 2023 23:36:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeab0826386b334263843df3860f46ec4cb1baa7490d55f653630de11aefecb2`  
		Last Modified: Fri, 02 Jun 2023 15:54:19 GMT  
		Size: 279.0 MB (278994275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5f2afb9fbda66fff0a22400f8df154060d0f1d74944a07653c6466fb541622`  
		Last Modified: Fri, 02 Jun 2023 15:54:08 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b24eb5989fbe19cfbfa7fade0c611dd880bd9f279f3960ce96ca5a35e4188ad`  
		Last Modified: Fri, 02 Jun 2023 15:54:08 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fbd279dbd567d795f616c80182d1ea59f0584002dcd56265accfa296ec81551`  
		Last Modified: Fri, 02 Jun 2023 15:54:08 GMT  
		Size: 8.3 KB (8265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf0d1005aca634a3af1af7d7165552463412e8d705e08a29aec622534e2987f`  
		Last Modified: Fri, 02 Jun 2023 15:54:08 GMT  
		Size: 1.8 MB (1774360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
