## `solr:slim`

```console
$ docker pull solr@sha256:ef48f73f752c8814af9e6f22db4a3f54186f4afe48f55f1986ba5b153b8009da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `solr:slim` - linux; amd64

```console
$ docker pull solr@sha256:3d7f5180d5b57dcc7fef6eccb2c08e19af43a4896b22f0f71b6924011d9d2e65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.3 MB (302324546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62cebb137a7c25cd7af6d2499a15c558a454659ee7c783dfce4c873c25879e8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:20:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 28 Sep 2021 09:20:42 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:20:42 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:20:43 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:20:43 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 28 Sep 2021 09:23:38 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Wed, 29 Sep 2021 10:36:12 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 29 Sep 2021 10:36:13 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 01 Oct 2021 02:00:00 GMT
ARG SOLR_VERSION=8.10.0
# Fri, 01 Oct 2021 02:00:01 GMT
ARG SOLR_SHA512=7bd884f9bb2ee0a632156996c710e8d755db34408b503093570bcef43c085d814b27e1f39fd78e6af7349e390b20e084923188a05876badedbad07e21e3a1757
# Fri, 01 Oct 2021 02:00:01 GMT
ARG SOLR_KEYS=FBC25D7E1712025294FE66590A6AA179B9BBF45E
# Fri, 01 Oct 2021 02:00:01 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 01 Oct 2021 02:00:01 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 01 Oct 2021 02:00:10 GMT
# ARGS: SOLR_KEYS=FBC25D7E1712025294FE66590A6AA179B9BBF45E SOLR_SHA512=7bd884f9bb2ee0a632156996c710e8d755db34408b503093570bcef43c085d814b27e1f39fd78e6af7349e390b20e084923188a05876badedbad07e21e3a1757 SOLR_VERSION=8.10.0
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 01 Oct 2021 02:00:10 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.10.0/solr-8.10.0.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.10.0/solr-8.10.0.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.10.0/solr-8.10.0.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 01 Oct 2021 02:00:11 GMT
# ARGS: SOLR_KEYS=FBC25D7E1712025294FE66590A6AA179B9BBF45E SOLR_SHA512=7bd884f9bb2ee0a632156996c710e8d755db34408b503093570bcef43c085d814b27e1f39fd78e6af7349e390b20e084923188a05876badedbad07e21e3a1757 SOLR_VERSION=8.10.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 01 Oct 2021 02:00:14 GMT
# ARGS: SOLR_KEYS=FBC25D7E1712025294FE66590A6AA179B9BBF45E SOLR_SHA512=7bd884f9bb2ee0a632156996c710e8d755db34408b503093570bcef43c085d814b27e1f39fd78e6af7349e390b20e084923188a05876badedbad07e21e3a1757 SOLR_VERSION=8.10.0
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 01 Oct 2021 02:00:24 GMT
# ARGS: SOLR_KEYS=FBC25D7E1712025294FE66590A6AA179B9BBF45E SOLR_SHA512=7bd884f9bb2ee0a632156996c710e8d755db34408b503093570bcef43c085d814b27e1f39fd78e6af7349e390b20e084923188a05876badedbad07e21e3a1757 SOLR_VERSION=8.10.0
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 01 Oct 2021 02:00:25 GMT
COPY --chown=0:0dir:9bc5f3733a819401f8f06067a2f41713605d2c3bb03bbbe92d04dc2f83bd0265 in /opt/docker-solr/scripts 
# Fri, 01 Oct 2021 02:00:25 GMT
VOLUME [/var/solr]
# Fri, 01 Oct 2021 02:00:25 GMT
EXPOSE 8983
# Fri, 01 Oct 2021 02:00:25 GMT
WORKDIR /opt/solr
# Fri, 01 Oct 2021 02:00:26 GMT
USER solr
# Fri, 01 Oct 2021 02:00:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Oct 2021 02:00:26 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc7fec72146c7ce5a6ca7ee0750b1c72d0554380437767653dcb8dc27d303e4`  
		Last Modified: Tue, 28 Sep 2021 09:34:00 GMT  
		Size: 1.6 MB (1582018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c358bab58aafe7953024dec2395ce3385361e6be5c9d9ad1eddea9778be0a1`  
		Last Modified: Tue, 28 Sep 2021 09:42:41 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12f81e19ff214b2e1faf681ba8c235d1febe310c4c5356b13826ef22647b543`  
		Last Modified: Tue, 28 Sep 2021 09:45:35 GMT  
		Size: 47.1 MB (47129875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ada455e4db4a1af031f97141fa113c22400bab6c156dbf190cbff1e458ac59b`  
		Last Modified: Fri, 01 Oct 2021 02:03:21 GMT  
		Size: 6.9 MB (6898123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b121283a79761fde60df1a6bcebad2f3160edce71287ef659d4ebbccf056a4`  
		Last Modified: Fri, 01 Oct 2021 02:03:22 GMT  
		Size: 4.3 KB (4286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7f47259be17492b3477f8e2d7b54b9e34d8d25ee489914ea912ba1d86b7887`  
		Last Modified: Fri, 01 Oct 2021 02:03:20 GMT  
		Size: 2.9 KB (2928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d72dd6a59e7b90fd8ffa218c28f41f9629e19554b3250b279d507bf6fad7375`  
		Last Modified: Fri, 01 Oct 2021 02:03:31 GMT  
		Size: 215.3 MB (215331918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea031c6640afea4dcc678b6a1a7a903fbd276bcb927f3889d987818bfe4ec09`  
		Last Modified: Fri, 01 Oct 2021 02:03:20 GMT  
		Size: 6.3 KB (6275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:slim` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:9a8a767f4976943d857fc56c5ae0ff5b6adafd19a1b2c772bca87558c76aaa97
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.5 MB (299538697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:673c2607b86b6148f8a55af92e017fd96181ff35a03ec74d038bed0361bb7f33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:18 GMT
ADD file:d84144ad575672cd6cc8a00c8e5a88ab0545348f040fc249ea5fcf8193b2bce6 in / 
# Tue, 12 Oct 2021 01:41:18 GMT
CMD ["bash"]
# Wed, 13 Oct 2021 06:00:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 06:09:36 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 13 Oct 2021 06:09:37 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 13 Oct 2021 06:09:38 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 06:09:39 GMT
ENV LANG=C.UTF-8
# Wed, 13 Oct 2021 06:09:40 GMT
ENV JAVA_VERSION=11.0.12
# Wed, 13 Oct 2021 06:11:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Wed, 13 Oct 2021 11:08:19 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 13 Oct 2021 11:08:20 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 13 Oct 2021 11:08:21 GMT
ARG SOLR_VERSION=8.10.0
# Wed, 13 Oct 2021 11:08:22 GMT
ARG SOLR_SHA512=7bd884f9bb2ee0a632156996c710e8d755db34408b503093570bcef43c085d814b27e1f39fd78e6af7349e390b20e084923188a05876badedbad07e21e3a1757
# Wed, 13 Oct 2021 11:08:23 GMT
ARG SOLR_KEYS=FBC25D7E1712025294FE66590A6AA179B9BBF45E
# Wed, 13 Oct 2021 11:08:24 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 13 Oct 2021 11:08:25 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 13 Oct 2021 11:08:32 GMT
# ARGS: SOLR_KEYS=FBC25D7E1712025294FE66590A6AA179B9BBF45E SOLR_SHA512=7bd884f9bb2ee0a632156996c710e8d755db34408b503093570bcef43c085d814b27e1f39fd78e6af7349e390b20e084923188a05876badedbad07e21e3a1757 SOLR_VERSION=8.10.0
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 13 Oct 2021 11:08:33 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.10.0/solr-8.10.0.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.10.0/solr-8.10.0.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.10.0/solr-8.10.0.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 13 Oct 2021 11:08:34 GMT
# ARGS: SOLR_KEYS=FBC25D7E1712025294FE66590A6AA179B9BBF45E SOLR_SHA512=7bd884f9bb2ee0a632156996c710e8d755db34408b503093570bcef43c085d814b27e1f39fd78e6af7349e390b20e084923188a05876badedbad07e21e3a1757 SOLR_VERSION=8.10.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 13 Oct 2021 11:08:40 GMT
# ARGS: SOLR_KEYS=FBC25D7E1712025294FE66590A6AA179B9BBF45E SOLR_SHA512=7bd884f9bb2ee0a632156996c710e8d755db34408b503093570bcef43c085d814b27e1f39fd78e6af7349e390b20e084923188a05876badedbad07e21e3a1757 SOLR_VERSION=8.10.0
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 13 Oct 2021 11:08:48 GMT
# ARGS: SOLR_KEYS=FBC25D7E1712025294FE66590A6AA179B9BBF45E SOLR_SHA512=7bd884f9bb2ee0a632156996c710e8d755db34408b503093570bcef43c085d814b27e1f39fd78e6af7349e390b20e084923188a05876badedbad07e21e3a1757 SOLR_VERSION=8.10.0
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 13 Oct 2021 11:08:49 GMT
COPY --chown=0:0dir:9bc5f3733a819401f8f06067a2f41713605d2c3bb03bbbe92d04dc2f83bd0265 in /opt/docker-solr/scripts 
# Wed, 13 Oct 2021 11:08:49 GMT
VOLUME [/var/solr]
# Wed, 13 Oct 2021 11:08:50 GMT
EXPOSE 8983
# Wed, 13 Oct 2021 11:08:51 GMT
WORKDIR /opt/solr
# Wed, 13 Oct 2021 11:08:52 GMT
USER solr
# Wed, 13 Oct 2021 11:08:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Oct 2021 11:08:54 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:a9eb63951c1c2ee8efcc12b696928fee3741a2d4eae76f2da3e161a5d90548bf`  
		Last Modified: Tue, 12 Oct 2021 01:48:13 GMT  
		Size: 30.0 MB (30043906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8552e0d309d6deaf17b87f395ca03a5bb0b4c14128cd49208ab21c34bf39e933`  
		Last Modified: Wed, 13 Oct 2021 06:25:32 GMT  
		Size: 1.6 MB (1565908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c654db09bcc79500b8b4835083562086d498045750c7ce5721d4beab40690d`  
		Last Modified: Wed, 13 Oct 2021 06:38:41 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01bf26d26431a78a90e003223885dbd1921cada6d650354a6e8993b51ddd2af`  
		Last Modified: Wed, 13 Oct 2021 06:41:29 GMT  
		Size: 46.0 MB (45986006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99631a0616b34ed1b2d4023b57efeb79f099b0cbde88ea969ea6d4136821e277`  
		Last Modified: Wed, 13 Oct 2021 11:38:53 GMT  
		Size: 6.6 MB (6597729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4888e24113c679a13b9946bedc1ffc851ae143cea27ea29c12e66b1f2bcbfdb`  
		Last Modified: Wed, 13 Oct 2021 11:38:52 GMT  
		Size: 4.2 KB (4198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7839438a635d1791ca9f084bfc69bdc686e3af83a2c0b815ecdf63a78ddfb69f`  
		Last Modified: Wed, 13 Oct 2021 11:38:52 GMT  
		Size: 2.9 KB (2895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e5bb00e2b4c88820e9dc488dd80e81a19bedc9527e78c619dd7aba71e0c216`  
		Last Modified: Wed, 13 Oct 2021 11:39:12 GMT  
		Size: 215.3 MB (215331597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0d1470a9b0c189ce04d3032e9ad96542095e751b1109f049bda910846d0c70`  
		Last Modified: Wed, 13 Oct 2021 11:38:52 GMT  
		Size: 6.2 KB (6247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
