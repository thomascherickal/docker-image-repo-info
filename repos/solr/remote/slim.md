## `solr:slim`

```console
$ docker pull solr@sha256:c9104e1ce376d57c3ada9e6d1fafd390016ae2c20c50a4fe21f487ad8dd949c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `solr:slim` - linux; amd64

```console
$ docker pull solr@sha256:4f65b7b0da8759eb5777e218dfc9e297fa296b728fca584bafe06351dc4a2a42
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274807459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b6f455868f5c214e38c2f10d484b9a53a35d7129572f6ac95355bf6846d22c9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:58:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:58:53 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 09:03:20 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 13 Oct 2020 09:03:20 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 09:03:21 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 13 Oct 2020 09:03:22 GMT
ENV JAVA_VERSION=11.0.8
# Tue, 13 Oct 2020 09:04:49 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_aarch64_linux_11.0.8_10.tar.gz ;; 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_x64_linux_11.0.8_10.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Wed, 14 Oct 2020 06:01:39 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 14 Oct 2020 06:01:39 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 14 Oct 2020 06:01:40 GMT
ARG SOLR_VERSION=8.6.3
# Wed, 14 Oct 2020 06:01:40 GMT
ARG SOLR_SHA512=f040d4489118b655bd27451a717c1f22f180c398638d944a53889a1a449e7032b016cecbff1979c2e8bfd51fc037dd613f3b968254001d34fe0e8fc4f6761dcf
# Wed, 14 Oct 2020 06:01:40 GMT
ARG SOLR_KEYS=902CC51935C140BF820230961FD5295281436075
# Wed, 14 Oct 2020 06:01:40 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 14 Oct 2020 06:01:40 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 14 Oct 2020 06:01:48 GMT
# ARGS: SOLR_KEYS=902CC51935C140BF820230961FD5295281436075 SOLR_SHA512=f040d4489118b655bd27451a717c1f22f180c398638d944a53889a1a449e7032b016cecbff1979c2e8bfd51fc037dd613f3b968254001d34fe0e8fc4f6761dcf SOLR_VERSION=8.6.3
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 14 Oct 2020 06:01:48 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.6.3/solr-8.6.3.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.6.3/solr-8.6.3.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.6.3/solr-8.6.3.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 14 Oct 2020 06:01:49 GMT
# ARGS: SOLR_KEYS=902CC51935C140BF820230961FD5295281436075 SOLR_SHA512=f040d4489118b655bd27451a717c1f22f180c398638d944a53889a1a449e7032b016cecbff1979c2e8bfd51fc037dd613f3b968254001d34fe0e8fc4f6761dcf SOLR_VERSION=8.6.3
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 14 Oct 2020 06:01:50 GMT
# ARGS: SOLR_KEYS=902CC51935C140BF820230961FD5295281436075 SOLR_SHA512=f040d4489118b655bd27451a717c1f22f180c398638d944a53889a1a449e7032b016cecbff1979c2e8bfd51fc037dd613f3b968254001d34fe0e8fc4f6761dcf SOLR_VERSION=8.6.3
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 14 Oct 2020 06:02:19 GMT
# ARGS: SOLR_KEYS=902CC51935C140BF820230961FD5295281436075 SOLR_SHA512=f040d4489118b655bd27451a717c1f22f180c398638d944a53889a1a449e7032b016cecbff1979c2e8bfd51fc037dd613f3b968254001d34fe0e8fc4f6761dcf SOLR_VERSION=8.6.3
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 14 Oct 2020 06:02:19 GMT
COPY --chown=0:0dir:9bc5f3733a819401f8f06067a2f41713605d2c3bb03bbbe92d04dc2f83bd0265 in /opt/docker-solr/scripts 
# Wed, 14 Oct 2020 06:02:19 GMT
VOLUME [/var/solr]
# Wed, 14 Oct 2020 06:02:19 GMT
EXPOSE 8983
# Wed, 14 Oct 2020 06:02:20 GMT
WORKDIR /opt/solr
# Wed, 14 Oct 2020 06:02:20 GMT
USER solr
# Wed, 14 Oct 2020 06:02:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Oct 2020 06:02:20 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00028440d132be6f9dd59a787bc5d1372d575a539c19954651757f12912f2e65`  
		Last Modified: Tue, 13 Oct 2020 09:08:08 GMT  
		Size: 3.2 MB (3248445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd07266fb437b6b55170580d257a3cb1cd0fd3f85ffb57552d1a1017b7bed24`  
		Last Modified: Tue, 13 Oct 2020 09:11:50 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4194f179c57f8ab61f02a649b3a35ba182212b17a4be3ab1192d77b1d08e65b8`  
		Last Modified: Tue, 13 Oct 2020 09:12:39 GMT  
		Size: 42.2 MB (42225252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadb7856ac89b4ba86ee854016a7cf8e16d60a33bb2e0e3bf4dbf58a92805dd0`  
		Last Modified: Wed, 14 Oct 2020 06:14:53 GMT  
		Size: 6.5 MB (6453216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a69493bce3b4e11f346644658e9afc97a7646cc7e4b968f1cd5f61229531364`  
		Last Modified: Wed, 14 Oct 2020 06:14:51 GMT  
		Size: 4.3 KB (4289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d113f81a605e9265623b3c255b6482b7dab940c849d7c1145fd88f0bdef565cf`  
		Last Modified: Wed, 14 Oct 2020 06:14:52 GMT  
		Size: 2.9 KB (2892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d71152e5e66aa61d7bcac7779c2751463f4c1ded6f531a0c73df1d0e7c48be7`  
		Last Modified: Wed, 14 Oct 2020 06:15:03 GMT  
		Size: 195.8 MB (195774678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af117c7d8e7d0d7fd6e1bf1407fbc80df9218610e89ba00d3fe32bbd1aba19c8`  
		Last Modified: Wed, 14 Oct 2020 06:14:51 GMT  
		Size: 6.2 KB (6247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:slim` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:ab8e0980e81ea5c57ee92fba5f95fce08eecef0011d0ca73d6cd2e4e2c4bc31a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.4 MB (272419803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84d288c1894239369ff85824887ea33e593321f803f021f11dcf7dc48d189e42`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:09 GMT
ADD file:3488b1423094a75be5bb5956e9187827b8dd35d7a1f2b14081f8e74a1629e7d0 in / 
# Tue, 13 Oct 2020 01:41:11 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 12:24:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 12:24:15 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 12:27:51 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 13 Oct 2020 12:27:57 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 12:28:12 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 13 Oct 2020 12:28:18 GMT
ENV JAVA_VERSION=11.0.8
# Tue, 13 Oct 2020 12:31:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_aarch64_linux_11.0.8_10.tar.gz ;; 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_x64_linux_11.0.8_10.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Wed, 14 Oct 2020 11:10:14 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 14 Oct 2020 11:10:14 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 14 Oct 2020 11:10:15 GMT
ARG SOLR_VERSION=8.6.3
# Wed, 14 Oct 2020 11:10:16 GMT
ARG SOLR_SHA512=f040d4489118b655bd27451a717c1f22f180c398638d944a53889a1a449e7032b016cecbff1979c2e8bfd51fc037dd613f3b968254001d34fe0e8fc4f6761dcf
# Wed, 14 Oct 2020 11:10:16 GMT
ARG SOLR_KEYS=902CC51935C140BF820230961FD5295281436075
# Wed, 14 Oct 2020 11:10:17 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 14 Oct 2020 11:10:18 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 14 Oct 2020 11:10:46 GMT
# ARGS: SOLR_KEYS=902CC51935C140BF820230961FD5295281436075 SOLR_SHA512=f040d4489118b655bd27451a717c1f22f180c398638d944a53889a1a449e7032b016cecbff1979c2e8bfd51fc037dd613f3b968254001d34fe0e8fc4f6761dcf SOLR_VERSION=8.6.3
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 14 Oct 2020 11:10:47 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.6.3/solr-8.6.3.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.6.3/solr-8.6.3.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.6.3/solr-8.6.3.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 14 Oct 2020 11:10:49 GMT
# ARGS: SOLR_KEYS=902CC51935C140BF820230961FD5295281436075 SOLR_SHA512=f040d4489118b655bd27451a717c1f22f180c398638d944a53889a1a449e7032b016cecbff1979c2e8bfd51fc037dd613f3b968254001d34fe0e8fc4f6761dcf SOLR_VERSION=8.6.3
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 14 Oct 2020 11:10:51 GMT
# ARGS: SOLR_KEYS=902CC51935C140BF820230961FD5295281436075 SOLR_SHA512=f040d4489118b655bd27451a717c1f22f180c398638d944a53889a1a449e7032b016cecbff1979c2e8bfd51fc037dd613f3b968254001d34fe0e8fc4f6761dcf SOLR_VERSION=8.6.3
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 14 Oct 2020 11:11:09 GMT
# ARGS: SOLR_KEYS=902CC51935C140BF820230961FD5295281436075 SOLR_SHA512=f040d4489118b655bd27451a717c1f22f180c398638d944a53889a1a449e7032b016cecbff1979c2e8bfd51fc037dd613f3b968254001d34fe0e8fc4f6761dcf SOLR_VERSION=8.6.3
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 14 Oct 2020 11:11:11 GMT
COPY --chown=0:0dir:9bc5f3733a819401f8f06067a2f41713605d2c3bb03bbbe92d04dc2f83bd0265 in /opt/docker-solr/scripts 
# Wed, 14 Oct 2020 11:11:12 GMT
VOLUME [/var/solr]
# Wed, 14 Oct 2020 11:11:13 GMT
EXPOSE 8983
# Wed, 14 Oct 2020 11:11:14 GMT
WORKDIR /opt/solr
# Wed, 14 Oct 2020 11:11:14 GMT
USER solr
# Wed, 14 Oct 2020 11:11:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Oct 2020 11:11:16 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:4e6164a63b7b4cf981546947e191644c122214975d40b51ede0536791ebec3d4`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 25.8 MB (25849329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51571e799d6113fa90df1694d3dac0eb7b52f4ce6cdddd495020745912328e3f`  
		Last Modified: Tue, 13 Oct 2020 12:34:16 GMT  
		Size: 3.1 MB (3101485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7c34b6cf1a00cac272424dd06c1f2ed5ec8ccfda6a4e9d8ed75c328eab6c78`  
		Last Modified: Tue, 13 Oct 2020 12:37:20 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a520a80b502069b84037dc7cf318e70411b03cdb5119cbc43076fe6bd1320340`  
		Last Modified: Tue, 13 Oct 2020 12:38:41 GMT  
		Size: 41.3 MB (41330898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d61780296d3584261ab81674a933ff54900245757041b86fc9561e4800f6d1`  
		Last Modified: Wed, 14 Oct 2020 11:25:51 GMT  
		Size: 6.3 MB (6349860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c72018f53e4a7c86ca41f52c39b5a4683cbb69fbeb13f363e6e71edad8ef0219`  
		Last Modified: Wed, 14 Oct 2020 11:25:49 GMT  
		Size: 4.3 KB (4323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0b3d2df9dbd91ff95b826b354d0e440d5e9a51f1c5df4c732463bfb6fd9ccb`  
		Last Modified: Wed, 14 Oct 2020 11:25:50 GMT  
		Size: 2.9 KB (2920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79844761008c9d01e7cd2454e6b5e36429e26614f7ceafaf36c3797c4d038c27`  
		Last Modified: Wed, 14 Oct 2020 11:26:24 GMT  
		Size: 195.8 MB (195774501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d932ffc229fb042c1ad838558cd310ce66a7d5cb7a43729f90b74afb2c74a8c1`  
		Last Modified: Wed, 14 Oct 2020 11:25:49 GMT  
		Size: 6.3 KB (6276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
