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
-	[`solr:9.2.0`](#solr920)
-	[`solr:latest`](#solrlatest)

## `solr:8`

```console
$ docker pull solr@sha256:2607eca8ca54a2d91d2f32300a2bc2917150c7f2338b4bae5c149d2c24c800cb
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
$ docker pull solr@sha256:b210a1886da5e6bd04b978e092ad2282fefb2b2ab9e928465b5c6d4cad58497d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.8 MB (314801289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fee171281dcf64fb86a69dad1e9390dee50678fea5dc79f0259935b9760cd04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 00:42:52 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 00:42:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 00:42:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 00:43:22 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 00:43:54 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 00:44:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:20 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 05:38:29 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Tue, 18 Apr 2023 05:38:29 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Tue, 18 Apr 2023 05:38:29 GMT
ARG SOLR_VERSION=8.11.2
# Tue, 18 Apr 2023 05:38:29 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Tue, 18 Apr 2023 05:38:30 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Tue, 18 Apr 2023 05:38:30 GMT
ARG SOLR_DOWNLOAD_URL
# Tue, 18 Apr 2023 05:38:30 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 18 Apr 2023 05:38:37 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Tue, 18 Apr 2023 05:38:37 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Tue, 18 Apr 2023 05:38:37 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 18 Apr 2023 05:38:46 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Tue, 18 Apr 2023 05:39:20 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Tue, 18 Apr 2023 05:39:20 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Tue, 18 Apr 2023 05:39:20 GMT
VOLUME [/var/solr]
# Tue, 18 Apr 2023 05:39:20 GMT
EXPOSE 8983
# Tue, 18 Apr 2023 05:39:20 GMT
WORKDIR /opt/solr
# Tue, 18 Apr 2023 05:39:20 GMT
USER 8983
# Tue, 18 Apr 2023 05:39:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 05:39:21 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7affba4c9a33ed5dd050532c0d53e38b2c35c2fe490db721d943658feee4c914`  
		Last Modified: Tue, 18 Apr 2023 00:46:23 GMT  
		Size: 16.3 MB (16347011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fb5d08d03b0834295af88b5b911dca1240bcbdc3268dbc4c8ce24934ae017e`  
		Last Modified: Tue, 18 Apr 2023 00:47:26 GMT  
		Size: 46.6 MB (46632203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ef4a2443f5b89eae76a92c01bf3a006c986bb4fe658aa46a8dccc0bed2f523`  
		Last Modified: Tue, 18 Apr 2023 00:47:19 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e005372261eff41e611105a513fed9afaef08b30a879c639a8ac0efafd9300`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 4.9 MB (4901010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad0a251b15f3c813079323fdb45751b01c5753143b2c5dc1c6665bcc3e2680c`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 4.3 KB (4291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53da2eb3eae194651c65ebab849877740d6128968fd6e3f78f1a669b1ecb73d`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2462511e3bac8b859994f31534f2cfff6f8bfc787b5dc0909219b61ba839fdd1`  
		Last Modified: Tue, 18 Apr 2023 05:40:25 GMT  
		Size: 218.3 MB (218328276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7090d8a3f08936349556e936cfd4a9bfb2cd6661eeab03630417cee2cad95bfd`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8` - linux; arm variant v7

```console
$ docker pull solr@sha256:6dafcadde2e7a193d0625f280e2682fd53f6d499b74d4af8025e660f6f25a348
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.2 MB (307180449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0dd03a8533275b4869866465fbd3cb5250aa0d685f1cef49c33f55f3e477b90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:52:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:52:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:52:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:52:26 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:58:18 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:58:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:58:58 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:55:48 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 26 Apr 2023 20:55:48 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 26 Apr 2023 20:55:48 GMT
ARG SOLR_VERSION=8.11.2
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:55:55 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 26 Apr 2023 20:55:55 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 26 Apr 2023 20:55:56 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:56:04 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 26 Apr 2023 20:56:41 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 26 Apr 2023 20:56:42 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 26 Apr 2023 20:56:42 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:56:42 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:56:42 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:56:42 GMT
USER 8983
# Wed, 26 Apr 2023 20:56:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:56:42 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:e68c91cb250f35160f683afa80c3ada46f06948ded46a188be490ea3afff08f5`  
		Last Modified: Fri, 14 Apr 2023 09:34:28 GMT  
		Size: 24.6 MB (24586976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26020bb58aaff7bb6175448d285783e1d1698e726bcba90502c721abc88f2a2`  
		Last Modified: Tue, 18 Apr 2023 01:54:29 GMT  
		Size: 15.2 MB (15177669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6beb6c54ed90fe5685ff23c9c1c5c2e8f9cfb87d68e53bccd8a0ba8ea6bb45e`  
		Last Modified: Wed, 26 Apr 2023 20:01:25 GMT  
		Size: 44.9 MB (44878110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2be4736e459b5628fd2b307c8d7943b3f55d8dccdd160ec14322808c4042aa`  
		Last Modified: Wed, 26 Apr 2023 20:01:18 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f5442bfaa9ed3f392420670361ffe3de09563936eafbb08e3d1751bd41fe08`  
		Last Modified: Wed, 26 Apr 2023 20:58:05 GMT  
		Size: 4.2 MB (4195197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092c315c9b467de64195ac22278518557f4a1786ce8531d558c69b7baa3795c1`  
		Last Modified: Wed, 26 Apr 2023 20:58:04 GMT  
		Size: 4.2 KB (4229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc80305416e522db899c313b1d14efc8a78c84b41c6f7e823d6d065651db97df`  
		Last Modified: Wed, 26 Apr 2023 20:58:04 GMT  
		Size: 3.5 KB (3465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b3deffe546af271360886735be91826cf5dadf35b44ec9886d3c0fd0b41681`  
		Last Modified: Wed, 26 Apr 2023 20:58:16 GMT  
		Size: 218.3 MB (218328333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27437b66908cc998c75f64e651aa564eadd0eb13069222b57e72d0553f0f7362`  
		Last Modified: Wed, 26 Apr 2023 20:58:04 GMT  
		Size: 6.3 KB (6310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:9c83437dd68f23bd3272fa16658b6bb0a96b4c47b0e19257d018071f1cbfe495
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.5 MB (311481859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee0bcfc19e6f7e821e073ab8496a566a25ab40161cd530e90512c5f46ed1bf67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:40:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:40:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:40:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:41:09 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:41:31 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 01:41:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 01:41:55 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 03:21:22 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Tue, 18 Apr 2023 03:21:23 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_VERSION=8.11.2
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_DOWNLOAD_URL
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 18 Apr 2023 03:21:28 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Tue, 18 Apr 2023 03:21:29 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Tue, 18 Apr 2023 03:21:29 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 18 Apr 2023 03:21:43 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Tue, 18 Apr 2023 03:22:14 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Tue, 18 Apr 2023 03:22:16 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Tue, 18 Apr 2023 03:22:16 GMT
VOLUME [/var/solr]
# Tue, 18 Apr 2023 03:22:16 GMT
EXPOSE 8983
# Tue, 18 Apr 2023 03:22:16 GMT
WORKDIR /opt/solr
# Tue, 18 Apr 2023 03:22:16 GMT
USER 8983
# Tue, 18 Apr 2023 03:22:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 03:22:16 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269336393c4662b72ac4a2be29473801366e79f4db6c8b9944509f1903ee3fe6`  
		Last Modified: Tue, 18 Apr 2023 01:43:30 GMT  
		Size: 16.2 MB (16213349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5775e69497bdf42d2ad7b39be6112c42f7fb711efa0036c55e9a5ddf8b30c244`  
		Last Modified: Tue, 18 Apr 2023 01:44:26 GMT  
		Size: 45.0 MB (44979459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff94c7a5594b10847f2895eb9f20938960ec3194f7398f5da8e801aff22ab00`  
		Last Modified: Tue, 18 Apr 2023 01:44:21 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3419bf7e5540a3bcd6132aa79f49429981574fb43627e2e617efd771123733e`  
		Last Modified: Tue, 18 Apr 2023 03:23:06 GMT  
		Size: 4.8 MB (4750130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f986cb8a544e5f5ed858bfd84e22a07cc5d8d5133bf126062e34097fb071cea9`  
		Last Modified: Tue, 18 Apr 2023 03:23:05 GMT  
		Size: 4.3 KB (4335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46abce6c72ed3766b9f8dfbfadcecd21ca0597eef161bd3ef3b10408b72ae346`  
		Last Modified: Tue, 18 Apr 2023 03:23:05 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbfb9f1a96f5d4bb8867ba070a31604ef992f2fe5672efd1775b3f3335be352`  
		Last Modified: Tue, 18 Apr 2023 03:23:15 GMT  
		Size: 218.3 MB (218328255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6099366efb07d013239cc98b209d1b555226441829877031336b84cc7f2f083`  
		Last Modified: Tue, 18 Apr 2023 03:23:05 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8` - linux; ppc64le

```console
$ docker pull solr@sha256:89193853b9976c1e9bf28386f66c7fc5fca07d300011b106e1336e61c60a1642
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.1 MB (317097124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e4efdfa11f4e85646d5c547f7ba3db1ceb897451de41508ad75533c2f5786f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:06:30 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:06:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:06:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:07:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:19:05 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:21:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:21:50 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:41:58 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 26 Apr 2023 20:41:58 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 26 Apr 2023 20:41:58 GMT
ARG SOLR_VERSION=8.11.2
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:42:14 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 26 Apr 2023 20:42:14 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 26 Apr 2023 20:42:16 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:42:37 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 26 Apr 2023 20:43:05 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 26 Apr 2023 20:43:08 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 26 Apr 2023 20:43:08 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:43:09 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:43:09 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:43:09 GMT
USER 8983
# Wed, 26 Apr 2023 20:43:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:43:10 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:d276072145993a42aed3e2b3e8cd26b6e08aab266d9c9d792ee89b26150681da`  
		Last Modified: Fri, 14 Apr 2023 09:36:00 GMT  
		Size: 33.3 MB (33300980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4018ee3c8b327c120bbf0427fb12e76c74cb054a92177aeeae16bcf0efa4e86`  
		Last Modified: Tue, 18 Apr 2023 01:11:24 GMT  
		Size: 17.6 MB (17582531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68132c1824ed616e2aa64a0252f82705524204a2dcc79d1bbf7f8a481f482bc0`  
		Last Modified: Wed, 26 Apr 2023 19:32:54 GMT  
		Size: 42.1 MB (42093906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705220513c41d99a8d5e529e29488b3b903dad838d853121dc9cbf9dcb950209`  
		Last Modified: Wed, 26 Apr 2023 19:32:43 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a018bd1c2d0feb9fe5b7c849d3b3d1bc427f062719f198d72eaf9eb16e1305b`  
		Last Modified: Wed, 26 Apr 2023 20:45:12 GMT  
		Size: 5.8 MB (5777193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65368a709ae0c7650e4198a55b2881827eb073d63097628050704e0542e86e3`  
		Last Modified: Wed, 26 Apr 2023 20:45:11 GMT  
		Size: 4.3 KB (4299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b057f087dfda706087959b2cbe2f9badb9984f26149834861a9e8bbfcfc6bb40`  
		Last Modified: Wed, 26 Apr 2023 20:45:11 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e36d02c2b4075d6f7050b9befb0e3b722f04cd0d99de9c8f7485a2dbf232f2`  
		Last Modified: Wed, 26 Apr 2023 20:45:29 GMT  
		Size: 218.3 MB (218328281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed30ffc679a350213ccaeb74148aef8cfec6c885c4264b98898b15fc32956f2`  
		Last Modified: Wed, 26 Apr 2023 20:45:11 GMT  
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
$ docker pull solr@sha256:2607eca8ca54a2d91d2f32300a2bc2917150c7f2338b4bae5c149d2c24c800cb
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
$ docker pull solr@sha256:b210a1886da5e6bd04b978e092ad2282fefb2b2ab9e928465b5c6d4cad58497d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.8 MB (314801289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fee171281dcf64fb86a69dad1e9390dee50678fea5dc79f0259935b9760cd04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 00:42:52 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 00:42:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 00:42:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 00:43:22 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 00:43:54 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 00:44:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:20 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 05:38:29 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Tue, 18 Apr 2023 05:38:29 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Tue, 18 Apr 2023 05:38:29 GMT
ARG SOLR_VERSION=8.11.2
# Tue, 18 Apr 2023 05:38:29 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Tue, 18 Apr 2023 05:38:30 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Tue, 18 Apr 2023 05:38:30 GMT
ARG SOLR_DOWNLOAD_URL
# Tue, 18 Apr 2023 05:38:30 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 18 Apr 2023 05:38:37 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Tue, 18 Apr 2023 05:38:37 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Tue, 18 Apr 2023 05:38:37 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 18 Apr 2023 05:38:46 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Tue, 18 Apr 2023 05:39:20 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Tue, 18 Apr 2023 05:39:20 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Tue, 18 Apr 2023 05:39:20 GMT
VOLUME [/var/solr]
# Tue, 18 Apr 2023 05:39:20 GMT
EXPOSE 8983
# Tue, 18 Apr 2023 05:39:20 GMT
WORKDIR /opt/solr
# Tue, 18 Apr 2023 05:39:20 GMT
USER 8983
# Tue, 18 Apr 2023 05:39:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 05:39:21 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7affba4c9a33ed5dd050532c0d53e38b2c35c2fe490db721d943658feee4c914`  
		Last Modified: Tue, 18 Apr 2023 00:46:23 GMT  
		Size: 16.3 MB (16347011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fb5d08d03b0834295af88b5b911dca1240bcbdc3268dbc4c8ce24934ae017e`  
		Last Modified: Tue, 18 Apr 2023 00:47:26 GMT  
		Size: 46.6 MB (46632203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ef4a2443f5b89eae76a92c01bf3a006c986bb4fe658aa46a8dccc0bed2f523`  
		Last Modified: Tue, 18 Apr 2023 00:47:19 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e005372261eff41e611105a513fed9afaef08b30a879c639a8ac0efafd9300`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 4.9 MB (4901010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad0a251b15f3c813079323fdb45751b01c5753143b2c5dc1c6665bcc3e2680c`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 4.3 KB (4291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53da2eb3eae194651c65ebab849877740d6128968fd6e3f78f1a669b1ecb73d`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2462511e3bac8b859994f31534f2cfff6f8bfc787b5dc0909219b61ba839fdd1`  
		Last Modified: Tue, 18 Apr 2023 05:40:25 GMT  
		Size: 218.3 MB (218328276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7090d8a3f08936349556e936cfd4a9bfb2cd6661eeab03630417cee2cad95bfd`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8-slim` - linux; arm variant v7

```console
$ docker pull solr@sha256:6dafcadde2e7a193d0625f280e2682fd53f6d499b74d4af8025e660f6f25a348
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.2 MB (307180449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0dd03a8533275b4869866465fbd3cb5250aa0d685f1cef49c33f55f3e477b90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:52:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:52:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:52:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:52:26 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:58:18 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:58:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:58:58 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:55:48 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 26 Apr 2023 20:55:48 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 26 Apr 2023 20:55:48 GMT
ARG SOLR_VERSION=8.11.2
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:55:55 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 26 Apr 2023 20:55:55 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 26 Apr 2023 20:55:56 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:56:04 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 26 Apr 2023 20:56:41 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 26 Apr 2023 20:56:42 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 26 Apr 2023 20:56:42 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:56:42 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:56:42 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:56:42 GMT
USER 8983
# Wed, 26 Apr 2023 20:56:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:56:42 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:e68c91cb250f35160f683afa80c3ada46f06948ded46a188be490ea3afff08f5`  
		Last Modified: Fri, 14 Apr 2023 09:34:28 GMT  
		Size: 24.6 MB (24586976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26020bb58aaff7bb6175448d285783e1d1698e726bcba90502c721abc88f2a2`  
		Last Modified: Tue, 18 Apr 2023 01:54:29 GMT  
		Size: 15.2 MB (15177669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6beb6c54ed90fe5685ff23c9c1c5c2e8f9cfb87d68e53bccd8a0ba8ea6bb45e`  
		Last Modified: Wed, 26 Apr 2023 20:01:25 GMT  
		Size: 44.9 MB (44878110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2be4736e459b5628fd2b307c8d7943b3f55d8dccdd160ec14322808c4042aa`  
		Last Modified: Wed, 26 Apr 2023 20:01:18 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f5442bfaa9ed3f392420670361ffe3de09563936eafbb08e3d1751bd41fe08`  
		Last Modified: Wed, 26 Apr 2023 20:58:05 GMT  
		Size: 4.2 MB (4195197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092c315c9b467de64195ac22278518557f4a1786ce8531d558c69b7baa3795c1`  
		Last Modified: Wed, 26 Apr 2023 20:58:04 GMT  
		Size: 4.2 KB (4229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc80305416e522db899c313b1d14efc8a78c84b41c6f7e823d6d065651db97df`  
		Last Modified: Wed, 26 Apr 2023 20:58:04 GMT  
		Size: 3.5 KB (3465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b3deffe546af271360886735be91826cf5dadf35b44ec9886d3c0fd0b41681`  
		Last Modified: Wed, 26 Apr 2023 20:58:16 GMT  
		Size: 218.3 MB (218328333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27437b66908cc998c75f64e651aa564eadd0eb13069222b57e72d0553f0f7362`  
		Last Modified: Wed, 26 Apr 2023 20:58:04 GMT  
		Size: 6.3 KB (6310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8-slim` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:9c83437dd68f23bd3272fa16658b6bb0a96b4c47b0e19257d018071f1cbfe495
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.5 MB (311481859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee0bcfc19e6f7e821e073ab8496a566a25ab40161cd530e90512c5f46ed1bf67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:40:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:40:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:40:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:41:09 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:41:31 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 01:41:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 01:41:55 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 03:21:22 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Tue, 18 Apr 2023 03:21:23 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_VERSION=8.11.2
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_DOWNLOAD_URL
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 18 Apr 2023 03:21:28 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Tue, 18 Apr 2023 03:21:29 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Tue, 18 Apr 2023 03:21:29 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 18 Apr 2023 03:21:43 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Tue, 18 Apr 2023 03:22:14 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Tue, 18 Apr 2023 03:22:16 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Tue, 18 Apr 2023 03:22:16 GMT
VOLUME [/var/solr]
# Tue, 18 Apr 2023 03:22:16 GMT
EXPOSE 8983
# Tue, 18 Apr 2023 03:22:16 GMT
WORKDIR /opt/solr
# Tue, 18 Apr 2023 03:22:16 GMT
USER 8983
# Tue, 18 Apr 2023 03:22:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 03:22:16 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269336393c4662b72ac4a2be29473801366e79f4db6c8b9944509f1903ee3fe6`  
		Last Modified: Tue, 18 Apr 2023 01:43:30 GMT  
		Size: 16.2 MB (16213349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5775e69497bdf42d2ad7b39be6112c42f7fb711efa0036c55e9a5ddf8b30c244`  
		Last Modified: Tue, 18 Apr 2023 01:44:26 GMT  
		Size: 45.0 MB (44979459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff94c7a5594b10847f2895eb9f20938960ec3194f7398f5da8e801aff22ab00`  
		Last Modified: Tue, 18 Apr 2023 01:44:21 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3419bf7e5540a3bcd6132aa79f49429981574fb43627e2e617efd771123733e`  
		Last Modified: Tue, 18 Apr 2023 03:23:06 GMT  
		Size: 4.8 MB (4750130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f986cb8a544e5f5ed858bfd84e22a07cc5d8d5133bf126062e34097fb071cea9`  
		Last Modified: Tue, 18 Apr 2023 03:23:05 GMT  
		Size: 4.3 KB (4335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46abce6c72ed3766b9f8dfbfadcecd21ca0597eef161bd3ef3b10408b72ae346`  
		Last Modified: Tue, 18 Apr 2023 03:23:05 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbfb9f1a96f5d4bb8867ba070a31604ef992f2fe5672efd1775b3f3335be352`  
		Last Modified: Tue, 18 Apr 2023 03:23:15 GMT  
		Size: 218.3 MB (218328255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6099366efb07d013239cc98b209d1b555226441829877031336b84cc7f2f083`  
		Last Modified: Tue, 18 Apr 2023 03:23:05 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8-slim` - linux; ppc64le

```console
$ docker pull solr@sha256:89193853b9976c1e9bf28386f66c7fc5fca07d300011b106e1336e61c60a1642
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.1 MB (317097124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e4efdfa11f4e85646d5c547f7ba3db1ceb897451de41508ad75533c2f5786f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:06:30 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:06:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:06:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:07:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:19:05 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:21:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:21:50 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:41:58 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 26 Apr 2023 20:41:58 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 26 Apr 2023 20:41:58 GMT
ARG SOLR_VERSION=8.11.2
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:42:14 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 26 Apr 2023 20:42:14 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 26 Apr 2023 20:42:16 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:42:37 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 26 Apr 2023 20:43:05 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 26 Apr 2023 20:43:08 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 26 Apr 2023 20:43:08 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:43:09 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:43:09 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:43:09 GMT
USER 8983
# Wed, 26 Apr 2023 20:43:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:43:10 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:d276072145993a42aed3e2b3e8cd26b6e08aab266d9c9d792ee89b26150681da`  
		Last Modified: Fri, 14 Apr 2023 09:36:00 GMT  
		Size: 33.3 MB (33300980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4018ee3c8b327c120bbf0427fb12e76c74cb054a92177aeeae16bcf0efa4e86`  
		Last Modified: Tue, 18 Apr 2023 01:11:24 GMT  
		Size: 17.6 MB (17582531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68132c1824ed616e2aa64a0252f82705524204a2dcc79d1bbf7f8a481f482bc0`  
		Last Modified: Wed, 26 Apr 2023 19:32:54 GMT  
		Size: 42.1 MB (42093906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705220513c41d99a8d5e529e29488b3b903dad838d853121dc9cbf9dcb950209`  
		Last Modified: Wed, 26 Apr 2023 19:32:43 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a018bd1c2d0feb9fe5b7c849d3b3d1bc427f062719f198d72eaf9eb16e1305b`  
		Last Modified: Wed, 26 Apr 2023 20:45:12 GMT  
		Size: 5.8 MB (5777193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65368a709ae0c7650e4198a55b2881827eb073d63097628050704e0542e86e3`  
		Last Modified: Wed, 26 Apr 2023 20:45:11 GMT  
		Size: 4.3 KB (4299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b057f087dfda706087959b2cbe2f9badb9984f26149834861a9e8bbfcfc6bb40`  
		Last Modified: Wed, 26 Apr 2023 20:45:11 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e36d02c2b4075d6f7050b9befb0e3b722f04cd0d99de9c8f7485a2dbf232f2`  
		Last Modified: Wed, 26 Apr 2023 20:45:29 GMT  
		Size: 218.3 MB (218328281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed30ffc679a350213ccaeb74148aef8cfec6c885c4264b98898b15fc32956f2`  
		Last Modified: Wed, 26 Apr 2023 20:45:11 GMT  
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
$ docker pull solr@sha256:2607eca8ca54a2d91d2f32300a2bc2917150c7f2338b4bae5c149d2c24c800cb
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
$ docker pull solr@sha256:b210a1886da5e6bd04b978e092ad2282fefb2b2ab9e928465b5c6d4cad58497d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.8 MB (314801289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fee171281dcf64fb86a69dad1e9390dee50678fea5dc79f0259935b9760cd04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 00:42:52 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 00:42:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 00:42:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 00:43:22 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 00:43:54 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 00:44:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:20 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 05:38:29 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Tue, 18 Apr 2023 05:38:29 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Tue, 18 Apr 2023 05:38:29 GMT
ARG SOLR_VERSION=8.11.2
# Tue, 18 Apr 2023 05:38:29 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Tue, 18 Apr 2023 05:38:30 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Tue, 18 Apr 2023 05:38:30 GMT
ARG SOLR_DOWNLOAD_URL
# Tue, 18 Apr 2023 05:38:30 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 18 Apr 2023 05:38:37 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Tue, 18 Apr 2023 05:38:37 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Tue, 18 Apr 2023 05:38:37 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 18 Apr 2023 05:38:46 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Tue, 18 Apr 2023 05:39:20 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Tue, 18 Apr 2023 05:39:20 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Tue, 18 Apr 2023 05:39:20 GMT
VOLUME [/var/solr]
# Tue, 18 Apr 2023 05:39:20 GMT
EXPOSE 8983
# Tue, 18 Apr 2023 05:39:20 GMT
WORKDIR /opt/solr
# Tue, 18 Apr 2023 05:39:20 GMT
USER 8983
# Tue, 18 Apr 2023 05:39:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 05:39:21 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7affba4c9a33ed5dd050532c0d53e38b2c35c2fe490db721d943658feee4c914`  
		Last Modified: Tue, 18 Apr 2023 00:46:23 GMT  
		Size: 16.3 MB (16347011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fb5d08d03b0834295af88b5b911dca1240bcbdc3268dbc4c8ce24934ae017e`  
		Last Modified: Tue, 18 Apr 2023 00:47:26 GMT  
		Size: 46.6 MB (46632203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ef4a2443f5b89eae76a92c01bf3a006c986bb4fe658aa46a8dccc0bed2f523`  
		Last Modified: Tue, 18 Apr 2023 00:47:19 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e005372261eff41e611105a513fed9afaef08b30a879c639a8ac0efafd9300`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 4.9 MB (4901010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad0a251b15f3c813079323fdb45751b01c5753143b2c5dc1c6665bcc3e2680c`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 4.3 KB (4291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53da2eb3eae194651c65ebab849877740d6128968fd6e3f78f1a669b1ecb73d`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2462511e3bac8b859994f31534f2cfff6f8bfc787b5dc0909219b61ba839fdd1`  
		Last Modified: Tue, 18 Apr 2023 05:40:25 GMT  
		Size: 218.3 MB (218328276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7090d8a3f08936349556e936cfd4a9bfb2cd6661eeab03630417cee2cad95bfd`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11` - linux; arm variant v7

```console
$ docker pull solr@sha256:6dafcadde2e7a193d0625f280e2682fd53f6d499b74d4af8025e660f6f25a348
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.2 MB (307180449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0dd03a8533275b4869866465fbd3cb5250aa0d685f1cef49c33f55f3e477b90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:52:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:52:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:52:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:52:26 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:58:18 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:58:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:58:58 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:55:48 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 26 Apr 2023 20:55:48 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 26 Apr 2023 20:55:48 GMT
ARG SOLR_VERSION=8.11.2
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:55:55 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 26 Apr 2023 20:55:55 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 26 Apr 2023 20:55:56 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:56:04 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 26 Apr 2023 20:56:41 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 26 Apr 2023 20:56:42 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 26 Apr 2023 20:56:42 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:56:42 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:56:42 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:56:42 GMT
USER 8983
# Wed, 26 Apr 2023 20:56:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:56:42 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:e68c91cb250f35160f683afa80c3ada46f06948ded46a188be490ea3afff08f5`  
		Last Modified: Fri, 14 Apr 2023 09:34:28 GMT  
		Size: 24.6 MB (24586976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26020bb58aaff7bb6175448d285783e1d1698e726bcba90502c721abc88f2a2`  
		Last Modified: Tue, 18 Apr 2023 01:54:29 GMT  
		Size: 15.2 MB (15177669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6beb6c54ed90fe5685ff23c9c1c5c2e8f9cfb87d68e53bccd8a0ba8ea6bb45e`  
		Last Modified: Wed, 26 Apr 2023 20:01:25 GMT  
		Size: 44.9 MB (44878110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2be4736e459b5628fd2b307c8d7943b3f55d8dccdd160ec14322808c4042aa`  
		Last Modified: Wed, 26 Apr 2023 20:01:18 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f5442bfaa9ed3f392420670361ffe3de09563936eafbb08e3d1751bd41fe08`  
		Last Modified: Wed, 26 Apr 2023 20:58:05 GMT  
		Size: 4.2 MB (4195197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092c315c9b467de64195ac22278518557f4a1786ce8531d558c69b7baa3795c1`  
		Last Modified: Wed, 26 Apr 2023 20:58:04 GMT  
		Size: 4.2 KB (4229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc80305416e522db899c313b1d14efc8a78c84b41c6f7e823d6d065651db97df`  
		Last Modified: Wed, 26 Apr 2023 20:58:04 GMT  
		Size: 3.5 KB (3465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b3deffe546af271360886735be91826cf5dadf35b44ec9886d3c0fd0b41681`  
		Last Modified: Wed, 26 Apr 2023 20:58:16 GMT  
		Size: 218.3 MB (218328333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27437b66908cc998c75f64e651aa564eadd0eb13069222b57e72d0553f0f7362`  
		Last Modified: Wed, 26 Apr 2023 20:58:04 GMT  
		Size: 6.3 KB (6310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:9c83437dd68f23bd3272fa16658b6bb0a96b4c47b0e19257d018071f1cbfe495
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.5 MB (311481859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee0bcfc19e6f7e821e073ab8496a566a25ab40161cd530e90512c5f46ed1bf67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:40:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:40:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:40:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:41:09 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:41:31 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 01:41:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 01:41:55 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 03:21:22 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Tue, 18 Apr 2023 03:21:23 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_VERSION=8.11.2
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_DOWNLOAD_URL
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 18 Apr 2023 03:21:28 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Tue, 18 Apr 2023 03:21:29 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Tue, 18 Apr 2023 03:21:29 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 18 Apr 2023 03:21:43 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Tue, 18 Apr 2023 03:22:14 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Tue, 18 Apr 2023 03:22:16 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Tue, 18 Apr 2023 03:22:16 GMT
VOLUME [/var/solr]
# Tue, 18 Apr 2023 03:22:16 GMT
EXPOSE 8983
# Tue, 18 Apr 2023 03:22:16 GMT
WORKDIR /opt/solr
# Tue, 18 Apr 2023 03:22:16 GMT
USER 8983
# Tue, 18 Apr 2023 03:22:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 03:22:16 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269336393c4662b72ac4a2be29473801366e79f4db6c8b9944509f1903ee3fe6`  
		Last Modified: Tue, 18 Apr 2023 01:43:30 GMT  
		Size: 16.2 MB (16213349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5775e69497bdf42d2ad7b39be6112c42f7fb711efa0036c55e9a5ddf8b30c244`  
		Last Modified: Tue, 18 Apr 2023 01:44:26 GMT  
		Size: 45.0 MB (44979459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff94c7a5594b10847f2895eb9f20938960ec3194f7398f5da8e801aff22ab00`  
		Last Modified: Tue, 18 Apr 2023 01:44:21 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3419bf7e5540a3bcd6132aa79f49429981574fb43627e2e617efd771123733e`  
		Last Modified: Tue, 18 Apr 2023 03:23:06 GMT  
		Size: 4.8 MB (4750130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f986cb8a544e5f5ed858bfd84e22a07cc5d8d5133bf126062e34097fb071cea9`  
		Last Modified: Tue, 18 Apr 2023 03:23:05 GMT  
		Size: 4.3 KB (4335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46abce6c72ed3766b9f8dfbfadcecd21ca0597eef161bd3ef3b10408b72ae346`  
		Last Modified: Tue, 18 Apr 2023 03:23:05 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbfb9f1a96f5d4bb8867ba070a31604ef992f2fe5672efd1775b3f3335be352`  
		Last Modified: Tue, 18 Apr 2023 03:23:15 GMT  
		Size: 218.3 MB (218328255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6099366efb07d013239cc98b209d1b555226441829877031336b84cc7f2f083`  
		Last Modified: Tue, 18 Apr 2023 03:23:05 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11` - linux; ppc64le

```console
$ docker pull solr@sha256:89193853b9976c1e9bf28386f66c7fc5fca07d300011b106e1336e61c60a1642
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.1 MB (317097124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e4efdfa11f4e85646d5c547f7ba3db1ceb897451de41508ad75533c2f5786f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:06:30 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:06:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:06:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:07:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:19:05 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:21:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:21:50 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:41:58 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 26 Apr 2023 20:41:58 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 26 Apr 2023 20:41:58 GMT
ARG SOLR_VERSION=8.11.2
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:42:14 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 26 Apr 2023 20:42:14 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 26 Apr 2023 20:42:16 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:42:37 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 26 Apr 2023 20:43:05 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 26 Apr 2023 20:43:08 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 26 Apr 2023 20:43:08 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:43:09 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:43:09 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:43:09 GMT
USER 8983
# Wed, 26 Apr 2023 20:43:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:43:10 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:d276072145993a42aed3e2b3e8cd26b6e08aab266d9c9d792ee89b26150681da`  
		Last Modified: Fri, 14 Apr 2023 09:36:00 GMT  
		Size: 33.3 MB (33300980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4018ee3c8b327c120bbf0427fb12e76c74cb054a92177aeeae16bcf0efa4e86`  
		Last Modified: Tue, 18 Apr 2023 01:11:24 GMT  
		Size: 17.6 MB (17582531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68132c1824ed616e2aa64a0252f82705524204a2dcc79d1bbf7f8a481f482bc0`  
		Last Modified: Wed, 26 Apr 2023 19:32:54 GMT  
		Size: 42.1 MB (42093906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705220513c41d99a8d5e529e29488b3b903dad838d853121dc9cbf9dcb950209`  
		Last Modified: Wed, 26 Apr 2023 19:32:43 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a018bd1c2d0feb9fe5b7c849d3b3d1bc427f062719f198d72eaf9eb16e1305b`  
		Last Modified: Wed, 26 Apr 2023 20:45:12 GMT  
		Size: 5.8 MB (5777193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65368a709ae0c7650e4198a55b2881827eb073d63097628050704e0542e86e3`  
		Last Modified: Wed, 26 Apr 2023 20:45:11 GMT  
		Size: 4.3 KB (4299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b057f087dfda706087959b2cbe2f9badb9984f26149834861a9e8bbfcfc6bb40`  
		Last Modified: Wed, 26 Apr 2023 20:45:11 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e36d02c2b4075d6f7050b9befb0e3b722f04cd0d99de9c8f7485a2dbf232f2`  
		Last Modified: Wed, 26 Apr 2023 20:45:29 GMT  
		Size: 218.3 MB (218328281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed30ffc679a350213ccaeb74148aef8cfec6c885c4264b98898b15fc32956f2`  
		Last Modified: Wed, 26 Apr 2023 20:45:11 GMT  
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
$ docker pull solr@sha256:2607eca8ca54a2d91d2f32300a2bc2917150c7f2338b4bae5c149d2c24c800cb
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
$ docker pull solr@sha256:b210a1886da5e6bd04b978e092ad2282fefb2b2ab9e928465b5c6d4cad58497d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.8 MB (314801289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fee171281dcf64fb86a69dad1e9390dee50678fea5dc79f0259935b9760cd04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 00:42:52 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 00:42:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 00:42:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 00:43:22 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 00:43:54 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 00:44:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:20 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 05:38:29 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Tue, 18 Apr 2023 05:38:29 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Tue, 18 Apr 2023 05:38:29 GMT
ARG SOLR_VERSION=8.11.2
# Tue, 18 Apr 2023 05:38:29 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Tue, 18 Apr 2023 05:38:30 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Tue, 18 Apr 2023 05:38:30 GMT
ARG SOLR_DOWNLOAD_URL
# Tue, 18 Apr 2023 05:38:30 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 18 Apr 2023 05:38:37 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Tue, 18 Apr 2023 05:38:37 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Tue, 18 Apr 2023 05:38:37 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 18 Apr 2023 05:38:46 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Tue, 18 Apr 2023 05:39:20 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Tue, 18 Apr 2023 05:39:20 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Tue, 18 Apr 2023 05:39:20 GMT
VOLUME [/var/solr]
# Tue, 18 Apr 2023 05:39:20 GMT
EXPOSE 8983
# Tue, 18 Apr 2023 05:39:20 GMT
WORKDIR /opt/solr
# Tue, 18 Apr 2023 05:39:20 GMT
USER 8983
# Tue, 18 Apr 2023 05:39:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 05:39:21 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7affba4c9a33ed5dd050532c0d53e38b2c35c2fe490db721d943658feee4c914`  
		Last Modified: Tue, 18 Apr 2023 00:46:23 GMT  
		Size: 16.3 MB (16347011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fb5d08d03b0834295af88b5b911dca1240bcbdc3268dbc4c8ce24934ae017e`  
		Last Modified: Tue, 18 Apr 2023 00:47:26 GMT  
		Size: 46.6 MB (46632203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ef4a2443f5b89eae76a92c01bf3a006c986bb4fe658aa46a8dccc0bed2f523`  
		Last Modified: Tue, 18 Apr 2023 00:47:19 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e005372261eff41e611105a513fed9afaef08b30a879c639a8ac0efafd9300`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 4.9 MB (4901010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad0a251b15f3c813079323fdb45751b01c5753143b2c5dc1c6665bcc3e2680c`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 4.3 KB (4291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53da2eb3eae194651c65ebab849877740d6128968fd6e3f78f1a669b1ecb73d`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2462511e3bac8b859994f31534f2cfff6f8bfc787b5dc0909219b61ba839fdd1`  
		Last Modified: Tue, 18 Apr 2023 05:40:25 GMT  
		Size: 218.3 MB (218328276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7090d8a3f08936349556e936cfd4a9bfb2cd6661eeab03630417cee2cad95bfd`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11-slim` - linux; arm variant v7

```console
$ docker pull solr@sha256:6dafcadde2e7a193d0625f280e2682fd53f6d499b74d4af8025e660f6f25a348
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.2 MB (307180449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0dd03a8533275b4869866465fbd3cb5250aa0d685f1cef49c33f55f3e477b90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:52:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:52:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:52:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:52:26 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:58:18 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:58:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:58:58 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:55:48 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 26 Apr 2023 20:55:48 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 26 Apr 2023 20:55:48 GMT
ARG SOLR_VERSION=8.11.2
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:55:55 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 26 Apr 2023 20:55:55 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 26 Apr 2023 20:55:56 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:56:04 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 26 Apr 2023 20:56:41 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 26 Apr 2023 20:56:42 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 26 Apr 2023 20:56:42 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:56:42 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:56:42 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:56:42 GMT
USER 8983
# Wed, 26 Apr 2023 20:56:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:56:42 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:e68c91cb250f35160f683afa80c3ada46f06948ded46a188be490ea3afff08f5`  
		Last Modified: Fri, 14 Apr 2023 09:34:28 GMT  
		Size: 24.6 MB (24586976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26020bb58aaff7bb6175448d285783e1d1698e726bcba90502c721abc88f2a2`  
		Last Modified: Tue, 18 Apr 2023 01:54:29 GMT  
		Size: 15.2 MB (15177669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6beb6c54ed90fe5685ff23c9c1c5c2e8f9cfb87d68e53bccd8a0ba8ea6bb45e`  
		Last Modified: Wed, 26 Apr 2023 20:01:25 GMT  
		Size: 44.9 MB (44878110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2be4736e459b5628fd2b307c8d7943b3f55d8dccdd160ec14322808c4042aa`  
		Last Modified: Wed, 26 Apr 2023 20:01:18 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f5442bfaa9ed3f392420670361ffe3de09563936eafbb08e3d1751bd41fe08`  
		Last Modified: Wed, 26 Apr 2023 20:58:05 GMT  
		Size: 4.2 MB (4195197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092c315c9b467de64195ac22278518557f4a1786ce8531d558c69b7baa3795c1`  
		Last Modified: Wed, 26 Apr 2023 20:58:04 GMT  
		Size: 4.2 KB (4229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc80305416e522db899c313b1d14efc8a78c84b41c6f7e823d6d065651db97df`  
		Last Modified: Wed, 26 Apr 2023 20:58:04 GMT  
		Size: 3.5 KB (3465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b3deffe546af271360886735be91826cf5dadf35b44ec9886d3c0fd0b41681`  
		Last Modified: Wed, 26 Apr 2023 20:58:16 GMT  
		Size: 218.3 MB (218328333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27437b66908cc998c75f64e651aa564eadd0eb13069222b57e72d0553f0f7362`  
		Last Modified: Wed, 26 Apr 2023 20:58:04 GMT  
		Size: 6.3 KB (6310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11-slim` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:9c83437dd68f23bd3272fa16658b6bb0a96b4c47b0e19257d018071f1cbfe495
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.5 MB (311481859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee0bcfc19e6f7e821e073ab8496a566a25ab40161cd530e90512c5f46ed1bf67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:40:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:40:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:40:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:41:09 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:41:31 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 01:41:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 01:41:55 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 03:21:22 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Tue, 18 Apr 2023 03:21:23 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_VERSION=8.11.2
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_DOWNLOAD_URL
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 18 Apr 2023 03:21:28 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Tue, 18 Apr 2023 03:21:29 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Tue, 18 Apr 2023 03:21:29 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 18 Apr 2023 03:21:43 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Tue, 18 Apr 2023 03:22:14 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Tue, 18 Apr 2023 03:22:16 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Tue, 18 Apr 2023 03:22:16 GMT
VOLUME [/var/solr]
# Tue, 18 Apr 2023 03:22:16 GMT
EXPOSE 8983
# Tue, 18 Apr 2023 03:22:16 GMT
WORKDIR /opt/solr
# Tue, 18 Apr 2023 03:22:16 GMT
USER 8983
# Tue, 18 Apr 2023 03:22:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 03:22:16 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269336393c4662b72ac4a2be29473801366e79f4db6c8b9944509f1903ee3fe6`  
		Last Modified: Tue, 18 Apr 2023 01:43:30 GMT  
		Size: 16.2 MB (16213349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5775e69497bdf42d2ad7b39be6112c42f7fb711efa0036c55e9a5ddf8b30c244`  
		Last Modified: Tue, 18 Apr 2023 01:44:26 GMT  
		Size: 45.0 MB (44979459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff94c7a5594b10847f2895eb9f20938960ec3194f7398f5da8e801aff22ab00`  
		Last Modified: Tue, 18 Apr 2023 01:44:21 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3419bf7e5540a3bcd6132aa79f49429981574fb43627e2e617efd771123733e`  
		Last Modified: Tue, 18 Apr 2023 03:23:06 GMT  
		Size: 4.8 MB (4750130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f986cb8a544e5f5ed858bfd84e22a07cc5d8d5133bf126062e34097fb071cea9`  
		Last Modified: Tue, 18 Apr 2023 03:23:05 GMT  
		Size: 4.3 KB (4335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46abce6c72ed3766b9f8dfbfadcecd21ca0597eef161bd3ef3b10408b72ae346`  
		Last Modified: Tue, 18 Apr 2023 03:23:05 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbfb9f1a96f5d4bb8867ba070a31604ef992f2fe5672efd1775b3f3335be352`  
		Last Modified: Tue, 18 Apr 2023 03:23:15 GMT  
		Size: 218.3 MB (218328255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6099366efb07d013239cc98b209d1b555226441829877031336b84cc7f2f083`  
		Last Modified: Tue, 18 Apr 2023 03:23:05 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11-slim` - linux; ppc64le

```console
$ docker pull solr@sha256:89193853b9976c1e9bf28386f66c7fc5fca07d300011b106e1336e61c60a1642
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.1 MB (317097124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e4efdfa11f4e85646d5c547f7ba3db1ceb897451de41508ad75533c2f5786f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:06:30 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:06:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:06:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:07:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:19:05 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:21:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:21:50 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:41:58 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 26 Apr 2023 20:41:58 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 26 Apr 2023 20:41:58 GMT
ARG SOLR_VERSION=8.11.2
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:42:14 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 26 Apr 2023 20:42:14 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 26 Apr 2023 20:42:16 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:42:37 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 26 Apr 2023 20:43:05 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 26 Apr 2023 20:43:08 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 26 Apr 2023 20:43:08 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:43:09 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:43:09 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:43:09 GMT
USER 8983
# Wed, 26 Apr 2023 20:43:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:43:10 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:d276072145993a42aed3e2b3e8cd26b6e08aab266d9c9d792ee89b26150681da`  
		Last Modified: Fri, 14 Apr 2023 09:36:00 GMT  
		Size: 33.3 MB (33300980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4018ee3c8b327c120bbf0427fb12e76c74cb054a92177aeeae16bcf0efa4e86`  
		Last Modified: Tue, 18 Apr 2023 01:11:24 GMT  
		Size: 17.6 MB (17582531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68132c1824ed616e2aa64a0252f82705524204a2dcc79d1bbf7f8a481f482bc0`  
		Last Modified: Wed, 26 Apr 2023 19:32:54 GMT  
		Size: 42.1 MB (42093906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705220513c41d99a8d5e529e29488b3b903dad838d853121dc9cbf9dcb950209`  
		Last Modified: Wed, 26 Apr 2023 19:32:43 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a018bd1c2d0feb9fe5b7c849d3b3d1bc427f062719f198d72eaf9eb16e1305b`  
		Last Modified: Wed, 26 Apr 2023 20:45:12 GMT  
		Size: 5.8 MB (5777193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65368a709ae0c7650e4198a55b2881827eb073d63097628050704e0542e86e3`  
		Last Modified: Wed, 26 Apr 2023 20:45:11 GMT  
		Size: 4.3 KB (4299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b057f087dfda706087959b2cbe2f9badb9984f26149834861a9e8bbfcfc6bb40`  
		Last Modified: Wed, 26 Apr 2023 20:45:11 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e36d02c2b4075d6f7050b9befb0e3b722f04cd0d99de9c8f7485a2dbf232f2`  
		Last Modified: Wed, 26 Apr 2023 20:45:29 GMT  
		Size: 218.3 MB (218328281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed30ffc679a350213ccaeb74148aef8cfec6c885c4264b98898b15fc32956f2`  
		Last Modified: Wed, 26 Apr 2023 20:45:11 GMT  
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
$ docker pull solr@sha256:2607eca8ca54a2d91d2f32300a2bc2917150c7f2338b4bae5c149d2c24c800cb
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
$ docker pull solr@sha256:b210a1886da5e6bd04b978e092ad2282fefb2b2ab9e928465b5c6d4cad58497d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.8 MB (314801289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fee171281dcf64fb86a69dad1e9390dee50678fea5dc79f0259935b9760cd04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 00:42:52 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 00:42:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 00:42:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 00:43:22 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 00:43:54 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 00:44:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:20 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 05:38:29 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Tue, 18 Apr 2023 05:38:29 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Tue, 18 Apr 2023 05:38:29 GMT
ARG SOLR_VERSION=8.11.2
# Tue, 18 Apr 2023 05:38:29 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Tue, 18 Apr 2023 05:38:30 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Tue, 18 Apr 2023 05:38:30 GMT
ARG SOLR_DOWNLOAD_URL
# Tue, 18 Apr 2023 05:38:30 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 18 Apr 2023 05:38:37 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Tue, 18 Apr 2023 05:38:37 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Tue, 18 Apr 2023 05:38:37 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 18 Apr 2023 05:38:46 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Tue, 18 Apr 2023 05:39:20 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Tue, 18 Apr 2023 05:39:20 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Tue, 18 Apr 2023 05:39:20 GMT
VOLUME [/var/solr]
# Tue, 18 Apr 2023 05:39:20 GMT
EXPOSE 8983
# Tue, 18 Apr 2023 05:39:20 GMT
WORKDIR /opt/solr
# Tue, 18 Apr 2023 05:39:20 GMT
USER 8983
# Tue, 18 Apr 2023 05:39:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 05:39:21 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7affba4c9a33ed5dd050532c0d53e38b2c35c2fe490db721d943658feee4c914`  
		Last Modified: Tue, 18 Apr 2023 00:46:23 GMT  
		Size: 16.3 MB (16347011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fb5d08d03b0834295af88b5b911dca1240bcbdc3268dbc4c8ce24934ae017e`  
		Last Modified: Tue, 18 Apr 2023 00:47:26 GMT  
		Size: 46.6 MB (46632203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ef4a2443f5b89eae76a92c01bf3a006c986bb4fe658aa46a8dccc0bed2f523`  
		Last Modified: Tue, 18 Apr 2023 00:47:19 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e005372261eff41e611105a513fed9afaef08b30a879c639a8ac0efafd9300`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 4.9 MB (4901010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad0a251b15f3c813079323fdb45751b01c5753143b2c5dc1c6665bcc3e2680c`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 4.3 KB (4291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53da2eb3eae194651c65ebab849877740d6128968fd6e3f78f1a669b1ecb73d`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2462511e3bac8b859994f31534f2cfff6f8bfc787b5dc0909219b61ba839fdd1`  
		Last Modified: Tue, 18 Apr 2023 05:40:25 GMT  
		Size: 218.3 MB (218328276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7090d8a3f08936349556e936cfd4a9bfb2cd6661eeab03630417cee2cad95bfd`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11.2` - linux; arm variant v7

```console
$ docker pull solr@sha256:6dafcadde2e7a193d0625f280e2682fd53f6d499b74d4af8025e660f6f25a348
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.2 MB (307180449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0dd03a8533275b4869866465fbd3cb5250aa0d685f1cef49c33f55f3e477b90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:52:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:52:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:52:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:52:26 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:58:18 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:58:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:58:58 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:55:48 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 26 Apr 2023 20:55:48 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 26 Apr 2023 20:55:48 GMT
ARG SOLR_VERSION=8.11.2
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:55:55 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 26 Apr 2023 20:55:55 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 26 Apr 2023 20:55:56 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:56:04 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 26 Apr 2023 20:56:41 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 26 Apr 2023 20:56:42 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 26 Apr 2023 20:56:42 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:56:42 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:56:42 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:56:42 GMT
USER 8983
# Wed, 26 Apr 2023 20:56:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:56:42 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:e68c91cb250f35160f683afa80c3ada46f06948ded46a188be490ea3afff08f5`  
		Last Modified: Fri, 14 Apr 2023 09:34:28 GMT  
		Size: 24.6 MB (24586976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26020bb58aaff7bb6175448d285783e1d1698e726bcba90502c721abc88f2a2`  
		Last Modified: Tue, 18 Apr 2023 01:54:29 GMT  
		Size: 15.2 MB (15177669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6beb6c54ed90fe5685ff23c9c1c5c2e8f9cfb87d68e53bccd8a0ba8ea6bb45e`  
		Last Modified: Wed, 26 Apr 2023 20:01:25 GMT  
		Size: 44.9 MB (44878110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2be4736e459b5628fd2b307c8d7943b3f55d8dccdd160ec14322808c4042aa`  
		Last Modified: Wed, 26 Apr 2023 20:01:18 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f5442bfaa9ed3f392420670361ffe3de09563936eafbb08e3d1751bd41fe08`  
		Last Modified: Wed, 26 Apr 2023 20:58:05 GMT  
		Size: 4.2 MB (4195197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092c315c9b467de64195ac22278518557f4a1786ce8531d558c69b7baa3795c1`  
		Last Modified: Wed, 26 Apr 2023 20:58:04 GMT  
		Size: 4.2 KB (4229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc80305416e522db899c313b1d14efc8a78c84b41c6f7e823d6d065651db97df`  
		Last Modified: Wed, 26 Apr 2023 20:58:04 GMT  
		Size: 3.5 KB (3465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b3deffe546af271360886735be91826cf5dadf35b44ec9886d3c0fd0b41681`  
		Last Modified: Wed, 26 Apr 2023 20:58:16 GMT  
		Size: 218.3 MB (218328333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27437b66908cc998c75f64e651aa564eadd0eb13069222b57e72d0553f0f7362`  
		Last Modified: Wed, 26 Apr 2023 20:58:04 GMT  
		Size: 6.3 KB (6310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11.2` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:9c83437dd68f23bd3272fa16658b6bb0a96b4c47b0e19257d018071f1cbfe495
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.5 MB (311481859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee0bcfc19e6f7e821e073ab8496a566a25ab40161cd530e90512c5f46ed1bf67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:40:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:40:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:40:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:41:09 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:41:31 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 01:41:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 01:41:55 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 03:21:22 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Tue, 18 Apr 2023 03:21:23 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_VERSION=8.11.2
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_DOWNLOAD_URL
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 18 Apr 2023 03:21:28 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Tue, 18 Apr 2023 03:21:29 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Tue, 18 Apr 2023 03:21:29 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 18 Apr 2023 03:21:43 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Tue, 18 Apr 2023 03:22:14 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Tue, 18 Apr 2023 03:22:16 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Tue, 18 Apr 2023 03:22:16 GMT
VOLUME [/var/solr]
# Tue, 18 Apr 2023 03:22:16 GMT
EXPOSE 8983
# Tue, 18 Apr 2023 03:22:16 GMT
WORKDIR /opt/solr
# Tue, 18 Apr 2023 03:22:16 GMT
USER 8983
# Tue, 18 Apr 2023 03:22:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 03:22:16 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269336393c4662b72ac4a2be29473801366e79f4db6c8b9944509f1903ee3fe6`  
		Last Modified: Tue, 18 Apr 2023 01:43:30 GMT  
		Size: 16.2 MB (16213349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5775e69497bdf42d2ad7b39be6112c42f7fb711efa0036c55e9a5ddf8b30c244`  
		Last Modified: Tue, 18 Apr 2023 01:44:26 GMT  
		Size: 45.0 MB (44979459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff94c7a5594b10847f2895eb9f20938960ec3194f7398f5da8e801aff22ab00`  
		Last Modified: Tue, 18 Apr 2023 01:44:21 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3419bf7e5540a3bcd6132aa79f49429981574fb43627e2e617efd771123733e`  
		Last Modified: Tue, 18 Apr 2023 03:23:06 GMT  
		Size: 4.8 MB (4750130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f986cb8a544e5f5ed858bfd84e22a07cc5d8d5133bf126062e34097fb071cea9`  
		Last Modified: Tue, 18 Apr 2023 03:23:05 GMT  
		Size: 4.3 KB (4335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46abce6c72ed3766b9f8dfbfadcecd21ca0597eef161bd3ef3b10408b72ae346`  
		Last Modified: Tue, 18 Apr 2023 03:23:05 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbfb9f1a96f5d4bb8867ba070a31604ef992f2fe5672efd1775b3f3335be352`  
		Last Modified: Tue, 18 Apr 2023 03:23:15 GMT  
		Size: 218.3 MB (218328255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6099366efb07d013239cc98b209d1b555226441829877031336b84cc7f2f083`  
		Last Modified: Tue, 18 Apr 2023 03:23:05 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11.2` - linux; ppc64le

```console
$ docker pull solr@sha256:89193853b9976c1e9bf28386f66c7fc5fca07d300011b106e1336e61c60a1642
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.1 MB (317097124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e4efdfa11f4e85646d5c547f7ba3db1ceb897451de41508ad75533c2f5786f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:06:30 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:06:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:06:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:07:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:19:05 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:21:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:21:50 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:41:58 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 26 Apr 2023 20:41:58 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 26 Apr 2023 20:41:58 GMT
ARG SOLR_VERSION=8.11.2
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:42:14 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 26 Apr 2023 20:42:14 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 26 Apr 2023 20:42:16 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:42:37 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 26 Apr 2023 20:43:05 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 26 Apr 2023 20:43:08 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 26 Apr 2023 20:43:08 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:43:09 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:43:09 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:43:09 GMT
USER 8983
# Wed, 26 Apr 2023 20:43:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:43:10 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:d276072145993a42aed3e2b3e8cd26b6e08aab266d9c9d792ee89b26150681da`  
		Last Modified: Fri, 14 Apr 2023 09:36:00 GMT  
		Size: 33.3 MB (33300980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4018ee3c8b327c120bbf0427fb12e76c74cb054a92177aeeae16bcf0efa4e86`  
		Last Modified: Tue, 18 Apr 2023 01:11:24 GMT  
		Size: 17.6 MB (17582531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68132c1824ed616e2aa64a0252f82705524204a2dcc79d1bbf7f8a481f482bc0`  
		Last Modified: Wed, 26 Apr 2023 19:32:54 GMT  
		Size: 42.1 MB (42093906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705220513c41d99a8d5e529e29488b3b903dad838d853121dc9cbf9dcb950209`  
		Last Modified: Wed, 26 Apr 2023 19:32:43 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a018bd1c2d0feb9fe5b7c849d3b3d1bc427f062719f198d72eaf9eb16e1305b`  
		Last Modified: Wed, 26 Apr 2023 20:45:12 GMT  
		Size: 5.8 MB (5777193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65368a709ae0c7650e4198a55b2881827eb073d63097628050704e0542e86e3`  
		Last Modified: Wed, 26 Apr 2023 20:45:11 GMT  
		Size: 4.3 KB (4299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b057f087dfda706087959b2cbe2f9badb9984f26149834861a9e8bbfcfc6bb40`  
		Last Modified: Wed, 26 Apr 2023 20:45:11 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e36d02c2b4075d6f7050b9befb0e3b722f04cd0d99de9c8f7485a2dbf232f2`  
		Last Modified: Wed, 26 Apr 2023 20:45:29 GMT  
		Size: 218.3 MB (218328281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed30ffc679a350213ccaeb74148aef8cfec6c885c4264b98898b15fc32956f2`  
		Last Modified: Wed, 26 Apr 2023 20:45:11 GMT  
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
$ docker pull solr@sha256:2607eca8ca54a2d91d2f32300a2bc2917150c7f2338b4bae5c149d2c24c800cb
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
$ docker pull solr@sha256:b210a1886da5e6bd04b978e092ad2282fefb2b2ab9e928465b5c6d4cad58497d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.8 MB (314801289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fee171281dcf64fb86a69dad1e9390dee50678fea5dc79f0259935b9760cd04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 00:42:52 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 00:42:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 00:42:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 00:43:22 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 00:43:54 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 00:44:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:20 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 05:38:29 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Tue, 18 Apr 2023 05:38:29 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Tue, 18 Apr 2023 05:38:29 GMT
ARG SOLR_VERSION=8.11.2
# Tue, 18 Apr 2023 05:38:29 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Tue, 18 Apr 2023 05:38:30 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Tue, 18 Apr 2023 05:38:30 GMT
ARG SOLR_DOWNLOAD_URL
# Tue, 18 Apr 2023 05:38:30 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 18 Apr 2023 05:38:37 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Tue, 18 Apr 2023 05:38:37 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Tue, 18 Apr 2023 05:38:37 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 18 Apr 2023 05:38:46 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Tue, 18 Apr 2023 05:39:20 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Tue, 18 Apr 2023 05:39:20 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Tue, 18 Apr 2023 05:39:20 GMT
VOLUME [/var/solr]
# Tue, 18 Apr 2023 05:39:20 GMT
EXPOSE 8983
# Tue, 18 Apr 2023 05:39:20 GMT
WORKDIR /opt/solr
# Tue, 18 Apr 2023 05:39:20 GMT
USER 8983
# Tue, 18 Apr 2023 05:39:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 05:39:21 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7affba4c9a33ed5dd050532c0d53e38b2c35c2fe490db721d943658feee4c914`  
		Last Modified: Tue, 18 Apr 2023 00:46:23 GMT  
		Size: 16.3 MB (16347011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fb5d08d03b0834295af88b5b911dca1240bcbdc3268dbc4c8ce24934ae017e`  
		Last Modified: Tue, 18 Apr 2023 00:47:26 GMT  
		Size: 46.6 MB (46632203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ef4a2443f5b89eae76a92c01bf3a006c986bb4fe658aa46a8dccc0bed2f523`  
		Last Modified: Tue, 18 Apr 2023 00:47:19 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e005372261eff41e611105a513fed9afaef08b30a879c639a8ac0efafd9300`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 4.9 MB (4901010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad0a251b15f3c813079323fdb45751b01c5753143b2c5dc1c6665bcc3e2680c`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 4.3 KB (4291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53da2eb3eae194651c65ebab849877740d6128968fd6e3f78f1a669b1ecb73d`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2462511e3bac8b859994f31534f2cfff6f8bfc787b5dc0909219b61ba839fdd1`  
		Last Modified: Tue, 18 Apr 2023 05:40:25 GMT  
		Size: 218.3 MB (218328276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7090d8a3f08936349556e936cfd4a9bfb2cd6661eeab03630417cee2cad95bfd`  
		Last Modified: Tue, 18 Apr 2023 05:40:16 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11.2-slim` - linux; arm variant v7

```console
$ docker pull solr@sha256:6dafcadde2e7a193d0625f280e2682fd53f6d499b74d4af8025e660f6f25a348
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.2 MB (307180449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0dd03a8533275b4869866465fbd3cb5250aa0d685f1cef49c33f55f3e477b90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:52:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:52:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:52:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:52:26 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:58:18 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:58:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:58:58 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:55:48 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 26 Apr 2023 20:55:48 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 26 Apr 2023 20:55:48 GMT
ARG SOLR_VERSION=8.11.2
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:55:49 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:55:55 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 26 Apr 2023 20:55:55 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 26 Apr 2023 20:55:56 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:56:04 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 26 Apr 2023 20:56:41 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 26 Apr 2023 20:56:42 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 26 Apr 2023 20:56:42 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:56:42 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:56:42 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:56:42 GMT
USER 8983
# Wed, 26 Apr 2023 20:56:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:56:42 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:e68c91cb250f35160f683afa80c3ada46f06948ded46a188be490ea3afff08f5`  
		Last Modified: Fri, 14 Apr 2023 09:34:28 GMT  
		Size: 24.6 MB (24586976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26020bb58aaff7bb6175448d285783e1d1698e726bcba90502c721abc88f2a2`  
		Last Modified: Tue, 18 Apr 2023 01:54:29 GMT  
		Size: 15.2 MB (15177669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6beb6c54ed90fe5685ff23c9c1c5c2e8f9cfb87d68e53bccd8a0ba8ea6bb45e`  
		Last Modified: Wed, 26 Apr 2023 20:01:25 GMT  
		Size: 44.9 MB (44878110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2be4736e459b5628fd2b307c8d7943b3f55d8dccdd160ec14322808c4042aa`  
		Last Modified: Wed, 26 Apr 2023 20:01:18 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f5442bfaa9ed3f392420670361ffe3de09563936eafbb08e3d1751bd41fe08`  
		Last Modified: Wed, 26 Apr 2023 20:58:05 GMT  
		Size: 4.2 MB (4195197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092c315c9b467de64195ac22278518557f4a1786ce8531d558c69b7baa3795c1`  
		Last Modified: Wed, 26 Apr 2023 20:58:04 GMT  
		Size: 4.2 KB (4229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc80305416e522db899c313b1d14efc8a78c84b41c6f7e823d6d065651db97df`  
		Last Modified: Wed, 26 Apr 2023 20:58:04 GMT  
		Size: 3.5 KB (3465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b3deffe546af271360886735be91826cf5dadf35b44ec9886d3c0fd0b41681`  
		Last Modified: Wed, 26 Apr 2023 20:58:16 GMT  
		Size: 218.3 MB (218328333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27437b66908cc998c75f64e651aa564eadd0eb13069222b57e72d0553f0f7362`  
		Last Modified: Wed, 26 Apr 2023 20:58:04 GMT  
		Size: 6.3 KB (6310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11.2-slim` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:9c83437dd68f23bd3272fa16658b6bb0a96b4c47b0e19257d018071f1cbfe495
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.5 MB (311481859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee0bcfc19e6f7e821e073ab8496a566a25ab40161cd530e90512c5f46ed1bf67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:40:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:40:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:40:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:41:09 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:41:31 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 01:41:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 01:41:55 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 03:21:22 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Tue, 18 Apr 2023 03:21:23 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_VERSION=8.11.2
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_DOWNLOAD_URL
# Tue, 18 Apr 2023 03:21:23 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 18 Apr 2023 03:21:28 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Tue, 18 Apr 2023 03:21:29 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Tue, 18 Apr 2023 03:21:29 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 18 Apr 2023 03:21:43 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Tue, 18 Apr 2023 03:22:14 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Tue, 18 Apr 2023 03:22:16 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Tue, 18 Apr 2023 03:22:16 GMT
VOLUME [/var/solr]
# Tue, 18 Apr 2023 03:22:16 GMT
EXPOSE 8983
# Tue, 18 Apr 2023 03:22:16 GMT
WORKDIR /opt/solr
# Tue, 18 Apr 2023 03:22:16 GMT
USER 8983
# Tue, 18 Apr 2023 03:22:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 03:22:16 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269336393c4662b72ac4a2be29473801366e79f4db6c8b9944509f1903ee3fe6`  
		Last Modified: Tue, 18 Apr 2023 01:43:30 GMT  
		Size: 16.2 MB (16213349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5775e69497bdf42d2ad7b39be6112c42f7fb711efa0036c55e9a5ddf8b30c244`  
		Last Modified: Tue, 18 Apr 2023 01:44:26 GMT  
		Size: 45.0 MB (44979459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff94c7a5594b10847f2895eb9f20938960ec3194f7398f5da8e801aff22ab00`  
		Last Modified: Tue, 18 Apr 2023 01:44:21 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3419bf7e5540a3bcd6132aa79f49429981574fb43627e2e617efd771123733e`  
		Last Modified: Tue, 18 Apr 2023 03:23:06 GMT  
		Size: 4.8 MB (4750130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f986cb8a544e5f5ed858bfd84e22a07cc5d8d5133bf126062e34097fb071cea9`  
		Last Modified: Tue, 18 Apr 2023 03:23:05 GMT  
		Size: 4.3 KB (4335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46abce6c72ed3766b9f8dfbfadcecd21ca0597eef161bd3ef3b10408b72ae346`  
		Last Modified: Tue, 18 Apr 2023 03:23:05 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbfb9f1a96f5d4bb8867ba070a31604ef992f2fe5672efd1775b3f3335be352`  
		Last Modified: Tue, 18 Apr 2023 03:23:15 GMT  
		Size: 218.3 MB (218328255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6099366efb07d013239cc98b209d1b555226441829877031336b84cc7f2f083`  
		Last Modified: Tue, 18 Apr 2023 03:23:05 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11.2-slim` - linux; ppc64le

```console
$ docker pull solr@sha256:89193853b9976c1e9bf28386f66c7fc5fca07d300011b106e1336e61c60a1642
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.1 MB (317097124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e4efdfa11f4e85646d5c547f7ba3db1ceb897451de41508ad75533c2f5786f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:06:30 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:06:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:06:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:07:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:19:05 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:21:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:21:50 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:41:58 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 26 Apr 2023 20:41:58 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 26 Apr 2023 20:41:58 GMT
ARG SOLR_VERSION=8.11.2
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:41:59 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:42:14 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v2.0/jattach; chmod 755 jattach;   echo >jattach.sha512 "a19e774600d6aa844bceb2189285848127a70130a69fb1840c10367f3360972c733b3f09e60e9672d387e2d48c750ab56acfe8f80f7c6af76f5d1123e5ad7222  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 26 Apr 2023 20:42:14 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.2/solr-8.11.2.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.2/solr-8.11.2.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 26 Apr 2023 20:42:16 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:42:37 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 26 Apr 2023 20:43:05 GMT
# ARGS: SOLR_KEYS=86EDB9C33B8517228E88A8F93E48C0C6EF362B9E SOLR_SHA512=22fedcc0090eda72c3c5a5ea769c93adaf7d92c5c4479993f009ef0b9d42de5bd2ed1e0565ca01f3428587d8a3836286aa3017aab157050f2bd5bc3482fdebaa SOLR_VERSION=8.11.2
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 26 Apr 2023 20:43:08 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 26 Apr 2023 20:43:08 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:43:09 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:43:09 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:43:09 GMT
USER 8983
# Wed, 26 Apr 2023 20:43:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:43:10 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:d276072145993a42aed3e2b3e8cd26b6e08aab266d9c9d792ee89b26150681da`  
		Last Modified: Fri, 14 Apr 2023 09:36:00 GMT  
		Size: 33.3 MB (33300980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4018ee3c8b327c120bbf0427fb12e76c74cb054a92177aeeae16bcf0efa4e86`  
		Last Modified: Tue, 18 Apr 2023 01:11:24 GMT  
		Size: 17.6 MB (17582531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68132c1824ed616e2aa64a0252f82705524204a2dcc79d1bbf7f8a481f482bc0`  
		Last Modified: Wed, 26 Apr 2023 19:32:54 GMT  
		Size: 42.1 MB (42093906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705220513c41d99a8d5e529e29488b3b903dad838d853121dc9cbf9dcb950209`  
		Last Modified: Wed, 26 Apr 2023 19:32:43 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a018bd1c2d0feb9fe5b7c849d3b3d1bc427f062719f198d72eaf9eb16e1305b`  
		Last Modified: Wed, 26 Apr 2023 20:45:12 GMT  
		Size: 5.8 MB (5777193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65368a709ae0c7650e4198a55b2881827eb073d63097628050704e0542e86e3`  
		Last Modified: Wed, 26 Apr 2023 20:45:11 GMT  
		Size: 4.3 KB (4299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b057f087dfda706087959b2cbe2f9badb9984f26149834861a9e8bbfcfc6bb40`  
		Last Modified: Wed, 26 Apr 2023 20:45:11 GMT  
		Size: 3.5 KB (3467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e36d02c2b4075d6f7050b9befb0e3b722f04cd0d99de9c8f7485a2dbf232f2`  
		Last Modified: Wed, 26 Apr 2023 20:45:29 GMT  
		Size: 218.3 MB (218328281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed30ffc679a350213ccaeb74148aef8cfec6c885c4264b98898b15fc32956f2`  
		Last Modified: Wed, 26 Apr 2023 20:45:11 GMT  
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
$ docker pull solr@sha256:6607abbaa3fb4314f8aafbc9f427ae13561bc0c5a8ec4290cf0e2b2e9cf5d55b
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
$ docker pull solr@sha256:cbee52e4b6a1e30d450e8ca19402c3bc15d4d8e8a75ca8501cb0f7f642cc76ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.9 MB (374859971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7d43c32e8ee6e715af99f55ba48e134125af6eadbc175932523f25a1070ce4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:44:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 02:44:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 02:44:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 02:46:48 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:46:48 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Thu, 16 Mar 2023 02:47:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 16 Mar 2023 02:47:22 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_VERSION=9.2.0
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:20:07 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:20:52 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.version=9.2.0
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 24 Mar 2023 20:20:53 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 24 Mar 2023 20:20:54 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 24 Mar 2023 20:20:55 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 24 Mar 2023 20:20:55 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 24 Mar 2023 20:21:03 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 24 Mar 2023 20:21:03 GMT
VOLUME [/var/solr]
# Fri, 24 Mar 2023 20:21:03 GMT
EXPOSE 8983
# Fri, 24 Mar 2023 20:21:03 GMT
WORKDIR /opt/solr
# Fri, 24 Mar 2023 20:21:04 GMT
USER 8983
# Fri, 24 Mar 2023 20:21:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Mar 2023 20:21:04 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a182a611d05b01879f065473c49fb968b8d30312f931350ea07af1c46aa8b4f9`  
		Last Modified: Thu, 16 Mar 2023 02:53:08 GMT  
		Size: 17.0 MB (16975402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb51f9f63778bb9fb97f2cb054b54dfc5098aba2931664a12930c35cf464ca6`  
		Last Modified: Thu, 16 Mar 2023 02:54:00 GMT  
		Size: 46.9 MB (46935467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1365afd8cae0153f1c2bfcf8a4c9b78f2e6e0f18431b0460c63c1fede7507fee`  
		Last Modified: Thu, 16 Mar 2023 02:53:53 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b70190cd6e82c4ac613c9f0f9bf4e42155528b445617672bcd7a211b2a2104`  
		Last Modified: Fri, 24 Mar 2023 20:21:43 GMT  
		Size: 278.7 MB (278678830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c984f04f09ad32d618a63f426eb4127534ca414910aa8b56da2355a3bcf17c17`  
		Last Modified: Fri, 24 Mar 2023 20:21:31 GMT  
		Size: 4.3 KB (4295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888b9068f218433d417da0cd83cca3863ad2cbea9bab37c09fc52a63fab6206e`  
		Last Modified: Fri, 24 Mar 2023 20:21:31 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1599d0444630b3ac11f8d61742ff79acaaec1b9cfcca5e176b131ef54c22bd`  
		Last Modified: Fri, 24 Mar 2023 20:21:32 GMT  
		Size: 8.3 KB (8264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cbc52fa8b34cbd17b27c7c562e83344a928724a395e74a740d6bcfbd0aca1e8`  
		Last Modified: Fri, 24 Mar 2023 20:21:32 GMT  
		Size: 1.8 MB (1827370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9` - linux; arm variant v7

```console
$ docker pull solr@sha256:8544ae0dc85e554f5d5267937f74c720c90b07f1cf05ffc3201f4eb9095b42dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **369.0 MB (369045467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73e472402be480932e64f4a05bda9a60df8996c5852b59ceb376c284295bafa8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:31:41 GMT
ADD file:e9c3ac290fb81ae2e78de99052d776396ee3aff05e1a66fd2dccb01d7de9bb45 in / 
# Wed, 08 Mar 2023 04:31:42 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:46:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 02:46:15 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 02:46:15 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 02:49:36 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:59:26 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:59:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:59:55 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:52:45 GMT
ARG SOLR_VERSION=9.2.0
# Wed, 26 Apr 2023 20:52:45 GMT
ARG SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665
# Wed, 26 Apr 2023 20:52:45 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Wed, 26 Apr 2023 20:52:45 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:52:46 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:52:46 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:52:46 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:52:46 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:53:18 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.version=9.2.0
# Wed, 26 Apr 2023 20:53:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:53:21 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:53:21 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:53:22 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:53:22 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:53:32 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:53:32 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:53:32 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:53:32 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:53:32 GMT
USER 8983
# Wed, 26 Apr 2023 20:53:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:53:33 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:cba1fa3bcdf4f746dcf5b8f86874cee4a6eff75dd5c5cd29e4c912574b12a1c6`  
		Last Modified: Thu, 09 Mar 2023 04:41:14 GMT  
		Size: 27.0 MB (27025397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85169cff2ee4bc04fcfaf94a937435e69eb27ca38bf1dcbd04593cccacf0d702`  
		Last Modified: Thu, 16 Mar 2023 02:56:32 GMT  
		Size: 17.1 MB (17093778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de292b783be3523048fe05ba87f22c3948fb2a4468235c054ea6a35a4f7a053`  
		Last Modified: Wed, 26 Apr 2023 20:03:03 GMT  
		Size: 44.6 MB (44579974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05ce4c34b22f40a9acec67a1a46b86a1435158c0dc9bd6e001f1bf7d77326a5`  
		Last Modified: Wed, 26 Apr 2023 20:02:56 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7651a81ea9e32ab5c6154450135c9f73f51999c9aaa7b801c5f62089fe7acb50`  
		Last Modified: Wed, 26 Apr 2023 20:57:10 GMT  
		Size: 278.7 MB (278680039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bbc9eb9d4ef7ab913012093550bd6110ea6f7556b355caddf44f4b7a8a145fa`  
		Last Modified: Wed, 26 Apr 2023 20:56:56 GMT  
		Size: 4.2 KB (4226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cf324cc98872102c6e9fbf9d55d4a0ab567ca7652ca01e8cc4ffc4e33366b6`  
		Last Modified: Wed, 26 Apr 2023 20:56:56 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddea7d711377bed446cb0468d2e74276ea12f53af7dd1f6975b66c6911baf6b`  
		Last Modified: Wed, 26 Apr 2023 20:56:56 GMT  
		Size: 8.3 KB (8261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac376cfc47e23bc8413e65021ee472c27047ebd1ad83f73d4053e0a55edcd477`  
		Last Modified: Wed, 26 Apr 2023 20:56:56 GMT  
		Size: 1.7 MB (1653413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:58619b9500a6637702a27985f2cf8b17cb13dae6c2673f3abaa9a1bd824277ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **373.6 MB (373587696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25f72e1df4e02c02f553d7d54dd64951829dbdd59095775a6634ddce70eadc8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:52:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 01:52:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 01:52:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 01:55:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:55:04 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Thu, 16 Mar 2023 01:55:29 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 16 Mar 2023 01:55:30 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_VERSION=9.2.0
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:47:31 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:47:31 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:48:14 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 24 Mar 2023 20:48:17 GMT
LABEL org.opencontainers.image.version=9.2.0
# Fri, 24 Mar 2023 20:48:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 24 Mar 2023 20:48:17 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 24 Mar 2023 20:48:17 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 24 Mar 2023 20:48:18 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 24 Mar 2023 20:48:18 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 24 Mar 2023 20:48:27 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 24 Mar 2023 20:48:27 GMT
VOLUME [/var/solr]
# Fri, 24 Mar 2023 20:48:27 GMT
EXPOSE 8983
# Fri, 24 Mar 2023 20:48:27 GMT
WORKDIR /opt/solr
# Fri, 24 Mar 2023 20:48:28 GMT
USER 8983
# Fri, 24 Mar 2023 20:48:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Mar 2023 20:48:28 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40b70fd7935308ad0e072e7e06ec8c3abdc59beae70ca716dcd04e971680865`  
		Last Modified: Thu, 16 Mar 2023 02:00:42 GMT  
		Size: 18.4 MB (18400790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33dd5efa5ce73b25dc0236fcd408527b63e42c87e6da9672a356731004b8949`  
		Last Modified: Thu, 16 Mar 2023 02:01:25 GMT  
		Size: 46.4 MB (46421360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ce9280353ea6c4511dc5378e2f0f4742d499bf6df15c8d10804513c8c5115a`  
		Last Modified: Thu, 16 Mar 2023 02:01:20 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85ed965ce21582560c60a815ae59ae9cf0fcb5c9270ba02dfc5ca1c135b44f`  
		Last Modified: Fri, 24 Mar 2023 20:49:04 GMT  
		Size: 278.7 MB (278678702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a47faea25001b6a9178cab60304409e81d636878232dda7e76d519e7490bbc9`  
		Last Modified: Fri, 24 Mar 2023 20:48:54 GMT  
		Size: 4.3 KB (4331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7792e9b554723df7cdd9593ee715d8fe16cfec71a28c58e0b01e2534e7f2c8`  
		Last Modified: Fri, 24 Mar 2023 20:48:54 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9435de9f76e1e09e2078c456e20cd6a83a757671ecc43398fed205b323cb3c6b`  
		Last Modified: Fri, 24 Mar 2023 20:48:54 GMT  
		Size: 8.3 KB (8261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fc7a7f4116bfd1b88180e25c33fa7c4d571df7caad6ffebbec7786b32b2738`  
		Last Modified: Fri, 24 Mar 2023 20:48:54 GMT  
		Size: 1.7 MB (1686320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9` - linux; ppc64le

```console
$ docker pull solr@sha256:f390f3d9f15f1aa1bbad8f1f2e7d13c3cc0599c722e9b9751d40ee71aa084561
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.4 MB (381368174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c8aecc2dc5554acdda867249e249f23bafb21f089ae5b92d1530289c7651a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:16 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:20 GMT
ADD file:d7434a52d8d8aa6288e788f6fe7e156f0e11bf9b8275efaf70aab0bfc4d919cf in / 
# Wed, 08 Mar 2023 04:39:20 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:57:34 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 03:57:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 03:57:35 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 04:03:27 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:23:33 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:26:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:26:14 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:36:53 GMT
ARG SOLR_VERSION=9.2.0
# Wed, 26 Apr 2023 20:36:54 GMT
ARG SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665
# Wed, 26 Apr 2023 20:36:54 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Wed, 26 Apr 2023 20:36:54 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:36:54 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:36:55 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:36:55 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:36:55 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:38:40 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Wed, 26 Apr 2023 20:38:44 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:38:44 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:38:44 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:38:44 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:38:45 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:38:45 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:38:45 GMT
LABEL org.opencontainers.image.version=9.2.0
# Wed, 26 Apr 2023 20:38:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:38:46 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:38:47 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:38:48 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:38:49 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:39:04 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:39:05 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:39:05 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:39:05 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:39:05 GMT
USER 8983
# Wed, 26 Apr 2023 20:39:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:39:06 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:deffc758660db3b0ee7a1f211d720633f06f27ab1e4c31db4caf8c27f4a80eeb`  
		Last Modified: Thu, 16 Mar 2023 02:22:27 GMT  
		Size: 35.7 MB (35711728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c06c33e4689e5957d961321ac18da32bea369d2eccc9173c9ad8b517f802ea`  
		Last Modified: Thu, 16 Mar 2023 04:14:09 GMT  
		Size: 18.3 MB (18257665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25abdd535a180a29cc8edf36ac17eb237551826124456d77040e4d464bceb120`  
		Last Modified: Wed, 26 Apr 2023 19:37:08 GMT  
		Size: 46.9 MB (46872523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9532e0e54e3616e367a6095c24ff50105415ae0333e1fabc59c04be22f053e`  
		Last Modified: Wed, 26 Apr 2023 19:36:55 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182d7fc15b9c08e18cdc6cdf0160b68aa45d1b34992b787cdd7f49c9e030e2c9`  
		Last Modified: Wed, 26 Apr 2023 20:43:58 GMT  
		Size: 278.7 MB (278679581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585651ad84270f628cfb14608c4dbb4e3a7a7d865d31747e5aa6084bd109a1c0`  
		Last Modified: Wed, 26 Apr 2023 20:43:36 GMT  
		Size: 4.3 KB (4298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ed3ec073534fcdcfe0bb91a989a24838b5fae6c4a74b6a898b2dc3694b5407`  
		Last Modified: Wed, 26 Apr 2023 20:43:36 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450540c1db3e7e00d5d9ef4f2fc497c849bf895bc1c6478b3017070f8938b7ee`  
		Last Modified: Wed, 26 Apr 2023 20:43:36 GMT  
		Size: 8.3 KB (8255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9738eccb09731f4eae5b20b3bec3d18ba11a98334974ff4f652999eabd29c1`  
		Last Modified: Wed, 26 Apr 2023 20:43:37 GMT  
		Size: 1.8 MB (1833743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9` - linux; s390x

```console
$ docker pull solr@sha256:3bf7b256991de31d033da2ffbf31cb9b6d95ef615a6b9792a34577903efd2612
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **369.6 MB (369641824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33ecafe05af5a8d70f6d65e63cea1441abacad2ed33f011d1fd02de369e339bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:26 GMT
ADD file:630f9865d3d4fd4294d45cac7cbaea83fb549c2e563de454348da964d19fbbba in / 
# Wed, 08 Mar 2023 04:39:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:06:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 02:06:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 02:06:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 02:07:58 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:43:50 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:44:49 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:44:51 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:34:03 GMT
ARG SOLR_VERSION=9.2.0
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:34:40 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.version=9.2.0
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:34:45 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:34:46 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:34:46 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:34:47 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:34:51 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:34:51 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:34:51 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:34:52 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:34:52 GMT
USER 8983
# Wed, 26 Apr 2023 20:34:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:34:52 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:2c7366af510b72cc0b3456fb93cfa0bfc76f7d383db5cb315967e7b1ce2e0c42`  
		Last Modified: Thu, 16 Mar 2023 02:02:40 GMT  
		Size: 28.6 MB (28647599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d28ae42a862e9773a02317b5a0eeb71ddfe3a887bb001c8f23a2786c926287`  
		Last Modified: Thu, 16 Mar 2023 02:13:35 GMT  
		Size: 16.8 MB (16753284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed61af6a2c87d412802d8f160fb683fc3ec859e336bfe78f93cdcc31e81a5d1a`  
		Last Modified: Wed, 26 Apr 2023 19:48:14 GMT  
		Size: 43.8 MB (43774584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1494ca84bd62528d8f5f078978408f8e5d411da7a46a6065b53e647d1149f5e6`  
		Last Modified: Wed, 26 Apr 2023 19:48:08 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10d1906d4f5008ad00b585c01cb6bdfc068441c94a1d90e8d5945b3b3ddcce6`  
		Last Modified: Wed, 26 Apr 2023 20:37:47 GMT  
		Size: 278.7 MB (278679157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135adf4cb67937fdd1cdf49ca0951324c2a557081953bdf42ed6010b5aadad12`  
		Last Modified: Wed, 26 Apr 2023 20:37:35 GMT  
		Size: 4.3 KB (4329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1770bb3c6b573d4b988aa5479ae3f73c2af9183c16554ec894a2dcb2394a50e`  
		Last Modified: Wed, 26 Apr 2023 20:37:36 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7508a18ea82d8ebe5d57e272b8378f77364d1c20247feab03855086fe8a39fd`  
		Last Modified: Wed, 26 Apr 2023 20:37:36 GMT  
		Size: 8.3 KB (8260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6560f9ee79577800018ac8eba33b185d6cdae6b516d8bb88d5d469a7ddcc2e3a`  
		Last Modified: Wed, 26 Apr 2023 20:37:36 GMT  
		Size: 1.8 MB (1774233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:9.0`

```console
$ docker pull solr@sha256:c38e31f6fc075b337c47bfb75de8b3c6e80a6e39f6ac22bcdcc91a8c73b6fa07
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
$ docker pull solr@sha256:f18526a050126b6147881c8dd4d460a4bbdfee8961af0ff48e4191f37ba9c6b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.9 MB (324868649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6ed6d388f891f47949ba624eca0e87d9d960ff664167f65447e228a008442f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground","-a","-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 00:42:52 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 00:42:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 00:42:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 00:44:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 00:44:48 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Tue, 18 Apr 2023 00:45:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:45:16 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 05:36:36 GMT
ARG SOLR_VERSION=9.0.0
# Tue, 18 Apr 2023 05:36:36 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Tue, 18 Apr 2023 05:36:36 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Tue, 18 Apr 2023 05:36:37 GMT
ARG SOLR_DOWNLOAD_URL
# Tue, 18 Apr 2023 05:36:37 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 18 Apr 2023 05:36:37 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Tue, 18 Apr 2023 05:36:37 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Tue, 18 Apr 2023 05:36:37 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Tue, 18 Apr 2023 05:38:15 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Tue, 18 Apr 2023 05:38:15 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Tue, 18 Apr 2023 05:38:16 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Tue, 18 Apr 2023 05:38:16 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Tue, 18 Apr 2023 05:38:16 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Tue, 18 Apr 2023 05:38:16 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Tue, 18 Apr 2023 05:38:16 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Tue, 18 Apr 2023 05:38:16 GMT
LABEL org.opencontainers.image.version=9.0.0
# Tue, 18 Apr 2023 05:38:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 18 Apr 2023 05:38:16 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Tue, 18 Apr 2023 05:38:17 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 18 Apr 2023 05:38:17 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Tue, 18 Apr 2023 05:38:18 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Tue, 18 Apr 2023 05:38:23 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Tue, 18 Apr 2023 05:38:23 GMT
VOLUME [/var/solr]
# Tue, 18 Apr 2023 05:38:23 GMT
EXPOSE 8983
# Tue, 18 Apr 2023 05:38:23 GMT
WORKDIR /opt/solr
# Tue, 18 Apr 2023 05:38:23 GMT
USER solr
# Tue, 18 Apr 2023 05:38:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 05:38:23 GMT
CMD ["solr-foreground" "-a" "-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b493027a1bf3e6a19b932ebe3c6dbfe19dc6a4583dfe39282977a57c89b31e87`  
		Last Modified: Tue, 18 Apr 2023 00:47:39 GMT  
		Size: 20.1 MB (20096839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02938177297ab7e29f7435f1f8092e05942dc412fbdfa6c1421589d8ef0adb57`  
		Last Modified: Tue, 18 Apr 2023 00:48:08 GMT  
		Size: 46.9 MB (46937043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e9595e3a57ad3c2eaf905104408a625b61809733c58a795c86405e275aea0b`  
		Last Modified: Tue, 18 Apr 2023 00:48:02 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98193c6fa8ee72e820dc54e8630cbd02c47cc281df0d68e994ca080d99640121`  
		Last Modified: Tue, 18 Apr 2023 05:40:08 GMT  
		Size: 227.7 MB (227662006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e117f25a692ce00f5f650f780a4628128f67b5147b2d108763cd51a15fece7`  
		Last Modified: Tue, 18 Apr 2023 05:39:57 GMT  
		Size: 4.3 KB (4295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c44df4002d9a5cc50c30572f7ce52330b70e5bd0dabb2e428900a6668689ede`  
		Last Modified: Tue, 18 Apr 2023 05:39:57 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f2037c2a933d185399697810bbaa8a464d0ff063b932b21edfcaf641068d6b`  
		Last Modified: Tue, 18 Apr 2023 05:39:57 GMT  
		Size: 7.9 KB (7908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb7c6696693b299c6ca775396a3f776e19489087ceb99fbb661b46714595d73`  
		Last Modified: Tue, 18 Apr 2023 05:39:58 GMT  
		Size: 1.6 MB (1581615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.0` - linux; arm variant v7

```console
$ docker pull solr@sha256:277301330f86140d3fe36e6270dc15ab78ba10d75b8c9d4b1fd62cc7df319a78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.2 MB (317181111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65fc12eb48a93c600db373ed8fc25cb210052268a92aff980b588656ae4a9aa2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground","-a","-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:52:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:52:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:52:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:53:36 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:59:07 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:59:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:59:48 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:54:51 GMT
ARG SOLR_VERSION=9.0.0
# Wed, 26 Apr 2023 20:54:51 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Wed, 26 Apr 2023 20:54:51 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Wed, 26 Apr 2023 20:54:51 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:54:51 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:54:51 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Wed, 26 Apr 2023 20:54:52 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Wed, 26 Apr 2023 20:54:52 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Wed, 26 Apr 2023 20:55:37 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Wed, 26 Apr 2023 20:55:38 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:55:38 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:55:38 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:55:38 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:55:38 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:55:39 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:55:39 GMT
LABEL org.opencontainers.image.version=9.0.0
# Wed, 26 Apr 2023 20:55:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:55:39 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:55:39 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:55:40 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:55:40 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:55:45 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:55:45 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:55:45 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:55:45 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:55:45 GMT
USER solr
# Wed, 26 Apr 2023 20:55:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:55:45 GMT
CMD ["solr-foreground" "-a" "-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]
```

-	Layers:
	-	`sha256:e68c91cb250f35160f683afa80c3ada46f06948ded46a188be490ea3afff08f5`  
		Last Modified: Fri, 14 Apr 2023 09:34:28 GMT  
		Size: 24.6 MB (24586976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85796ae94aa6103041abcc6b06ff12a50d94cadaf6e06eb70a7394c3872a6748`  
		Last Modified: Tue, 18 Apr 2023 01:55:40 GMT  
		Size: 19.5 MB (19465888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddecf044ea404868fe676602278605918cf777a58be10ee59c72a7f7b91d23ea`  
		Last Modified: Wed, 26 Apr 2023 20:02:48 GMT  
		Size: 44.6 MB (44580407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d3b70b93915547c3833fab1fff6c2b5ca5742e7b1d1dda6489dc5aee45c0e9`  
		Last Modified: Wed, 26 Apr 2023 20:02:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab067f22a8dbfc54287123275d1539acbc6a612f28b3bc6abe950ec957809290`  
		Last Modified: Wed, 26 Apr 2023 20:57:56 GMT  
		Size: 227.1 MB (227140730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098ecc5eeb4554a2cb63d047616ccdec22a9ab501d72325d706e0ce752e41a04`  
		Last Modified: Wed, 26 Apr 2023 20:57:44 GMT  
		Size: 4.2 KB (4223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045cf6aa534e46e18c82d1e723c16ac5a2dfcdabef58d7181ddb5ff87ca95699`  
		Last Modified: Wed, 26 Apr 2023 20:57:43 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79482ddae88ff1a58bb8400b13080c21481aff8fc549aa570870e115fcadf47`  
		Last Modified: Wed, 26 Apr 2023 20:57:44 GMT  
		Size: 7.9 KB (7899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e39de5143441161fa41d6e459e9530ea9ee6d8b2444772319ffcc7d6b861e2f`  
		Last Modified: Wed, 26 Apr 2023 20:57:44 GMT  
		Size: 1.4 MB (1394609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.0` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:04b463901ac8bde6a6272968ee59681b13ac42b5fc6f51354aa63e950303c655
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.5 MB (323539610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b7d64830b601b2d2e151a405e707709593e852282532226766335d39e6f8d9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground","-a","-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:40:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:40:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:40:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:42:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:42:18 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Tue, 18 Apr 2023 01:42:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 01:42:41 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 03:20:25 GMT
ARG SOLR_VERSION=9.0.0
# Tue, 18 Apr 2023 03:20:25 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Tue, 18 Apr 2023 03:20:25 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Tue, 18 Apr 2023 03:20:26 GMT
ARG SOLR_DOWNLOAD_URL
# Tue, 18 Apr 2023 03:20:26 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 18 Apr 2023 03:20:26 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Tue, 18 Apr 2023 03:20:26 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Tue, 18 Apr 2023 03:20:26 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Tue, 18 Apr 2023 03:21:07 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Tue, 18 Apr 2023 03:21:08 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Tue, 18 Apr 2023 03:21:08 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Tue, 18 Apr 2023 03:21:09 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Tue, 18 Apr 2023 03:21:09 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Tue, 18 Apr 2023 03:21:09 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Tue, 18 Apr 2023 03:21:09 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Tue, 18 Apr 2023 03:21:09 GMT
LABEL org.opencontainers.image.version=9.0.0
# Tue, 18 Apr 2023 03:21:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 18 Apr 2023 03:21:09 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Tue, 18 Apr 2023 03:21:10 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 18 Apr 2023 03:21:10 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Tue, 18 Apr 2023 03:21:11 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Tue, 18 Apr 2023 03:21:14 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Tue, 18 Apr 2023 03:21:14 GMT
VOLUME [/var/solr]
# Tue, 18 Apr 2023 03:21:14 GMT
EXPOSE 8983
# Tue, 18 Apr 2023 03:21:14 GMT
WORKDIR /opt/solr
# Tue, 18 Apr 2023 03:21:14 GMT
USER solr
# Tue, 18 Apr 2023 03:21:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 03:21:15 GMT
CMD ["solr-foreground" "-a" "-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f855dc454f40dbe47d375c509772787d9d27ff505e14349af4f2e3944f28f75`  
		Last Modified: Tue, 18 Apr 2023 01:44:38 GMT  
		Size: 20.8 MB (20815202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c91968e85b36d056d961163f2b9155edf8119f19516132648c5ecae886bcb3`  
		Last Modified: Tue, 18 Apr 2023 01:45:04 GMT  
		Size: 46.4 MB (46422365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6e32ee26ed47aaac9a5a70c0af73a59858c966aa6646cc3b0151c938bf39b1`  
		Last Modified: Tue, 18 Apr 2023 01:44:58 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0524d79428e8b6d258e182e12c143bc4636644497eb2f713d60bdfc592edcd6`  
		Last Modified: Tue, 18 Apr 2023 03:22:57 GMT  
		Size: 227.6 MB (227649927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02d66c108983824382ae01d655355e198973423b56fe3eac73aee5179245f16`  
		Last Modified: Tue, 18 Apr 2023 03:22:48 GMT  
		Size: 4.3 KB (4330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2681b3124697ad3547533a9029d2e44719236d1c5eae31b97c12ac3d5ea9b6`  
		Last Modified: Tue, 18 Apr 2023 03:22:48 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b070826d2cc919b0a9d715e8dc23ac37c6b5068504db8966f7a4ea17da59adf`  
		Last Modified: Tue, 18 Apr 2023 03:22:48 GMT  
		Size: 7.9 KB (7899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c094f24ea3e7d5f503111a9b1379c03432bce9153ceba74dd261b293c853d1f`  
		Last Modified: Tue, 18 Apr 2023 03:22:48 GMT  
		Size: 1.4 MB (1443110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.0` - linux; ppc64le

```console
$ docker pull solr@sha256:f7511434305145641466ed160b2ba32a8509089cd7a1d4e067543f2d0259983c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.4 MB (332376871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3bdf6c51da704ee050930cea56753ade6ddded5001e77c40c5e57a3195d30e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground","-a","-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:06:30 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:06:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:06:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:09:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:22:51 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:25:49 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:25:52 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:40:48 GMT
ARG SOLR_VERSION=9.0.0
# Wed, 26 Apr 2023 20:40:48 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Wed, 26 Apr 2023 20:40:48 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Wed, 26 Apr 2023 20:40:48 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:40:48 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:40:49 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Wed, 26 Apr 2023 20:40:49 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Wed, 26 Apr 2023 20:40:49 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Wed, 26 Apr 2023 20:41:32 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Wed, 26 Apr 2023 20:41:35 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:41:35 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:41:35 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:41:36 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:41:36 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:41:36 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:41:36 GMT
LABEL org.opencontainers.image.version=9.0.0
# Wed, 26 Apr 2023 20:41:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:41:37 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:41:38 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:41:39 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:41:40 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:41:49 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:41:50 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:41:50 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:41:50 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:41:51 GMT
USER solr
# Wed, 26 Apr 2023 20:41:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:41:51 GMT
CMD ["solr-foreground" "-a" "-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]
```

-	Layers:
	-	`sha256:d276072145993a42aed3e2b3e8cd26b6e08aab266d9c9d792ee89b26150681da`  
		Last Modified: Fri, 14 Apr 2023 09:36:00 GMT  
		Size: 33.3 MB (33300980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d16c8f7fe3c69e12b82f6ead20825685acccc07c7db20352690c45095874956`  
		Last Modified: Tue, 18 Apr 2023 01:13:05 GMT  
		Size: 22.1 MB (22066207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6193924dcc6a0c16fcd313f0de2f47c224244a3b32a2e66ac95fb8caf4acb0a3`  
		Last Modified: Wed, 26 Apr 2023 19:36:46 GMT  
		Size: 46.9 MB (46872363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d65ded274243674ad49fb2ed7f15e5ae634747fb0c35f80c742fa2cc980aebe`  
		Last Modified: Wed, 26 Apr 2023 19:36:34 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b60a9e993a2359eb13be1c3dd7cc9d1b680a432e45822c0cfd9805959d0c53`  
		Last Modified: Wed, 26 Apr 2023 20:45:00 GMT  
		Size: 228.5 MB (228520794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1d018ee730b68370b2d20556f3637f2f95b3c6b8af81afa80d639cb32dbe1c`  
		Last Modified: Wed, 26 Apr 2023 20:44:41 GMT  
		Size: 4.3 KB (4295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d826f0a2e7bc4caa8dd9e7d986bb9dfcbabd693f3e5eda30b9418e6128cdab`  
		Last Modified: Wed, 26 Apr 2023 20:44:41 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c9bd5131b72b5e96e04f63bd2567eae6b65d99426f937141092816c9c1e01d`  
		Last Modified: Wed, 26 Apr 2023 20:44:41 GMT  
		Size: 7.9 KB (7903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec4163ecd354d7cfd19c998698a72c234eceaa90ea874bc56dbe58a71a06db4`  
		Last Modified: Wed, 26 Apr 2023 20:44:41 GMT  
		Size: 1.6 MB (1603949 bytes)  
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
$ docker pull solr@sha256:c38e31f6fc075b337c47bfb75de8b3c6e80a6e39f6ac22bcdcc91a8c73b6fa07
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
$ docker pull solr@sha256:f18526a050126b6147881c8dd4d460a4bbdfee8961af0ff48e4191f37ba9c6b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.9 MB (324868649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6ed6d388f891f47949ba624eca0e87d9d960ff664167f65447e228a008442f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground","-a","-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 00:42:52 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 00:42:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 00:42:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 00:44:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 00:44:48 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Tue, 18 Apr 2023 00:45:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:45:16 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 05:36:36 GMT
ARG SOLR_VERSION=9.0.0
# Tue, 18 Apr 2023 05:36:36 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Tue, 18 Apr 2023 05:36:36 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Tue, 18 Apr 2023 05:36:37 GMT
ARG SOLR_DOWNLOAD_URL
# Tue, 18 Apr 2023 05:36:37 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 18 Apr 2023 05:36:37 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Tue, 18 Apr 2023 05:36:37 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Tue, 18 Apr 2023 05:36:37 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Tue, 18 Apr 2023 05:38:15 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Tue, 18 Apr 2023 05:38:15 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Tue, 18 Apr 2023 05:38:16 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Tue, 18 Apr 2023 05:38:16 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Tue, 18 Apr 2023 05:38:16 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Tue, 18 Apr 2023 05:38:16 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Tue, 18 Apr 2023 05:38:16 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Tue, 18 Apr 2023 05:38:16 GMT
LABEL org.opencontainers.image.version=9.0.0
# Tue, 18 Apr 2023 05:38:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 18 Apr 2023 05:38:16 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Tue, 18 Apr 2023 05:38:17 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 18 Apr 2023 05:38:17 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Tue, 18 Apr 2023 05:38:18 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Tue, 18 Apr 2023 05:38:23 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Tue, 18 Apr 2023 05:38:23 GMT
VOLUME [/var/solr]
# Tue, 18 Apr 2023 05:38:23 GMT
EXPOSE 8983
# Tue, 18 Apr 2023 05:38:23 GMT
WORKDIR /opt/solr
# Tue, 18 Apr 2023 05:38:23 GMT
USER solr
# Tue, 18 Apr 2023 05:38:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 05:38:23 GMT
CMD ["solr-foreground" "-a" "-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b493027a1bf3e6a19b932ebe3c6dbfe19dc6a4583dfe39282977a57c89b31e87`  
		Last Modified: Tue, 18 Apr 2023 00:47:39 GMT  
		Size: 20.1 MB (20096839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02938177297ab7e29f7435f1f8092e05942dc412fbdfa6c1421589d8ef0adb57`  
		Last Modified: Tue, 18 Apr 2023 00:48:08 GMT  
		Size: 46.9 MB (46937043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e9595e3a57ad3c2eaf905104408a625b61809733c58a795c86405e275aea0b`  
		Last Modified: Tue, 18 Apr 2023 00:48:02 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98193c6fa8ee72e820dc54e8630cbd02c47cc281df0d68e994ca080d99640121`  
		Last Modified: Tue, 18 Apr 2023 05:40:08 GMT  
		Size: 227.7 MB (227662006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e117f25a692ce00f5f650f780a4628128f67b5147b2d108763cd51a15fece7`  
		Last Modified: Tue, 18 Apr 2023 05:39:57 GMT  
		Size: 4.3 KB (4295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c44df4002d9a5cc50c30572f7ce52330b70e5bd0dabb2e428900a6668689ede`  
		Last Modified: Tue, 18 Apr 2023 05:39:57 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f2037c2a933d185399697810bbaa8a464d0ff063b932b21edfcaf641068d6b`  
		Last Modified: Tue, 18 Apr 2023 05:39:57 GMT  
		Size: 7.9 KB (7908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb7c6696693b299c6ca775396a3f776e19489087ceb99fbb661b46714595d73`  
		Last Modified: Tue, 18 Apr 2023 05:39:58 GMT  
		Size: 1.6 MB (1581615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.0.0` - linux; arm variant v7

```console
$ docker pull solr@sha256:277301330f86140d3fe36e6270dc15ab78ba10d75b8c9d4b1fd62cc7df319a78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.2 MB (317181111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65fc12eb48a93c600db373ed8fc25cb210052268a92aff980b588656ae4a9aa2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground","-a","-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:52:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:52:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:52:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:53:36 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:59:07 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:59:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:59:48 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:54:51 GMT
ARG SOLR_VERSION=9.0.0
# Wed, 26 Apr 2023 20:54:51 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Wed, 26 Apr 2023 20:54:51 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Wed, 26 Apr 2023 20:54:51 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:54:51 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:54:51 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Wed, 26 Apr 2023 20:54:52 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Wed, 26 Apr 2023 20:54:52 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Wed, 26 Apr 2023 20:55:37 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Wed, 26 Apr 2023 20:55:38 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:55:38 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:55:38 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:55:38 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:55:38 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:55:39 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:55:39 GMT
LABEL org.opencontainers.image.version=9.0.0
# Wed, 26 Apr 2023 20:55:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:55:39 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:55:39 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:55:40 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:55:40 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:55:45 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:55:45 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:55:45 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:55:45 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:55:45 GMT
USER solr
# Wed, 26 Apr 2023 20:55:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:55:45 GMT
CMD ["solr-foreground" "-a" "-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]
```

-	Layers:
	-	`sha256:e68c91cb250f35160f683afa80c3ada46f06948ded46a188be490ea3afff08f5`  
		Last Modified: Fri, 14 Apr 2023 09:34:28 GMT  
		Size: 24.6 MB (24586976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85796ae94aa6103041abcc6b06ff12a50d94cadaf6e06eb70a7394c3872a6748`  
		Last Modified: Tue, 18 Apr 2023 01:55:40 GMT  
		Size: 19.5 MB (19465888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddecf044ea404868fe676602278605918cf777a58be10ee59c72a7f7b91d23ea`  
		Last Modified: Wed, 26 Apr 2023 20:02:48 GMT  
		Size: 44.6 MB (44580407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d3b70b93915547c3833fab1fff6c2b5ca5742e7b1d1dda6489dc5aee45c0e9`  
		Last Modified: Wed, 26 Apr 2023 20:02:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab067f22a8dbfc54287123275d1539acbc6a612f28b3bc6abe950ec957809290`  
		Last Modified: Wed, 26 Apr 2023 20:57:56 GMT  
		Size: 227.1 MB (227140730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098ecc5eeb4554a2cb63d047616ccdec22a9ab501d72325d706e0ce752e41a04`  
		Last Modified: Wed, 26 Apr 2023 20:57:44 GMT  
		Size: 4.2 KB (4223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045cf6aa534e46e18c82d1e723c16ac5a2dfcdabef58d7181ddb5ff87ca95699`  
		Last Modified: Wed, 26 Apr 2023 20:57:43 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79482ddae88ff1a58bb8400b13080c21481aff8fc549aa570870e115fcadf47`  
		Last Modified: Wed, 26 Apr 2023 20:57:44 GMT  
		Size: 7.9 KB (7899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e39de5143441161fa41d6e459e9530ea9ee6d8b2444772319ffcc7d6b861e2f`  
		Last Modified: Wed, 26 Apr 2023 20:57:44 GMT  
		Size: 1.4 MB (1394609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.0.0` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:04b463901ac8bde6a6272968ee59681b13ac42b5fc6f51354aa63e950303c655
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.5 MB (323539610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b7d64830b601b2d2e151a405e707709593e852282532226766335d39e6f8d9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground","-a","-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:40:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:40:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:40:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:42:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:42:18 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Tue, 18 Apr 2023 01:42:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 01:42:41 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 03:20:25 GMT
ARG SOLR_VERSION=9.0.0
# Tue, 18 Apr 2023 03:20:25 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Tue, 18 Apr 2023 03:20:25 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Tue, 18 Apr 2023 03:20:26 GMT
ARG SOLR_DOWNLOAD_URL
# Tue, 18 Apr 2023 03:20:26 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 18 Apr 2023 03:20:26 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Tue, 18 Apr 2023 03:20:26 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Tue, 18 Apr 2023 03:20:26 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Tue, 18 Apr 2023 03:21:07 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Tue, 18 Apr 2023 03:21:08 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Tue, 18 Apr 2023 03:21:08 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Tue, 18 Apr 2023 03:21:09 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Tue, 18 Apr 2023 03:21:09 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Tue, 18 Apr 2023 03:21:09 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Tue, 18 Apr 2023 03:21:09 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Tue, 18 Apr 2023 03:21:09 GMT
LABEL org.opencontainers.image.version=9.0.0
# Tue, 18 Apr 2023 03:21:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 18 Apr 2023 03:21:09 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Tue, 18 Apr 2023 03:21:10 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 18 Apr 2023 03:21:10 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Tue, 18 Apr 2023 03:21:11 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Tue, 18 Apr 2023 03:21:14 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Tue, 18 Apr 2023 03:21:14 GMT
VOLUME [/var/solr]
# Tue, 18 Apr 2023 03:21:14 GMT
EXPOSE 8983
# Tue, 18 Apr 2023 03:21:14 GMT
WORKDIR /opt/solr
# Tue, 18 Apr 2023 03:21:14 GMT
USER solr
# Tue, 18 Apr 2023 03:21:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 03:21:15 GMT
CMD ["solr-foreground" "-a" "-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f855dc454f40dbe47d375c509772787d9d27ff505e14349af4f2e3944f28f75`  
		Last Modified: Tue, 18 Apr 2023 01:44:38 GMT  
		Size: 20.8 MB (20815202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c91968e85b36d056d961163f2b9155edf8119f19516132648c5ecae886bcb3`  
		Last Modified: Tue, 18 Apr 2023 01:45:04 GMT  
		Size: 46.4 MB (46422365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6e32ee26ed47aaac9a5a70c0af73a59858c966aa6646cc3b0151c938bf39b1`  
		Last Modified: Tue, 18 Apr 2023 01:44:58 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0524d79428e8b6d258e182e12c143bc4636644497eb2f713d60bdfc592edcd6`  
		Last Modified: Tue, 18 Apr 2023 03:22:57 GMT  
		Size: 227.6 MB (227649927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02d66c108983824382ae01d655355e198973423b56fe3eac73aee5179245f16`  
		Last Modified: Tue, 18 Apr 2023 03:22:48 GMT  
		Size: 4.3 KB (4330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2681b3124697ad3547533a9029d2e44719236d1c5eae31b97c12ac3d5ea9b6`  
		Last Modified: Tue, 18 Apr 2023 03:22:48 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b070826d2cc919b0a9d715e8dc23ac37c6b5068504db8966f7a4ea17da59adf`  
		Last Modified: Tue, 18 Apr 2023 03:22:48 GMT  
		Size: 7.9 KB (7899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c094f24ea3e7d5f503111a9b1379c03432bce9153ceba74dd261b293c853d1f`  
		Last Modified: Tue, 18 Apr 2023 03:22:48 GMT  
		Size: 1.4 MB (1443110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.0.0` - linux; ppc64le

```console
$ docker pull solr@sha256:f7511434305145641466ed160b2ba32a8509089cd7a1d4e067543f2d0259983c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.4 MB (332376871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3bdf6c51da704ee050930cea56753ade6ddded5001e77c40c5e57a3195d30e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground","-a","-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:06:30 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:06:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:06:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:09:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:22:51 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:25:49 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:25:52 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:40:48 GMT
ARG SOLR_VERSION=9.0.0
# Wed, 26 Apr 2023 20:40:48 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Wed, 26 Apr 2023 20:40:48 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Wed, 26 Apr 2023 20:40:48 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:40:48 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:40:49 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Wed, 26 Apr 2023 20:40:49 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Wed, 26 Apr 2023 20:40:49 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Wed, 26 Apr 2023 20:41:32 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Wed, 26 Apr 2023 20:41:35 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:41:35 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:41:35 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:41:36 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:41:36 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:41:36 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:41:36 GMT
LABEL org.opencontainers.image.version=9.0.0
# Wed, 26 Apr 2023 20:41:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:41:37 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:41:38 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:41:39 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:41:40 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:41:49 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:41:50 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:41:50 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:41:50 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:41:51 GMT
USER solr
# Wed, 26 Apr 2023 20:41:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:41:51 GMT
CMD ["solr-foreground" "-a" "-XX:CompileCommand=exclude,com.github.benmanes.caffeine.cache.BoundedLocalCache::put"]
```

-	Layers:
	-	`sha256:d276072145993a42aed3e2b3e8cd26b6e08aab266d9c9d792ee89b26150681da`  
		Last Modified: Fri, 14 Apr 2023 09:36:00 GMT  
		Size: 33.3 MB (33300980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d16c8f7fe3c69e12b82f6ead20825685acccc07c7db20352690c45095874956`  
		Last Modified: Tue, 18 Apr 2023 01:13:05 GMT  
		Size: 22.1 MB (22066207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6193924dcc6a0c16fcd313f0de2f47c224244a3b32a2e66ac95fb8caf4acb0a3`  
		Last Modified: Wed, 26 Apr 2023 19:36:46 GMT  
		Size: 46.9 MB (46872363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d65ded274243674ad49fb2ed7f15e5ae634747fb0c35f80c742fa2cc980aebe`  
		Last Modified: Wed, 26 Apr 2023 19:36:34 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b60a9e993a2359eb13be1c3dd7cc9d1b680a432e45822c0cfd9805959d0c53`  
		Last Modified: Wed, 26 Apr 2023 20:45:00 GMT  
		Size: 228.5 MB (228520794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1d018ee730b68370b2d20556f3637f2f95b3c6b8af81afa80d639cb32dbe1c`  
		Last Modified: Wed, 26 Apr 2023 20:44:41 GMT  
		Size: 4.3 KB (4295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d826f0a2e7bc4caa8dd9e7d986bb9dfcbabd693f3e5eda30b9418e6128cdab`  
		Last Modified: Wed, 26 Apr 2023 20:44:41 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c9bd5131b72b5e96e04f63bd2567eae6b65d99426f937141092816c9c1e01d`  
		Last Modified: Wed, 26 Apr 2023 20:44:41 GMT  
		Size: 7.9 KB (7903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec4163ecd354d7cfd19c998698a72c234eceaa90ea874bc56dbe58a71a06db4`  
		Last Modified: Wed, 26 Apr 2023 20:44:41 GMT  
		Size: 1.6 MB (1603949 bytes)  
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
$ docker pull solr@sha256:d1ba76a1180ae22bcb4080a646d843f5a1d6941ec0f4a02e0ec7a802e7273620
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
$ docker pull solr@sha256:80658a894fbda0918ddb14af9b4f2802ebe65250c10e41d3e344f7f2b6f4d1f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.9 MB (330947807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c10e05a6a28f30bb535d8f21ea16df798f3d8b9e695324911cbceed695df00e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 00:42:52 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 00:42:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 00:42:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 00:44:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 00:44:48 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Tue, 18 Apr 2023 00:45:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:45:16 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 05:34:28 GMT
ARG SOLR_VERSION=9.1.1
# Tue, 18 Apr 2023 05:34:28 GMT
ARG SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f
# Tue, 18 Apr 2023 05:34:28 GMT
ARG SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763
# Tue, 18 Apr 2023 05:34:28 GMT
ARG SOLR_DOWNLOAD_URL
# Tue, 18 Apr 2023 05:34:28 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 18 Apr 2023 05:34:29 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz
# Tue, 18 Apr 2023 05:34:29 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Tue, 18 Apr 2023 05:34:29 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Tue, 18 Apr 2023 05:36:09 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Tue, 18 Apr 2023 05:36:10 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Tue, 18 Apr 2023 05:36:10 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Tue, 18 Apr 2023 05:36:10 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Tue, 18 Apr 2023 05:36:10 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Tue, 18 Apr 2023 05:36:10 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Tue, 18 Apr 2023 05:36:10 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Tue, 18 Apr 2023 05:36:10 GMT
LABEL org.opencontainers.image.version=9.1.1
# Tue, 18 Apr 2023 05:36:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 18 Apr 2023 05:36:10 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Tue, 18 Apr 2023 05:36:11 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 18 Apr 2023 05:36:11 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Tue, 18 Apr 2023 05:36:12 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Tue, 18 Apr 2023 05:36:20 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Tue, 18 Apr 2023 05:36:20 GMT
VOLUME [/var/solr]
# Tue, 18 Apr 2023 05:36:20 GMT
EXPOSE 8983
# Tue, 18 Apr 2023 05:36:20 GMT
WORKDIR /opt/solr
# Tue, 18 Apr 2023 05:36:20 GMT
USER 8983
# Tue, 18 Apr 2023 05:36:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 05:36:20 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b493027a1bf3e6a19b932ebe3c6dbfe19dc6a4583dfe39282977a57c89b31e87`  
		Last Modified: Tue, 18 Apr 2023 00:47:39 GMT  
		Size: 20.1 MB (20096839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02938177297ab7e29f7435f1f8092e05942dc412fbdfa6c1421589d8ef0adb57`  
		Last Modified: Tue, 18 Apr 2023 00:48:08 GMT  
		Size: 46.9 MB (46937043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e9595e3a57ad3c2eaf905104408a625b61809733c58a795c86405e275aea0b`  
		Last Modified: Tue, 18 Apr 2023 00:48:02 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ee77bff8d90cf9a351e1ce423014f4ff0f658293ca052a701886ea666d5fcc`  
		Last Modified: Tue, 18 Apr 2023 05:39:49 GMT  
		Size: 233.7 MB (233740953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5123a34ee6fa079f353e4bc304854acc6ffe3ba9cd2a5bfa47a7d4fda94b88be`  
		Last Modified: Tue, 18 Apr 2023 05:39:38 GMT  
		Size: 4.3 KB (4297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6dfda3f43afacbf8f2eb91877ce1c0f090c255c372e5a4f2022c017dad3ccfd`  
		Last Modified: Tue, 18 Apr 2023 05:39:39 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67d1f2ce2a1c23a9482d1aacca94ff05f266b538c1dd86725e930e309ad625f`  
		Last Modified: Tue, 18 Apr 2023 05:39:38 GMT  
		Size: 8.1 KB (8085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a342ac0282ccec59096fc2e74be5d78fde3c37f3ff8efe643a91945f37386448`  
		Last Modified: Tue, 18 Apr 2023 05:39:39 GMT  
		Size: 1.6 MB (1581649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.1` - linux; arm variant v7

```console
$ docker pull solr@sha256:95d88c5b740feb275a3fd34f161f040db9858bd68c00e04e2922a072d9eaac74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.3 MB (323261228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15750c0611f1a3f7679495e1515b8a02b4243c6c7aa147e31e9e42a53b332fcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:52:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:52:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:52:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:53:36 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:59:07 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:59:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:59:48 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:53:42 GMT
ARG SOLR_VERSION=9.1.1
# Wed, 26 Apr 2023 20:53:42 GMT
ARG SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f
# Wed, 26 Apr 2023 20:53:43 GMT
ARG SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763
# Wed, 26 Apr 2023 20:53:43 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:53:43 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:53:43 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz
# Wed, 26 Apr 2023 20:53:43 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Wed, 26 Apr 2023 20:53:43 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Wed, 26 Apr 2023 20:54:30 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Wed, 26 Apr 2023 20:54:31 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:54:31 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:54:31 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:54:32 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:54:32 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:54:32 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:54:32 GMT
LABEL org.opencontainers.image.version=9.1.1
# Wed, 26 Apr 2023 20:54:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:54:32 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:54:33 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:54:33 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:54:34 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:54:40 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:54:40 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:54:40 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:54:40 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:54:40 GMT
USER 8983
# Wed, 26 Apr 2023 20:54:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:54:40 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:e68c91cb250f35160f683afa80c3ada46f06948ded46a188be490ea3afff08f5`  
		Last Modified: Fri, 14 Apr 2023 09:34:28 GMT  
		Size: 24.6 MB (24586976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85796ae94aa6103041abcc6b06ff12a50d94cadaf6e06eb70a7394c3872a6748`  
		Last Modified: Tue, 18 Apr 2023 01:55:40 GMT  
		Size: 19.5 MB (19465888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddecf044ea404868fe676602278605918cf777a58be10ee59c72a7f7b91d23ea`  
		Last Modified: Wed, 26 Apr 2023 20:02:48 GMT  
		Size: 44.6 MB (44580407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d3b70b93915547c3833fab1fff6c2b5ca5742e7b1d1dda6489dc5aee45c0e9`  
		Last Modified: Wed, 26 Apr 2023 20:02:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e0a3739738b1505d2aa2e77b87f629e7b60ad701cbe80dfeca317de57ea27b`  
		Last Modified: Wed, 26 Apr 2023 20:57:35 GMT  
		Size: 233.2 MB (233220667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a822791bff0f72d4ae55bf4863aebb21a0903a92d9df44e69972202f435a56`  
		Last Modified: Wed, 26 Apr 2023 20:57:23 GMT  
		Size: 4.2 KB (4225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b37a1a5d357ea560dbd09c16429d4253032b5c1eea735ffb080ea774f8c43b`  
		Last Modified: Wed, 26 Apr 2023 20:57:23 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b88d27b99e2f54899bfdc8d7e339bed20cd3781daa0cda9780ce359ba57e069`  
		Last Modified: Wed, 26 Apr 2023 20:57:23 GMT  
		Size: 8.1 KB (8079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55df05b2f152434bc011cee3cc7f7de0efe6d4181cc53b4df82f088e92eed047`  
		Last Modified: Wed, 26 Apr 2023 20:57:23 GMT  
		Size: 1.4 MB (1394606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.1` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:756183ae377d29f4285ffc3ecae5dfbbb5a3ababadb28b12166dd36ddf186549
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.6 MB (329621218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04a7971549dffa1c9364de4726369f6ebf901d6487248614fe8098b27873a4ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:40:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:40:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:40:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:42:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:42:18 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Tue, 18 Apr 2023 01:42:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 01:42:41 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 03:19:28 GMT
ARG SOLR_VERSION=9.1.1
# Tue, 18 Apr 2023 03:19:28 GMT
ARG SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f
# Tue, 18 Apr 2023 03:19:28 GMT
ARG SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763
# Tue, 18 Apr 2023 03:19:28 GMT
ARG SOLR_DOWNLOAD_URL
# Tue, 18 Apr 2023 03:19:28 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 18 Apr 2023 03:19:28 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz
# Tue, 18 Apr 2023 03:19:29 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Tue, 18 Apr 2023 03:19:29 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Tue, 18 Apr 2023 03:20:08 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Tue, 18 Apr 2023 03:20:10 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Tue, 18 Apr 2023 03:20:10 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Tue, 18 Apr 2023 03:20:10 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Tue, 18 Apr 2023 03:20:10 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Tue, 18 Apr 2023 03:20:10 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Tue, 18 Apr 2023 03:20:10 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Tue, 18 Apr 2023 03:20:10 GMT
LABEL org.opencontainers.image.version=9.1.1
# Tue, 18 Apr 2023 03:20:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 18 Apr 2023 03:20:10 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Tue, 18 Apr 2023 03:20:11 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 18 Apr 2023 03:20:11 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Tue, 18 Apr 2023 03:20:12 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Tue, 18 Apr 2023 03:20:19 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Tue, 18 Apr 2023 03:20:19 GMT
VOLUME [/var/solr]
# Tue, 18 Apr 2023 03:20:19 GMT
EXPOSE 8983
# Tue, 18 Apr 2023 03:20:20 GMT
WORKDIR /opt/solr
# Tue, 18 Apr 2023 03:20:20 GMT
USER 8983
# Tue, 18 Apr 2023 03:20:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 03:20:20 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f855dc454f40dbe47d375c509772787d9d27ff505e14349af4f2e3944f28f75`  
		Last Modified: Tue, 18 Apr 2023 01:44:38 GMT  
		Size: 20.8 MB (20815202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c91968e85b36d056d961163f2b9155edf8119f19516132648c5ecae886bcb3`  
		Last Modified: Tue, 18 Apr 2023 01:45:04 GMT  
		Size: 46.4 MB (46422365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6e32ee26ed47aaac9a5a70c0af73a59858c966aa6646cc3b0151c938bf39b1`  
		Last Modified: Tue, 18 Apr 2023 01:44:58 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89355900f95b0a212d969f16b350857c1f2c484164a03a38942d9852b91faa46`  
		Last Modified: Tue, 18 Apr 2023 03:22:40 GMT  
		Size: 233.7 MB (233731364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5d238c8959564a4b0cdc672895e60492cdc82ad83c5d830b141bd5ff5fec7b`  
		Last Modified: Tue, 18 Apr 2023 03:22:31 GMT  
		Size: 4.3 KB (4330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797cde12c943c3478e869d8f23de31c7a29b17971f1b3a7162c2bb3ea213ecc5`  
		Last Modified: Tue, 18 Apr 2023 03:22:31 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5c3e86e33823bf7401a4a0e404d76113f801a1114b2c24a1d9b3e50af3fdcb`  
		Last Modified: Tue, 18 Apr 2023 03:22:31 GMT  
		Size: 8.1 KB (8085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e485d8d417dab6f7edacf648b1b41ec329e3a9cc83e99f106c73681d92dc29`  
		Last Modified: Tue, 18 Apr 2023 03:22:31 GMT  
		Size: 1.4 MB (1443095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.1` - linux; ppc64le

```console
$ docker pull solr@sha256:11c911a63efb87b6dc21c2f20cd7c62ef06c104a0fb4c2367586d2b88ca0f798
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.5 MB (338457239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae26641d93398dfb86ac8cca67ddf6b8feb85383ab79a642536fd8e365a5aa1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:06:30 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:06:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:06:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:09:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:22:51 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:25:49 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:25:52 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:39:23 GMT
ARG SOLR_VERSION=9.1.1
# Wed, 26 Apr 2023 20:39:24 GMT
ARG SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f
# Wed, 26 Apr 2023 20:39:24 GMT
ARG SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763
# Wed, 26 Apr 2023 20:39:24 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:39:25 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:39:25 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz
# Wed, 26 Apr 2023 20:39:25 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Wed, 26 Apr 2023 20:39:25 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Wed, 26 Apr 2023 20:40:10 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Wed, 26 Apr 2023 20:40:13 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:40:13 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:40:14 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:40:14 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:40:14 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:40:14 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:40:15 GMT
LABEL org.opencontainers.image.version=9.1.1
# Wed, 26 Apr 2023 20:40:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:40:15 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:40:17 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:40:18 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:40:19 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:40:30 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:40:30 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:40:31 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:40:31 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:40:31 GMT
USER 8983
# Wed, 26 Apr 2023 20:40:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:40:32 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:d276072145993a42aed3e2b3e8cd26b6e08aab266d9c9d792ee89b26150681da`  
		Last Modified: Fri, 14 Apr 2023 09:36:00 GMT  
		Size: 33.3 MB (33300980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d16c8f7fe3c69e12b82f6ead20825685acccc07c7db20352690c45095874956`  
		Last Modified: Tue, 18 Apr 2023 01:13:05 GMT  
		Size: 22.1 MB (22066207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6193924dcc6a0c16fcd313f0de2f47c224244a3b32a2e66ac95fb8caf4acb0a3`  
		Last Modified: Wed, 26 Apr 2023 19:36:46 GMT  
		Size: 46.9 MB (46872363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d65ded274243674ad49fb2ed7f15e5ae634747fb0c35f80c742fa2cc980aebe`  
		Last Modified: Wed, 26 Apr 2023 19:36:34 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93592fc93b9338f8fdc5a1463c21641cefb5b1d63e3e309fa94a5a013f3ad8f4`  
		Last Modified: Wed, 26 Apr 2023 20:44:31 GMT  
		Size: 234.6 MB (234600951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6bbb832f2610c512b29780ce62e45f1341ad6151a253fa3a7711e605adf60d`  
		Last Modified: Wed, 26 Apr 2023 20:44:12 GMT  
		Size: 4.3 KB (4295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da97cb7ca72b20e1d78b44290c3f42a074df1edf3b5c802b97d92d2627a6c89`  
		Last Modified: Wed, 26 Apr 2023 20:44:12 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848754de971b0ca8cefed25f67295c073d49528aa6e5776c350152c6f7b31f35`  
		Last Modified: Wed, 26 Apr 2023 20:44:12 GMT  
		Size: 8.1 KB (8084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30f79abbb0d6962fee4ec92cd0b9729c0d59b84c4a0d03bd2ff74897fc0fa66`  
		Last Modified: Wed, 26 Apr 2023 20:44:13 GMT  
		Size: 1.6 MB (1603980 bytes)  
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
$ docker pull solr@sha256:d1ba76a1180ae22bcb4080a646d843f5a1d6941ec0f4a02e0ec7a802e7273620
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
$ docker pull solr@sha256:80658a894fbda0918ddb14af9b4f2802ebe65250c10e41d3e344f7f2b6f4d1f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.9 MB (330947807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c10e05a6a28f30bb535d8f21ea16df798f3d8b9e695324911cbceed695df00e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 00:42:52 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 00:42:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 00:42:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 00:44:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 00:44:48 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Tue, 18 Apr 2023 00:45:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:45:16 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 05:34:28 GMT
ARG SOLR_VERSION=9.1.1
# Tue, 18 Apr 2023 05:34:28 GMT
ARG SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f
# Tue, 18 Apr 2023 05:34:28 GMT
ARG SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763
# Tue, 18 Apr 2023 05:34:28 GMT
ARG SOLR_DOWNLOAD_URL
# Tue, 18 Apr 2023 05:34:28 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 18 Apr 2023 05:34:29 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz
# Tue, 18 Apr 2023 05:34:29 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Tue, 18 Apr 2023 05:34:29 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Tue, 18 Apr 2023 05:36:09 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Tue, 18 Apr 2023 05:36:10 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Tue, 18 Apr 2023 05:36:10 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Tue, 18 Apr 2023 05:36:10 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Tue, 18 Apr 2023 05:36:10 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Tue, 18 Apr 2023 05:36:10 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Tue, 18 Apr 2023 05:36:10 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Tue, 18 Apr 2023 05:36:10 GMT
LABEL org.opencontainers.image.version=9.1.1
# Tue, 18 Apr 2023 05:36:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 18 Apr 2023 05:36:10 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Tue, 18 Apr 2023 05:36:11 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 18 Apr 2023 05:36:11 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Tue, 18 Apr 2023 05:36:12 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Tue, 18 Apr 2023 05:36:20 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Tue, 18 Apr 2023 05:36:20 GMT
VOLUME [/var/solr]
# Tue, 18 Apr 2023 05:36:20 GMT
EXPOSE 8983
# Tue, 18 Apr 2023 05:36:20 GMT
WORKDIR /opt/solr
# Tue, 18 Apr 2023 05:36:20 GMT
USER 8983
# Tue, 18 Apr 2023 05:36:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 05:36:20 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b493027a1bf3e6a19b932ebe3c6dbfe19dc6a4583dfe39282977a57c89b31e87`  
		Last Modified: Tue, 18 Apr 2023 00:47:39 GMT  
		Size: 20.1 MB (20096839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02938177297ab7e29f7435f1f8092e05942dc412fbdfa6c1421589d8ef0adb57`  
		Last Modified: Tue, 18 Apr 2023 00:48:08 GMT  
		Size: 46.9 MB (46937043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e9595e3a57ad3c2eaf905104408a625b61809733c58a795c86405e275aea0b`  
		Last Modified: Tue, 18 Apr 2023 00:48:02 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ee77bff8d90cf9a351e1ce423014f4ff0f658293ca052a701886ea666d5fcc`  
		Last Modified: Tue, 18 Apr 2023 05:39:49 GMT  
		Size: 233.7 MB (233740953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5123a34ee6fa079f353e4bc304854acc6ffe3ba9cd2a5bfa47a7d4fda94b88be`  
		Last Modified: Tue, 18 Apr 2023 05:39:38 GMT  
		Size: 4.3 KB (4297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6dfda3f43afacbf8f2eb91877ce1c0f090c255c372e5a4f2022c017dad3ccfd`  
		Last Modified: Tue, 18 Apr 2023 05:39:39 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67d1f2ce2a1c23a9482d1aacca94ff05f266b538c1dd86725e930e309ad625f`  
		Last Modified: Tue, 18 Apr 2023 05:39:38 GMT  
		Size: 8.1 KB (8085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a342ac0282ccec59096fc2e74be5d78fde3c37f3ff8efe643a91945f37386448`  
		Last Modified: Tue, 18 Apr 2023 05:39:39 GMT  
		Size: 1.6 MB (1581649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.1.1` - linux; arm variant v7

```console
$ docker pull solr@sha256:95d88c5b740feb275a3fd34f161f040db9858bd68c00e04e2922a072d9eaac74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.3 MB (323261228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15750c0611f1a3f7679495e1515b8a02b4243c6c7aa147e31e9e42a53b332fcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:52:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:52:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:52:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:53:36 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:59:07 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:59:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:59:48 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:53:42 GMT
ARG SOLR_VERSION=9.1.1
# Wed, 26 Apr 2023 20:53:42 GMT
ARG SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f
# Wed, 26 Apr 2023 20:53:43 GMT
ARG SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763
# Wed, 26 Apr 2023 20:53:43 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:53:43 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:53:43 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz
# Wed, 26 Apr 2023 20:53:43 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Wed, 26 Apr 2023 20:53:43 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Wed, 26 Apr 2023 20:54:30 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Wed, 26 Apr 2023 20:54:31 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:54:31 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:54:31 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:54:32 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:54:32 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:54:32 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:54:32 GMT
LABEL org.opencontainers.image.version=9.1.1
# Wed, 26 Apr 2023 20:54:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:54:32 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:54:33 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:54:33 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:54:34 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:54:40 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:54:40 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:54:40 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:54:40 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:54:40 GMT
USER 8983
# Wed, 26 Apr 2023 20:54:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:54:40 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:e68c91cb250f35160f683afa80c3ada46f06948ded46a188be490ea3afff08f5`  
		Last Modified: Fri, 14 Apr 2023 09:34:28 GMT  
		Size: 24.6 MB (24586976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85796ae94aa6103041abcc6b06ff12a50d94cadaf6e06eb70a7394c3872a6748`  
		Last Modified: Tue, 18 Apr 2023 01:55:40 GMT  
		Size: 19.5 MB (19465888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddecf044ea404868fe676602278605918cf777a58be10ee59c72a7f7b91d23ea`  
		Last Modified: Wed, 26 Apr 2023 20:02:48 GMT  
		Size: 44.6 MB (44580407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d3b70b93915547c3833fab1fff6c2b5ca5742e7b1d1dda6489dc5aee45c0e9`  
		Last Modified: Wed, 26 Apr 2023 20:02:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e0a3739738b1505d2aa2e77b87f629e7b60ad701cbe80dfeca317de57ea27b`  
		Last Modified: Wed, 26 Apr 2023 20:57:35 GMT  
		Size: 233.2 MB (233220667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a822791bff0f72d4ae55bf4863aebb21a0903a92d9df44e69972202f435a56`  
		Last Modified: Wed, 26 Apr 2023 20:57:23 GMT  
		Size: 4.2 KB (4225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b37a1a5d357ea560dbd09c16429d4253032b5c1eea735ffb080ea774f8c43b`  
		Last Modified: Wed, 26 Apr 2023 20:57:23 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b88d27b99e2f54899bfdc8d7e339bed20cd3781daa0cda9780ce359ba57e069`  
		Last Modified: Wed, 26 Apr 2023 20:57:23 GMT  
		Size: 8.1 KB (8079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55df05b2f152434bc011cee3cc7f7de0efe6d4181cc53b4df82f088e92eed047`  
		Last Modified: Wed, 26 Apr 2023 20:57:23 GMT  
		Size: 1.4 MB (1394606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.1.1` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:756183ae377d29f4285ffc3ecae5dfbbb5a3ababadb28b12166dd36ddf186549
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.6 MB (329621218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04a7971549dffa1c9364de4726369f6ebf901d6487248614fe8098b27873a4ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:40:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:40:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:40:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:42:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:42:18 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Tue, 18 Apr 2023 01:42:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 01:42:41 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 03:19:28 GMT
ARG SOLR_VERSION=9.1.1
# Tue, 18 Apr 2023 03:19:28 GMT
ARG SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f
# Tue, 18 Apr 2023 03:19:28 GMT
ARG SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763
# Tue, 18 Apr 2023 03:19:28 GMT
ARG SOLR_DOWNLOAD_URL
# Tue, 18 Apr 2023 03:19:28 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 18 Apr 2023 03:19:28 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz
# Tue, 18 Apr 2023 03:19:29 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Tue, 18 Apr 2023 03:19:29 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Tue, 18 Apr 2023 03:20:08 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Tue, 18 Apr 2023 03:20:10 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Tue, 18 Apr 2023 03:20:10 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Tue, 18 Apr 2023 03:20:10 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Tue, 18 Apr 2023 03:20:10 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Tue, 18 Apr 2023 03:20:10 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Tue, 18 Apr 2023 03:20:10 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Tue, 18 Apr 2023 03:20:10 GMT
LABEL org.opencontainers.image.version=9.1.1
# Tue, 18 Apr 2023 03:20:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 18 Apr 2023 03:20:10 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Tue, 18 Apr 2023 03:20:11 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 18 Apr 2023 03:20:11 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Tue, 18 Apr 2023 03:20:12 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Tue, 18 Apr 2023 03:20:19 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Tue, 18 Apr 2023 03:20:19 GMT
VOLUME [/var/solr]
# Tue, 18 Apr 2023 03:20:19 GMT
EXPOSE 8983
# Tue, 18 Apr 2023 03:20:20 GMT
WORKDIR /opt/solr
# Tue, 18 Apr 2023 03:20:20 GMT
USER 8983
# Tue, 18 Apr 2023 03:20:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 03:20:20 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f855dc454f40dbe47d375c509772787d9d27ff505e14349af4f2e3944f28f75`  
		Last Modified: Tue, 18 Apr 2023 01:44:38 GMT  
		Size: 20.8 MB (20815202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c91968e85b36d056d961163f2b9155edf8119f19516132648c5ecae886bcb3`  
		Last Modified: Tue, 18 Apr 2023 01:45:04 GMT  
		Size: 46.4 MB (46422365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6e32ee26ed47aaac9a5a70c0af73a59858c966aa6646cc3b0151c938bf39b1`  
		Last Modified: Tue, 18 Apr 2023 01:44:58 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89355900f95b0a212d969f16b350857c1f2c484164a03a38942d9852b91faa46`  
		Last Modified: Tue, 18 Apr 2023 03:22:40 GMT  
		Size: 233.7 MB (233731364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5d238c8959564a4b0cdc672895e60492cdc82ad83c5d830b141bd5ff5fec7b`  
		Last Modified: Tue, 18 Apr 2023 03:22:31 GMT  
		Size: 4.3 KB (4330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797cde12c943c3478e869d8f23de31c7a29b17971f1b3a7162c2bb3ea213ecc5`  
		Last Modified: Tue, 18 Apr 2023 03:22:31 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5c3e86e33823bf7401a4a0e404d76113f801a1114b2c24a1d9b3e50af3fdcb`  
		Last Modified: Tue, 18 Apr 2023 03:22:31 GMT  
		Size: 8.1 KB (8085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e485d8d417dab6f7edacf648b1b41ec329e3a9cc83e99f106c73681d92dc29`  
		Last Modified: Tue, 18 Apr 2023 03:22:31 GMT  
		Size: 1.4 MB (1443095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.1.1` - linux; ppc64le

```console
$ docker pull solr@sha256:11c911a63efb87b6dc21c2f20cd7c62ef06c104a0fb4c2367586d2b88ca0f798
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.5 MB (338457239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae26641d93398dfb86ac8cca67ddf6b8feb85383ab79a642536fd8e365a5aa1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:06:30 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:06:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:06:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:09:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:22:51 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:25:49 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:25:52 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:39:23 GMT
ARG SOLR_VERSION=9.1.1
# Wed, 26 Apr 2023 20:39:24 GMT
ARG SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f
# Wed, 26 Apr 2023 20:39:24 GMT
ARG SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763
# Wed, 26 Apr 2023 20:39:24 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:39:25 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:39:25 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz
# Wed, 26 Apr 2023 20:39:25 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Wed, 26 Apr 2023 20:39:25 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz
# Wed, 26 Apr 2023 20:40:10 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Wed, 26 Apr 2023 20:40:13 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:40:13 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:40:14 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:40:14 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:40:14 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:40:14 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:40:15 GMT
LABEL org.opencontainers.image.version=9.1.1
# Wed, 26 Apr 2023 20:40:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:40:15 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:40:17 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:40:18 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:40:19 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:40:30 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.1.1/solr-9.1.1.tgz SOLR_KEYS=C3E7CBD9B9FE2B419EB14B89612B39A5BC981763 SOLR_SHA512=59fd47185196fc6b0fad4b6b2ba547d136cc0c688addc9833129086944cc90e185a18c33fd70523edddad1a6ebe7b4cd893be5065c2b01fe21a5026bdb7e5d9f SOLR_VERSION=9.1.1
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:40:30 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:40:31 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:40:31 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:40:31 GMT
USER 8983
# Wed, 26 Apr 2023 20:40:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:40:32 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:d276072145993a42aed3e2b3e8cd26b6e08aab266d9c9d792ee89b26150681da`  
		Last Modified: Fri, 14 Apr 2023 09:36:00 GMT  
		Size: 33.3 MB (33300980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d16c8f7fe3c69e12b82f6ead20825685acccc07c7db20352690c45095874956`  
		Last Modified: Tue, 18 Apr 2023 01:13:05 GMT  
		Size: 22.1 MB (22066207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6193924dcc6a0c16fcd313f0de2f47c224244a3b32a2e66ac95fb8caf4acb0a3`  
		Last Modified: Wed, 26 Apr 2023 19:36:46 GMT  
		Size: 46.9 MB (46872363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d65ded274243674ad49fb2ed7f15e5ae634747fb0c35f80c742fa2cc980aebe`  
		Last Modified: Wed, 26 Apr 2023 19:36:34 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93592fc93b9338f8fdc5a1463c21641cefb5b1d63e3e309fa94a5a013f3ad8f4`  
		Last Modified: Wed, 26 Apr 2023 20:44:31 GMT  
		Size: 234.6 MB (234600951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6bbb832f2610c512b29780ce62e45f1341ad6151a253fa3a7711e605adf60d`  
		Last Modified: Wed, 26 Apr 2023 20:44:12 GMT  
		Size: 4.3 KB (4295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da97cb7ca72b20e1d78b44290c3f42a074df1edf3b5c802b97d92d2627a6c89`  
		Last Modified: Wed, 26 Apr 2023 20:44:12 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848754de971b0ca8cefed25f67295c073d49528aa6e5776c350152c6f7b31f35`  
		Last Modified: Wed, 26 Apr 2023 20:44:12 GMT  
		Size: 8.1 KB (8084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30f79abbb0d6962fee4ec92cd0b9729c0d59b84c4a0d03bd2ff74897fc0fa66`  
		Last Modified: Wed, 26 Apr 2023 20:44:13 GMT  
		Size: 1.6 MB (1603980 bytes)  
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
$ docker pull solr@sha256:6607abbaa3fb4314f8aafbc9f427ae13561bc0c5a8ec4290cf0e2b2e9cf5d55b
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
$ docker pull solr@sha256:cbee52e4b6a1e30d450e8ca19402c3bc15d4d8e8a75ca8501cb0f7f642cc76ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.9 MB (374859971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7d43c32e8ee6e715af99f55ba48e134125af6eadbc175932523f25a1070ce4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:44:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 02:44:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 02:44:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 02:46:48 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:46:48 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Thu, 16 Mar 2023 02:47:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 16 Mar 2023 02:47:22 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_VERSION=9.2.0
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:20:07 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:20:52 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.version=9.2.0
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 24 Mar 2023 20:20:53 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 24 Mar 2023 20:20:54 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 24 Mar 2023 20:20:55 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 24 Mar 2023 20:20:55 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 24 Mar 2023 20:21:03 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 24 Mar 2023 20:21:03 GMT
VOLUME [/var/solr]
# Fri, 24 Mar 2023 20:21:03 GMT
EXPOSE 8983
# Fri, 24 Mar 2023 20:21:03 GMT
WORKDIR /opt/solr
# Fri, 24 Mar 2023 20:21:04 GMT
USER 8983
# Fri, 24 Mar 2023 20:21:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Mar 2023 20:21:04 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a182a611d05b01879f065473c49fb968b8d30312f931350ea07af1c46aa8b4f9`  
		Last Modified: Thu, 16 Mar 2023 02:53:08 GMT  
		Size: 17.0 MB (16975402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb51f9f63778bb9fb97f2cb054b54dfc5098aba2931664a12930c35cf464ca6`  
		Last Modified: Thu, 16 Mar 2023 02:54:00 GMT  
		Size: 46.9 MB (46935467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1365afd8cae0153f1c2bfcf8a4c9b78f2e6e0f18431b0460c63c1fede7507fee`  
		Last Modified: Thu, 16 Mar 2023 02:53:53 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b70190cd6e82c4ac613c9f0f9bf4e42155528b445617672bcd7a211b2a2104`  
		Last Modified: Fri, 24 Mar 2023 20:21:43 GMT  
		Size: 278.7 MB (278678830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c984f04f09ad32d618a63f426eb4127534ca414910aa8b56da2355a3bcf17c17`  
		Last Modified: Fri, 24 Mar 2023 20:21:31 GMT  
		Size: 4.3 KB (4295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888b9068f218433d417da0cd83cca3863ad2cbea9bab37c09fc52a63fab6206e`  
		Last Modified: Fri, 24 Mar 2023 20:21:31 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1599d0444630b3ac11f8d61742ff79acaaec1b9cfcca5e176b131ef54c22bd`  
		Last Modified: Fri, 24 Mar 2023 20:21:32 GMT  
		Size: 8.3 KB (8264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cbc52fa8b34cbd17b27c7c562e83344a928724a395e74a740d6bcfbd0aca1e8`  
		Last Modified: Fri, 24 Mar 2023 20:21:32 GMT  
		Size: 1.8 MB (1827370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.2` - linux; arm variant v7

```console
$ docker pull solr@sha256:8544ae0dc85e554f5d5267937f74c720c90b07f1cf05ffc3201f4eb9095b42dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **369.0 MB (369045467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73e472402be480932e64f4a05bda9a60df8996c5852b59ceb376c284295bafa8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:31:41 GMT
ADD file:e9c3ac290fb81ae2e78de99052d776396ee3aff05e1a66fd2dccb01d7de9bb45 in / 
# Wed, 08 Mar 2023 04:31:42 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:46:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 02:46:15 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 02:46:15 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 02:49:36 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:59:26 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:59:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:59:55 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:52:45 GMT
ARG SOLR_VERSION=9.2.0
# Wed, 26 Apr 2023 20:52:45 GMT
ARG SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665
# Wed, 26 Apr 2023 20:52:45 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Wed, 26 Apr 2023 20:52:45 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:52:46 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:52:46 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:52:46 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:52:46 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:53:18 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.version=9.2.0
# Wed, 26 Apr 2023 20:53:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:53:21 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:53:21 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:53:22 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:53:22 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:53:32 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:53:32 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:53:32 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:53:32 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:53:32 GMT
USER 8983
# Wed, 26 Apr 2023 20:53:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:53:33 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:cba1fa3bcdf4f746dcf5b8f86874cee4a6eff75dd5c5cd29e4c912574b12a1c6`  
		Last Modified: Thu, 09 Mar 2023 04:41:14 GMT  
		Size: 27.0 MB (27025397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85169cff2ee4bc04fcfaf94a937435e69eb27ca38bf1dcbd04593cccacf0d702`  
		Last Modified: Thu, 16 Mar 2023 02:56:32 GMT  
		Size: 17.1 MB (17093778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de292b783be3523048fe05ba87f22c3948fb2a4468235c054ea6a35a4f7a053`  
		Last Modified: Wed, 26 Apr 2023 20:03:03 GMT  
		Size: 44.6 MB (44579974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05ce4c34b22f40a9acec67a1a46b86a1435158c0dc9bd6e001f1bf7d77326a5`  
		Last Modified: Wed, 26 Apr 2023 20:02:56 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7651a81ea9e32ab5c6154450135c9f73f51999c9aaa7b801c5f62089fe7acb50`  
		Last Modified: Wed, 26 Apr 2023 20:57:10 GMT  
		Size: 278.7 MB (278680039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bbc9eb9d4ef7ab913012093550bd6110ea6f7556b355caddf44f4b7a8a145fa`  
		Last Modified: Wed, 26 Apr 2023 20:56:56 GMT  
		Size: 4.2 KB (4226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cf324cc98872102c6e9fbf9d55d4a0ab567ca7652ca01e8cc4ffc4e33366b6`  
		Last Modified: Wed, 26 Apr 2023 20:56:56 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddea7d711377bed446cb0468d2e74276ea12f53af7dd1f6975b66c6911baf6b`  
		Last Modified: Wed, 26 Apr 2023 20:56:56 GMT  
		Size: 8.3 KB (8261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac376cfc47e23bc8413e65021ee472c27047ebd1ad83f73d4053e0a55edcd477`  
		Last Modified: Wed, 26 Apr 2023 20:56:56 GMT  
		Size: 1.7 MB (1653413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.2` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:58619b9500a6637702a27985f2cf8b17cb13dae6c2673f3abaa9a1bd824277ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **373.6 MB (373587696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25f72e1df4e02c02f553d7d54dd64951829dbdd59095775a6634ddce70eadc8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:52:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 01:52:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 01:52:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 01:55:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:55:04 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Thu, 16 Mar 2023 01:55:29 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 16 Mar 2023 01:55:30 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_VERSION=9.2.0
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:47:31 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:47:31 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:48:14 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 24 Mar 2023 20:48:17 GMT
LABEL org.opencontainers.image.version=9.2.0
# Fri, 24 Mar 2023 20:48:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 24 Mar 2023 20:48:17 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 24 Mar 2023 20:48:17 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 24 Mar 2023 20:48:18 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 24 Mar 2023 20:48:18 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 24 Mar 2023 20:48:27 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 24 Mar 2023 20:48:27 GMT
VOLUME [/var/solr]
# Fri, 24 Mar 2023 20:48:27 GMT
EXPOSE 8983
# Fri, 24 Mar 2023 20:48:27 GMT
WORKDIR /opt/solr
# Fri, 24 Mar 2023 20:48:28 GMT
USER 8983
# Fri, 24 Mar 2023 20:48:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Mar 2023 20:48:28 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40b70fd7935308ad0e072e7e06ec8c3abdc59beae70ca716dcd04e971680865`  
		Last Modified: Thu, 16 Mar 2023 02:00:42 GMT  
		Size: 18.4 MB (18400790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33dd5efa5ce73b25dc0236fcd408527b63e42c87e6da9672a356731004b8949`  
		Last Modified: Thu, 16 Mar 2023 02:01:25 GMT  
		Size: 46.4 MB (46421360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ce9280353ea6c4511dc5378e2f0f4742d499bf6df15c8d10804513c8c5115a`  
		Last Modified: Thu, 16 Mar 2023 02:01:20 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85ed965ce21582560c60a815ae59ae9cf0fcb5c9270ba02dfc5ca1c135b44f`  
		Last Modified: Fri, 24 Mar 2023 20:49:04 GMT  
		Size: 278.7 MB (278678702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a47faea25001b6a9178cab60304409e81d636878232dda7e76d519e7490bbc9`  
		Last Modified: Fri, 24 Mar 2023 20:48:54 GMT  
		Size: 4.3 KB (4331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7792e9b554723df7cdd9593ee715d8fe16cfec71a28c58e0b01e2534e7f2c8`  
		Last Modified: Fri, 24 Mar 2023 20:48:54 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9435de9f76e1e09e2078c456e20cd6a83a757671ecc43398fed205b323cb3c6b`  
		Last Modified: Fri, 24 Mar 2023 20:48:54 GMT  
		Size: 8.3 KB (8261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fc7a7f4116bfd1b88180e25c33fa7c4d571df7caad6ffebbec7786b32b2738`  
		Last Modified: Fri, 24 Mar 2023 20:48:54 GMT  
		Size: 1.7 MB (1686320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.2` - linux; ppc64le

```console
$ docker pull solr@sha256:f390f3d9f15f1aa1bbad8f1f2e7d13c3cc0599c722e9b9751d40ee71aa084561
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.4 MB (381368174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c8aecc2dc5554acdda867249e249f23bafb21f089ae5b92d1530289c7651a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:16 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:20 GMT
ADD file:d7434a52d8d8aa6288e788f6fe7e156f0e11bf9b8275efaf70aab0bfc4d919cf in / 
# Wed, 08 Mar 2023 04:39:20 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:57:34 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 03:57:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 03:57:35 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 04:03:27 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:23:33 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:26:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:26:14 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:36:53 GMT
ARG SOLR_VERSION=9.2.0
# Wed, 26 Apr 2023 20:36:54 GMT
ARG SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665
# Wed, 26 Apr 2023 20:36:54 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Wed, 26 Apr 2023 20:36:54 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:36:54 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:36:55 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:36:55 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:36:55 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:38:40 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Wed, 26 Apr 2023 20:38:44 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:38:44 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:38:44 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:38:44 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:38:45 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:38:45 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:38:45 GMT
LABEL org.opencontainers.image.version=9.2.0
# Wed, 26 Apr 2023 20:38:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:38:46 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:38:47 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:38:48 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:38:49 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:39:04 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:39:05 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:39:05 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:39:05 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:39:05 GMT
USER 8983
# Wed, 26 Apr 2023 20:39:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:39:06 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:deffc758660db3b0ee7a1f211d720633f06f27ab1e4c31db4caf8c27f4a80eeb`  
		Last Modified: Thu, 16 Mar 2023 02:22:27 GMT  
		Size: 35.7 MB (35711728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c06c33e4689e5957d961321ac18da32bea369d2eccc9173c9ad8b517f802ea`  
		Last Modified: Thu, 16 Mar 2023 04:14:09 GMT  
		Size: 18.3 MB (18257665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25abdd535a180a29cc8edf36ac17eb237551826124456d77040e4d464bceb120`  
		Last Modified: Wed, 26 Apr 2023 19:37:08 GMT  
		Size: 46.9 MB (46872523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9532e0e54e3616e367a6095c24ff50105415ae0333e1fabc59c04be22f053e`  
		Last Modified: Wed, 26 Apr 2023 19:36:55 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182d7fc15b9c08e18cdc6cdf0160b68aa45d1b34992b787cdd7f49c9e030e2c9`  
		Last Modified: Wed, 26 Apr 2023 20:43:58 GMT  
		Size: 278.7 MB (278679581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585651ad84270f628cfb14608c4dbb4e3a7a7d865d31747e5aa6084bd109a1c0`  
		Last Modified: Wed, 26 Apr 2023 20:43:36 GMT  
		Size: 4.3 KB (4298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ed3ec073534fcdcfe0bb91a989a24838b5fae6c4a74b6a898b2dc3694b5407`  
		Last Modified: Wed, 26 Apr 2023 20:43:36 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450540c1db3e7e00d5d9ef4f2fc497c849bf895bc1c6478b3017070f8938b7ee`  
		Last Modified: Wed, 26 Apr 2023 20:43:36 GMT  
		Size: 8.3 KB (8255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9738eccb09731f4eae5b20b3bec3d18ba11a98334974ff4f652999eabd29c1`  
		Last Modified: Wed, 26 Apr 2023 20:43:37 GMT  
		Size: 1.8 MB (1833743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.2` - linux; s390x

```console
$ docker pull solr@sha256:3bf7b256991de31d033da2ffbf31cb9b6d95ef615a6b9792a34577903efd2612
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **369.6 MB (369641824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33ecafe05af5a8d70f6d65e63cea1441abacad2ed33f011d1fd02de369e339bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:26 GMT
ADD file:630f9865d3d4fd4294d45cac7cbaea83fb549c2e563de454348da964d19fbbba in / 
# Wed, 08 Mar 2023 04:39:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:06:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 02:06:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 02:06:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 02:07:58 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:43:50 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:44:49 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:44:51 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:34:03 GMT
ARG SOLR_VERSION=9.2.0
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:34:40 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.version=9.2.0
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:34:45 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:34:46 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:34:46 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:34:47 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:34:51 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:34:51 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:34:51 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:34:52 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:34:52 GMT
USER 8983
# Wed, 26 Apr 2023 20:34:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:34:52 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:2c7366af510b72cc0b3456fb93cfa0bfc76f7d383db5cb315967e7b1ce2e0c42`  
		Last Modified: Thu, 16 Mar 2023 02:02:40 GMT  
		Size: 28.6 MB (28647599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d28ae42a862e9773a02317b5a0eeb71ddfe3a887bb001c8f23a2786c926287`  
		Last Modified: Thu, 16 Mar 2023 02:13:35 GMT  
		Size: 16.8 MB (16753284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed61af6a2c87d412802d8f160fb683fc3ec859e336bfe78f93cdcc31e81a5d1a`  
		Last Modified: Wed, 26 Apr 2023 19:48:14 GMT  
		Size: 43.8 MB (43774584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1494ca84bd62528d8f5f078978408f8e5d411da7a46a6065b53e647d1149f5e6`  
		Last Modified: Wed, 26 Apr 2023 19:48:08 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10d1906d4f5008ad00b585c01cb6bdfc068441c94a1d90e8d5945b3b3ddcce6`  
		Last Modified: Wed, 26 Apr 2023 20:37:47 GMT  
		Size: 278.7 MB (278679157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135adf4cb67937fdd1cdf49ca0951324c2a557081953bdf42ed6010b5aadad12`  
		Last Modified: Wed, 26 Apr 2023 20:37:35 GMT  
		Size: 4.3 KB (4329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1770bb3c6b573d4b988aa5479ae3f73c2af9183c16554ec894a2dcb2394a50e`  
		Last Modified: Wed, 26 Apr 2023 20:37:36 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7508a18ea82d8ebe5d57e272b8378f77364d1c20247feab03855086fe8a39fd`  
		Last Modified: Wed, 26 Apr 2023 20:37:36 GMT  
		Size: 8.3 KB (8260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6560f9ee79577800018ac8eba33b185d6cdae6b516d8bb88d5d469a7ddcc2e3a`  
		Last Modified: Wed, 26 Apr 2023 20:37:36 GMT  
		Size: 1.8 MB (1774233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:9.2.0`

```console
$ docker pull solr@sha256:6607abbaa3fb4314f8aafbc9f427ae13561bc0c5a8ec4290cf0e2b2e9cf5d55b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `solr:9.2.0` - linux; amd64

```console
$ docker pull solr@sha256:cbee52e4b6a1e30d450e8ca19402c3bc15d4d8e8a75ca8501cb0f7f642cc76ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.9 MB (374859971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7d43c32e8ee6e715af99f55ba48e134125af6eadbc175932523f25a1070ce4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:44:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 02:44:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 02:44:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 02:46:48 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:46:48 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Thu, 16 Mar 2023 02:47:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 16 Mar 2023 02:47:22 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_VERSION=9.2.0
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:20:07 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:20:52 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.version=9.2.0
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 24 Mar 2023 20:20:53 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 24 Mar 2023 20:20:54 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 24 Mar 2023 20:20:55 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 24 Mar 2023 20:20:55 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 24 Mar 2023 20:21:03 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 24 Mar 2023 20:21:03 GMT
VOLUME [/var/solr]
# Fri, 24 Mar 2023 20:21:03 GMT
EXPOSE 8983
# Fri, 24 Mar 2023 20:21:03 GMT
WORKDIR /opt/solr
# Fri, 24 Mar 2023 20:21:04 GMT
USER 8983
# Fri, 24 Mar 2023 20:21:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Mar 2023 20:21:04 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a182a611d05b01879f065473c49fb968b8d30312f931350ea07af1c46aa8b4f9`  
		Last Modified: Thu, 16 Mar 2023 02:53:08 GMT  
		Size: 17.0 MB (16975402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb51f9f63778bb9fb97f2cb054b54dfc5098aba2931664a12930c35cf464ca6`  
		Last Modified: Thu, 16 Mar 2023 02:54:00 GMT  
		Size: 46.9 MB (46935467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1365afd8cae0153f1c2bfcf8a4c9b78f2e6e0f18431b0460c63c1fede7507fee`  
		Last Modified: Thu, 16 Mar 2023 02:53:53 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b70190cd6e82c4ac613c9f0f9bf4e42155528b445617672bcd7a211b2a2104`  
		Last Modified: Fri, 24 Mar 2023 20:21:43 GMT  
		Size: 278.7 MB (278678830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c984f04f09ad32d618a63f426eb4127534ca414910aa8b56da2355a3bcf17c17`  
		Last Modified: Fri, 24 Mar 2023 20:21:31 GMT  
		Size: 4.3 KB (4295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888b9068f218433d417da0cd83cca3863ad2cbea9bab37c09fc52a63fab6206e`  
		Last Modified: Fri, 24 Mar 2023 20:21:31 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1599d0444630b3ac11f8d61742ff79acaaec1b9cfcca5e176b131ef54c22bd`  
		Last Modified: Fri, 24 Mar 2023 20:21:32 GMT  
		Size: 8.3 KB (8264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cbc52fa8b34cbd17b27c7c562e83344a928724a395e74a740d6bcfbd0aca1e8`  
		Last Modified: Fri, 24 Mar 2023 20:21:32 GMT  
		Size: 1.8 MB (1827370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.2.0` - linux; arm variant v7

```console
$ docker pull solr@sha256:8544ae0dc85e554f5d5267937f74c720c90b07f1cf05ffc3201f4eb9095b42dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **369.0 MB (369045467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73e472402be480932e64f4a05bda9a60df8996c5852b59ceb376c284295bafa8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:31:41 GMT
ADD file:e9c3ac290fb81ae2e78de99052d776396ee3aff05e1a66fd2dccb01d7de9bb45 in / 
# Wed, 08 Mar 2023 04:31:42 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:46:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 02:46:15 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 02:46:15 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 02:49:36 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:59:26 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:59:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:59:55 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:52:45 GMT
ARG SOLR_VERSION=9.2.0
# Wed, 26 Apr 2023 20:52:45 GMT
ARG SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665
# Wed, 26 Apr 2023 20:52:45 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Wed, 26 Apr 2023 20:52:45 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:52:46 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:52:46 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:52:46 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:52:46 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:53:18 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.version=9.2.0
# Wed, 26 Apr 2023 20:53:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:53:21 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:53:21 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:53:22 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:53:22 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:53:32 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:53:32 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:53:32 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:53:32 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:53:32 GMT
USER 8983
# Wed, 26 Apr 2023 20:53:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:53:33 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:cba1fa3bcdf4f746dcf5b8f86874cee4a6eff75dd5c5cd29e4c912574b12a1c6`  
		Last Modified: Thu, 09 Mar 2023 04:41:14 GMT  
		Size: 27.0 MB (27025397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85169cff2ee4bc04fcfaf94a937435e69eb27ca38bf1dcbd04593cccacf0d702`  
		Last Modified: Thu, 16 Mar 2023 02:56:32 GMT  
		Size: 17.1 MB (17093778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de292b783be3523048fe05ba87f22c3948fb2a4468235c054ea6a35a4f7a053`  
		Last Modified: Wed, 26 Apr 2023 20:03:03 GMT  
		Size: 44.6 MB (44579974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05ce4c34b22f40a9acec67a1a46b86a1435158c0dc9bd6e001f1bf7d77326a5`  
		Last Modified: Wed, 26 Apr 2023 20:02:56 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7651a81ea9e32ab5c6154450135c9f73f51999c9aaa7b801c5f62089fe7acb50`  
		Last Modified: Wed, 26 Apr 2023 20:57:10 GMT  
		Size: 278.7 MB (278680039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bbc9eb9d4ef7ab913012093550bd6110ea6f7556b355caddf44f4b7a8a145fa`  
		Last Modified: Wed, 26 Apr 2023 20:56:56 GMT  
		Size: 4.2 KB (4226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cf324cc98872102c6e9fbf9d55d4a0ab567ca7652ca01e8cc4ffc4e33366b6`  
		Last Modified: Wed, 26 Apr 2023 20:56:56 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddea7d711377bed446cb0468d2e74276ea12f53af7dd1f6975b66c6911baf6b`  
		Last Modified: Wed, 26 Apr 2023 20:56:56 GMT  
		Size: 8.3 KB (8261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac376cfc47e23bc8413e65021ee472c27047ebd1ad83f73d4053e0a55edcd477`  
		Last Modified: Wed, 26 Apr 2023 20:56:56 GMT  
		Size: 1.7 MB (1653413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.2.0` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:58619b9500a6637702a27985f2cf8b17cb13dae6c2673f3abaa9a1bd824277ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **373.6 MB (373587696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25f72e1df4e02c02f553d7d54dd64951829dbdd59095775a6634ddce70eadc8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:52:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 01:52:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 01:52:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 01:55:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:55:04 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Thu, 16 Mar 2023 01:55:29 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 16 Mar 2023 01:55:30 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_VERSION=9.2.0
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:47:31 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:47:31 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:48:14 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 24 Mar 2023 20:48:17 GMT
LABEL org.opencontainers.image.version=9.2.0
# Fri, 24 Mar 2023 20:48:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 24 Mar 2023 20:48:17 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 24 Mar 2023 20:48:17 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 24 Mar 2023 20:48:18 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 24 Mar 2023 20:48:18 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 24 Mar 2023 20:48:27 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 24 Mar 2023 20:48:27 GMT
VOLUME [/var/solr]
# Fri, 24 Mar 2023 20:48:27 GMT
EXPOSE 8983
# Fri, 24 Mar 2023 20:48:27 GMT
WORKDIR /opt/solr
# Fri, 24 Mar 2023 20:48:28 GMT
USER 8983
# Fri, 24 Mar 2023 20:48:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Mar 2023 20:48:28 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40b70fd7935308ad0e072e7e06ec8c3abdc59beae70ca716dcd04e971680865`  
		Last Modified: Thu, 16 Mar 2023 02:00:42 GMT  
		Size: 18.4 MB (18400790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33dd5efa5ce73b25dc0236fcd408527b63e42c87e6da9672a356731004b8949`  
		Last Modified: Thu, 16 Mar 2023 02:01:25 GMT  
		Size: 46.4 MB (46421360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ce9280353ea6c4511dc5378e2f0f4742d499bf6df15c8d10804513c8c5115a`  
		Last Modified: Thu, 16 Mar 2023 02:01:20 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85ed965ce21582560c60a815ae59ae9cf0fcb5c9270ba02dfc5ca1c135b44f`  
		Last Modified: Fri, 24 Mar 2023 20:49:04 GMT  
		Size: 278.7 MB (278678702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a47faea25001b6a9178cab60304409e81d636878232dda7e76d519e7490bbc9`  
		Last Modified: Fri, 24 Mar 2023 20:48:54 GMT  
		Size: 4.3 KB (4331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7792e9b554723df7cdd9593ee715d8fe16cfec71a28c58e0b01e2534e7f2c8`  
		Last Modified: Fri, 24 Mar 2023 20:48:54 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9435de9f76e1e09e2078c456e20cd6a83a757671ecc43398fed205b323cb3c6b`  
		Last Modified: Fri, 24 Mar 2023 20:48:54 GMT  
		Size: 8.3 KB (8261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fc7a7f4116bfd1b88180e25c33fa7c4d571df7caad6ffebbec7786b32b2738`  
		Last Modified: Fri, 24 Mar 2023 20:48:54 GMT  
		Size: 1.7 MB (1686320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.2.0` - linux; ppc64le

```console
$ docker pull solr@sha256:f390f3d9f15f1aa1bbad8f1f2e7d13c3cc0599c722e9b9751d40ee71aa084561
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.4 MB (381368174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c8aecc2dc5554acdda867249e249f23bafb21f089ae5b92d1530289c7651a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:16 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:20 GMT
ADD file:d7434a52d8d8aa6288e788f6fe7e156f0e11bf9b8275efaf70aab0bfc4d919cf in / 
# Wed, 08 Mar 2023 04:39:20 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:57:34 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 03:57:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 03:57:35 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 04:03:27 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:23:33 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:26:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:26:14 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:36:53 GMT
ARG SOLR_VERSION=9.2.0
# Wed, 26 Apr 2023 20:36:54 GMT
ARG SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665
# Wed, 26 Apr 2023 20:36:54 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Wed, 26 Apr 2023 20:36:54 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:36:54 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:36:55 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:36:55 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:36:55 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:38:40 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Wed, 26 Apr 2023 20:38:44 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:38:44 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:38:44 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:38:44 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:38:45 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:38:45 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:38:45 GMT
LABEL org.opencontainers.image.version=9.2.0
# Wed, 26 Apr 2023 20:38:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:38:46 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:38:47 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:38:48 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:38:49 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:39:04 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:39:05 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:39:05 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:39:05 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:39:05 GMT
USER 8983
# Wed, 26 Apr 2023 20:39:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:39:06 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:deffc758660db3b0ee7a1f211d720633f06f27ab1e4c31db4caf8c27f4a80eeb`  
		Last Modified: Thu, 16 Mar 2023 02:22:27 GMT  
		Size: 35.7 MB (35711728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c06c33e4689e5957d961321ac18da32bea369d2eccc9173c9ad8b517f802ea`  
		Last Modified: Thu, 16 Mar 2023 04:14:09 GMT  
		Size: 18.3 MB (18257665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25abdd535a180a29cc8edf36ac17eb237551826124456d77040e4d464bceb120`  
		Last Modified: Wed, 26 Apr 2023 19:37:08 GMT  
		Size: 46.9 MB (46872523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9532e0e54e3616e367a6095c24ff50105415ae0333e1fabc59c04be22f053e`  
		Last Modified: Wed, 26 Apr 2023 19:36:55 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182d7fc15b9c08e18cdc6cdf0160b68aa45d1b34992b787cdd7f49c9e030e2c9`  
		Last Modified: Wed, 26 Apr 2023 20:43:58 GMT  
		Size: 278.7 MB (278679581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585651ad84270f628cfb14608c4dbb4e3a7a7d865d31747e5aa6084bd109a1c0`  
		Last Modified: Wed, 26 Apr 2023 20:43:36 GMT  
		Size: 4.3 KB (4298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ed3ec073534fcdcfe0bb91a989a24838b5fae6c4a74b6a898b2dc3694b5407`  
		Last Modified: Wed, 26 Apr 2023 20:43:36 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450540c1db3e7e00d5d9ef4f2fc497c849bf895bc1c6478b3017070f8938b7ee`  
		Last Modified: Wed, 26 Apr 2023 20:43:36 GMT  
		Size: 8.3 KB (8255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9738eccb09731f4eae5b20b3bec3d18ba11a98334974ff4f652999eabd29c1`  
		Last Modified: Wed, 26 Apr 2023 20:43:37 GMT  
		Size: 1.8 MB (1833743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.2.0` - linux; s390x

```console
$ docker pull solr@sha256:3bf7b256991de31d033da2ffbf31cb9b6d95ef615a6b9792a34577903efd2612
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **369.6 MB (369641824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33ecafe05af5a8d70f6d65e63cea1441abacad2ed33f011d1fd02de369e339bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:26 GMT
ADD file:630f9865d3d4fd4294d45cac7cbaea83fb549c2e563de454348da964d19fbbba in / 
# Wed, 08 Mar 2023 04:39:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:06:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 02:06:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 02:06:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 02:07:58 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:43:50 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:44:49 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:44:51 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:34:03 GMT
ARG SOLR_VERSION=9.2.0
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:34:40 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.version=9.2.0
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:34:45 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:34:46 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:34:46 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:34:47 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:34:51 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:34:51 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:34:51 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:34:52 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:34:52 GMT
USER 8983
# Wed, 26 Apr 2023 20:34:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:34:52 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:2c7366af510b72cc0b3456fb93cfa0bfc76f7d383db5cb315967e7b1ce2e0c42`  
		Last Modified: Thu, 16 Mar 2023 02:02:40 GMT  
		Size: 28.6 MB (28647599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d28ae42a862e9773a02317b5a0eeb71ddfe3a887bb001c8f23a2786c926287`  
		Last Modified: Thu, 16 Mar 2023 02:13:35 GMT  
		Size: 16.8 MB (16753284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed61af6a2c87d412802d8f160fb683fc3ec859e336bfe78f93cdcc31e81a5d1a`  
		Last Modified: Wed, 26 Apr 2023 19:48:14 GMT  
		Size: 43.8 MB (43774584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1494ca84bd62528d8f5f078978408f8e5d411da7a46a6065b53e647d1149f5e6`  
		Last Modified: Wed, 26 Apr 2023 19:48:08 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10d1906d4f5008ad00b585c01cb6bdfc068441c94a1d90e8d5945b3b3ddcce6`  
		Last Modified: Wed, 26 Apr 2023 20:37:47 GMT  
		Size: 278.7 MB (278679157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135adf4cb67937fdd1cdf49ca0951324c2a557081953bdf42ed6010b5aadad12`  
		Last Modified: Wed, 26 Apr 2023 20:37:35 GMT  
		Size: 4.3 KB (4329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1770bb3c6b573d4b988aa5479ae3f73c2af9183c16554ec894a2dcb2394a50e`  
		Last Modified: Wed, 26 Apr 2023 20:37:36 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7508a18ea82d8ebe5d57e272b8378f77364d1c20247feab03855086fe8a39fd`  
		Last Modified: Wed, 26 Apr 2023 20:37:36 GMT  
		Size: 8.3 KB (8260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6560f9ee79577800018ac8eba33b185d6cdae6b516d8bb88d5d469a7ddcc2e3a`  
		Last Modified: Wed, 26 Apr 2023 20:37:36 GMT  
		Size: 1.8 MB (1774233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:latest`

```console
$ docker pull solr@sha256:6607abbaa3fb4314f8aafbc9f427ae13561bc0c5a8ec4290cf0e2b2e9cf5d55b
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
$ docker pull solr@sha256:cbee52e4b6a1e30d450e8ca19402c3bc15d4d8e8a75ca8501cb0f7f642cc76ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.9 MB (374859971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7d43c32e8ee6e715af99f55ba48e134125af6eadbc175932523f25a1070ce4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:44:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 02:44:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 02:44:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 02:46:48 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:46:48 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Thu, 16 Mar 2023 02:47:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 16 Mar 2023 02:47:22 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_VERSION=9.2.0
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:20:06 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:20:07 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:20:52 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.version=9.2.0
# Fri, 24 Mar 2023 20:20:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 24 Mar 2023 20:20:53 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 24 Mar 2023 20:20:54 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 24 Mar 2023 20:20:55 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 24 Mar 2023 20:20:55 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 24 Mar 2023 20:21:03 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 24 Mar 2023 20:21:03 GMT
VOLUME [/var/solr]
# Fri, 24 Mar 2023 20:21:03 GMT
EXPOSE 8983
# Fri, 24 Mar 2023 20:21:03 GMT
WORKDIR /opt/solr
# Fri, 24 Mar 2023 20:21:04 GMT
USER 8983
# Fri, 24 Mar 2023 20:21:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Mar 2023 20:21:04 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a182a611d05b01879f065473c49fb968b8d30312f931350ea07af1c46aa8b4f9`  
		Last Modified: Thu, 16 Mar 2023 02:53:08 GMT  
		Size: 17.0 MB (16975402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb51f9f63778bb9fb97f2cb054b54dfc5098aba2931664a12930c35cf464ca6`  
		Last Modified: Thu, 16 Mar 2023 02:54:00 GMT  
		Size: 46.9 MB (46935467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1365afd8cae0153f1c2bfcf8a4c9b78f2e6e0f18431b0460c63c1fede7507fee`  
		Last Modified: Thu, 16 Mar 2023 02:53:53 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b70190cd6e82c4ac613c9f0f9bf4e42155528b445617672bcd7a211b2a2104`  
		Last Modified: Fri, 24 Mar 2023 20:21:43 GMT  
		Size: 278.7 MB (278678830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c984f04f09ad32d618a63f426eb4127534ca414910aa8b56da2355a3bcf17c17`  
		Last Modified: Fri, 24 Mar 2023 20:21:31 GMT  
		Size: 4.3 KB (4295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888b9068f218433d417da0cd83cca3863ad2cbea9bab37c09fc52a63fab6206e`  
		Last Modified: Fri, 24 Mar 2023 20:21:31 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1599d0444630b3ac11f8d61742ff79acaaec1b9cfcca5e176b131ef54c22bd`  
		Last Modified: Fri, 24 Mar 2023 20:21:32 GMT  
		Size: 8.3 KB (8264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cbc52fa8b34cbd17b27c7c562e83344a928724a395e74a740d6bcfbd0aca1e8`  
		Last Modified: Fri, 24 Mar 2023 20:21:32 GMT  
		Size: 1.8 MB (1827370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:latest` - linux; arm variant v7

```console
$ docker pull solr@sha256:8544ae0dc85e554f5d5267937f74c720c90b07f1cf05ffc3201f4eb9095b42dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **369.0 MB (369045467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73e472402be480932e64f4a05bda9a60df8996c5852b59ceb376c284295bafa8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:31:41 GMT
ADD file:e9c3ac290fb81ae2e78de99052d776396ee3aff05e1a66fd2dccb01d7de9bb45 in / 
# Wed, 08 Mar 2023 04:31:42 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:46:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 02:46:15 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 02:46:15 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 02:49:36 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:59:26 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:59:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:59:55 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:52:45 GMT
ARG SOLR_VERSION=9.2.0
# Wed, 26 Apr 2023 20:52:45 GMT
ARG SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665
# Wed, 26 Apr 2023 20:52:45 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Wed, 26 Apr 2023 20:52:45 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:52:46 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:52:46 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:52:46 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:52:46 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:53:18 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:53:20 GMT
LABEL org.opencontainers.image.version=9.2.0
# Wed, 26 Apr 2023 20:53:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:53:21 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:53:21 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:53:22 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:53:22 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:53:32 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:53:32 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:53:32 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:53:32 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:53:32 GMT
USER 8983
# Wed, 26 Apr 2023 20:53:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:53:33 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:cba1fa3bcdf4f746dcf5b8f86874cee4a6eff75dd5c5cd29e4c912574b12a1c6`  
		Last Modified: Thu, 09 Mar 2023 04:41:14 GMT  
		Size: 27.0 MB (27025397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85169cff2ee4bc04fcfaf94a937435e69eb27ca38bf1dcbd04593cccacf0d702`  
		Last Modified: Thu, 16 Mar 2023 02:56:32 GMT  
		Size: 17.1 MB (17093778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de292b783be3523048fe05ba87f22c3948fb2a4468235c054ea6a35a4f7a053`  
		Last Modified: Wed, 26 Apr 2023 20:03:03 GMT  
		Size: 44.6 MB (44579974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05ce4c34b22f40a9acec67a1a46b86a1435158c0dc9bd6e001f1bf7d77326a5`  
		Last Modified: Wed, 26 Apr 2023 20:02:56 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7651a81ea9e32ab5c6154450135c9f73f51999c9aaa7b801c5f62089fe7acb50`  
		Last Modified: Wed, 26 Apr 2023 20:57:10 GMT  
		Size: 278.7 MB (278680039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bbc9eb9d4ef7ab913012093550bd6110ea6f7556b355caddf44f4b7a8a145fa`  
		Last Modified: Wed, 26 Apr 2023 20:56:56 GMT  
		Size: 4.2 KB (4226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cf324cc98872102c6e9fbf9d55d4a0ab567ca7652ca01e8cc4ffc4e33366b6`  
		Last Modified: Wed, 26 Apr 2023 20:56:56 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddea7d711377bed446cb0468d2e74276ea12f53af7dd1f6975b66c6911baf6b`  
		Last Modified: Wed, 26 Apr 2023 20:56:56 GMT  
		Size: 8.3 KB (8261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac376cfc47e23bc8413e65021ee472c27047ebd1ad83f73d4053e0a55edcd477`  
		Last Modified: Wed, 26 Apr 2023 20:56:56 GMT  
		Size: 1.7 MB (1653413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:latest` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:58619b9500a6637702a27985f2cf8b17cb13dae6c2673f3abaa9a1bd824277ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **373.6 MB (373587696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25f72e1df4e02c02f553d7d54dd64951829dbdd59095775a6634ddce70eadc8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:52:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 01:52:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 01:52:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 01:55:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:55:04 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Thu, 16 Mar 2023 01:55:29 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 16 Mar 2023 01:55:30 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_VERSION=9.2.0
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 24 Mar 2023 20:47:30 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:47:31 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:47:31 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Fri, 24 Mar 2023 20:48:14 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 24 Mar 2023 20:48:16 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 24 Mar 2023 20:48:17 GMT
LABEL org.opencontainers.image.version=9.2.0
# Fri, 24 Mar 2023 20:48:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 24 Mar 2023 20:48:17 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 24 Mar 2023 20:48:17 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 24 Mar 2023 20:48:18 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 24 Mar 2023 20:48:18 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 24 Mar 2023 20:48:27 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 24 Mar 2023 20:48:27 GMT
VOLUME [/var/solr]
# Fri, 24 Mar 2023 20:48:27 GMT
EXPOSE 8983
# Fri, 24 Mar 2023 20:48:27 GMT
WORKDIR /opt/solr
# Fri, 24 Mar 2023 20:48:28 GMT
USER 8983
# Fri, 24 Mar 2023 20:48:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Mar 2023 20:48:28 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40b70fd7935308ad0e072e7e06ec8c3abdc59beae70ca716dcd04e971680865`  
		Last Modified: Thu, 16 Mar 2023 02:00:42 GMT  
		Size: 18.4 MB (18400790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33dd5efa5ce73b25dc0236fcd408527b63e42c87e6da9672a356731004b8949`  
		Last Modified: Thu, 16 Mar 2023 02:01:25 GMT  
		Size: 46.4 MB (46421360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ce9280353ea6c4511dc5378e2f0f4742d499bf6df15c8d10804513c8c5115a`  
		Last Modified: Thu, 16 Mar 2023 02:01:20 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85ed965ce21582560c60a815ae59ae9cf0fcb5c9270ba02dfc5ca1c135b44f`  
		Last Modified: Fri, 24 Mar 2023 20:49:04 GMT  
		Size: 278.7 MB (278678702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a47faea25001b6a9178cab60304409e81d636878232dda7e76d519e7490bbc9`  
		Last Modified: Fri, 24 Mar 2023 20:48:54 GMT  
		Size: 4.3 KB (4331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7792e9b554723df7cdd9593ee715d8fe16cfec71a28c58e0b01e2534e7f2c8`  
		Last Modified: Fri, 24 Mar 2023 20:48:54 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9435de9f76e1e09e2078c456e20cd6a83a757671ecc43398fed205b323cb3c6b`  
		Last Modified: Fri, 24 Mar 2023 20:48:54 GMT  
		Size: 8.3 KB (8261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fc7a7f4116bfd1b88180e25c33fa7c4d571df7caad6ffebbec7786b32b2738`  
		Last Modified: Fri, 24 Mar 2023 20:48:54 GMT  
		Size: 1.7 MB (1686320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:latest` - linux; ppc64le

```console
$ docker pull solr@sha256:f390f3d9f15f1aa1bbad8f1f2e7d13c3cc0599c722e9b9751d40ee71aa084561
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.4 MB (381368174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c8aecc2dc5554acdda867249e249f23bafb21f089ae5b92d1530289c7651a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:16 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:20 GMT
ADD file:d7434a52d8d8aa6288e788f6fe7e156f0e11bf9b8275efaf70aab0bfc4d919cf in / 
# Wed, 08 Mar 2023 04:39:20 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:57:34 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 03:57:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 03:57:35 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 04:03:27 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:23:33 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:26:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:26:14 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:36:53 GMT
ARG SOLR_VERSION=9.2.0
# Wed, 26 Apr 2023 20:36:54 GMT
ARG SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665
# Wed, 26 Apr 2023 20:36:54 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Wed, 26 Apr 2023 20:36:54 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:36:54 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:36:55 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:36:55 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:36:55 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:38:40 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Wed, 26 Apr 2023 20:38:44 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:38:44 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:38:44 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:38:44 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:38:45 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:38:45 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:38:45 GMT
LABEL org.opencontainers.image.version=9.2.0
# Wed, 26 Apr 2023 20:38:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:38:46 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:38:47 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:38:48 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:38:49 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:39:04 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:39:05 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:39:05 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:39:05 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:39:05 GMT
USER 8983
# Wed, 26 Apr 2023 20:39:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:39:06 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:deffc758660db3b0ee7a1f211d720633f06f27ab1e4c31db4caf8c27f4a80eeb`  
		Last Modified: Thu, 16 Mar 2023 02:22:27 GMT  
		Size: 35.7 MB (35711728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c06c33e4689e5957d961321ac18da32bea369d2eccc9173c9ad8b517f802ea`  
		Last Modified: Thu, 16 Mar 2023 04:14:09 GMT  
		Size: 18.3 MB (18257665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25abdd535a180a29cc8edf36ac17eb237551826124456d77040e4d464bceb120`  
		Last Modified: Wed, 26 Apr 2023 19:37:08 GMT  
		Size: 46.9 MB (46872523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9532e0e54e3616e367a6095c24ff50105415ae0333e1fabc59c04be22f053e`  
		Last Modified: Wed, 26 Apr 2023 19:36:55 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182d7fc15b9c08e18cdc6cdf0160b68aa45d1b34992b787cdd7f49c9e030e2c9`  
		Last Modified: Wed, 26 Apr 2023 20:43:58 GMT  
		Size: 278.7 MB (278679581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585651ad84270f628cfb14608c4dbb4e3a7a7d865d31747e5aa6084bd109a1c0`  
		Last Modified: Wed, 26 Apr 2023 20:43:36 GMT  
		Size: 4.3 KB (4298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ed3ec073534fcdcfe0bb91a989a24838b5fae6c4a74b6a898b2dc3694b5407`  
		Last Modified: Wed, 26 Apr 2023 20:43:36 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450540c1db3e7e00d5d9ef4f2fc497c849bf895bc1c6478b3017070f8938b7ee`  
		Last Modified: Wed, 26 Apr 2023 20:43:36 GMT  
		Size: 8.3 KB (8255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9738eccb09731f4eae5b20b3bec3d18ba11a98334974ff4f652999eabd29c1`  
		Last Modified: Wed, 26 Apr 2023 20:43:37 GMT  
		Size: 1.8 MB (1833743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:latest` - linux; s390x

```console
$ docker pull solr@sha256:3bf7b256991de31d033da2ffbf31cb9b6d95ef615a6b9792a34577903efd2612
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **369.6 MB (369641824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33ecafe05af5a8d70f6d65e63cea1441abacad2ed33f011d1fd02de369e339bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:26 GMT
ADD file:630f9865d3d4fd4294d45cac7cbaea83fb549c2e563de454348da964d19fbbba in / 
# Wed, 08 Mar 2023 04:39:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:06:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 02:06:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 02:06:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 02:07:58 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:43:50 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:44:49 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:44:51 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:34:03 GMT
ARG SOLR_VERSION=9.2.0
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:34:04 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz
# Wed, 26 Apr 2023 20:34:40 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=3;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;   apt-get -y remove gpg dirmngr && apt-get -y autoremove;
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.version=9.2.0
# Wed, 26 Apr 2023 20:34:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Apr 2023 20:34:45 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Wed, 26 Apr 2023 20:34:46 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 26 Apr 2023 20:34:46 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Wed, 26 Apr 2023 20:34:47 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Wed, 26 Apr 2023 20:34:51 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.2.0/solr-9.2.0.tgz SOLR_KEYS=50E3EE1C91C7E0CB4DFB007B369424FC98F3F6EC SOLR_SHA512=f10c5e15a52882501bc29af11855066238c798658a21c8ccf780dcbdd269a1534a2d06e47f743a2c6331d4e45ab9c976cf7099337422698c4418c6373d284665 SOLR_VERSION=9.2.0
RUN set -ex;     apt-get update;     apt-get -y install acl lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Apr 2023 20:34:51 GMT
VOLUME [/var/solr]
# Wed, 26 Apr 2023 20:34:51 GMT
EXPOSE 8983
# Wed, 26 Apr 2023 20:34:52 GMT
WORKDIR /opt/solr
# Wed, 26 Apr 2023 20:34:52 GMT
USER 8983
# Wed, 26 Apr 2023 20:34:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 20:34:52 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:2c7366af510b72cc0b3456fb93cfa0bfc76f7d383db5cb315967e7b1ce2e0c42`  
		Last Modified: Thu, 16 Mar 2023 02:02:40 GMT  
		Size: 28.6 MB (28647599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d28ae42a862e9773a02317b5a0eeb71ddfe3a887bb001c8f23a2786c926287`  
		Last Modified: Thu, 16 Mar 2023 02:13:35 GMT  
		Size: 16.8 MB (16753284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed61af6a2c87d412802d8f160fb683fc3ec859e336bfe78f93cdcc31e81a5d1a`  
		Last Modified: Wed, 26 Apr 2023 19:48:14 GMT  
		Size: 43.8 MB (43774584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1494ca84bd62528d8f5f078978408f8e5d411da7a46a6065b53e647d1149f5e6`  
		Last Modified: Wed, 26 Apr 2023 19:48:08 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10d1906d4f5008ad00b585c01cb6bdfc068441c94a1d90e8d5945b3b3ddcce6`  
		Last Modified: Wed, 26 Apr 2023 20:37:47 GMT  
		Size: 278.7 MB (278679157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135adf4cb67937fdd1cdf49ca0951324c2a557081953bdf42ed6010b5aadad12`  
		Last Modified: Wed, 26 Apr 2023 20:37:35 GMT  
		Size: 4.3 KB (4329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1770bb3c6b573d4b988aa5479ae3f73c2af9183c16554ec894a2dcb2394a50e`  
		Last Modified: Wed, 26 Apr 2023 20:37:36 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7508a18ea82d8ebe5d57e272b8378f77364d1c20247feab03855086fe8a39fd`  
		Last Modified: Wed, 26 Apr 2023 20:37:36 GMT  
		Size: 8.3 KB (8260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6560f9ee79577800018ac8eba33b185d6cdae6b516d8bb88d5d469a7ddcc2e3a`  
		Last Modified: Wed, 26 Apr 2023 20:37:36 GMT  
		Size: 1.8 MB (1774233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
