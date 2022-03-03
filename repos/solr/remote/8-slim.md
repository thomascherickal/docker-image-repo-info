## `solr:8-slim`

```console
$ docker pull solr@sha256:be5468e40da14d4bd93a04f068cfecff99cd2fc4a00670928d24ee1a3d650e48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `solr:8-slim` - linux; amd64

```console
$ docker pull solr@sha256:ed692f213c43e82c08ea861fe82ed14f62c1aef5a1b3b4769f24a6d608b11baa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.3 MB (305250736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fe288cb1aa2bc8635c6e65fd8abaeab9be4cba49fa7542bf4c1ce4330854baf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 14:21:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 14:28:00 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 01 Mar 2022 14:28:01 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 01 Mar 2022 14:28:01 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 14:28:01 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 14:28:01 GMT
ENV JAVA_VERSION=11.0.14.1
# Tue, 01 Mar 2022 14:30:18 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Wed, 02 Mar 2022 21:36:53 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 02 Mar 2022 21:36:53 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 02 Mar 2022 21:36:53 GMT
ARG SOLR_VERSION=8.11.1
# Wed, 02 Mar 2022 21:36:53 GMT
ARG SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45
# Wed, 02 Mar 2022 21:36:54 GMT
ARG SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E
# Wed, 02 Mar 2022 21:36:54 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 02 Mar 2022 21:36:54 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 02 Mar 2022 21:37:06 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 02 Mar 2022 21:37:06 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.1/solr-8.11.1.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 02 Mar 2022 21:37:07 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 02 Mar 2022 21:37:25 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 02 Mar 2022 21:38:03 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 02 Mar 2022 21:38:04 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 02 Mar 2022 21:38:04 GMT
VOLUME [/var/solr]
# Wed, 02 Mar 2022 21:38:04 GMT
EXPOSE 8983
# Wed, 02 Mar 2022 21:38:05 GMT
WORKDIR /opt/solr
# Wed, 02 Mar 2022 21:38:05 GMT
USER solr
# Wed, 02 Mar 2022 21:38:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Mar 2022 21:38:05 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8366d5a4a5f71bf009ed651eb5566bf81bcd61ddaa4a2541fc65505bb076ca`  
		Last Modified: Tue, 01 Mar 2022 14:40:45 GMT  
		Size: 1.6 MB (1582090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3634e671f7dc632d921a097fe73b18827d8bb820de8629789b27342956ea45e`  
		Last Modified: Tue, 01 Mar 2022 14:49:45 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715bddf5d050e2e23dc57b2e7809eb93613da14342668a8560e73fae0305ef57`  
		Last Modified: Tue, 01 Mar 2022 14:53:02 GMT  
		Size: 47.2 MB (47151809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171a3f2b512f1661624a7f41a307c643709ec58e08a9054f80e0b7e392d61065`  
		Last Modified: Wed, 02 Mar 2022 22:45:27 GMT  
		Size: 6.9 MB (6902395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a68f988e2c88aa16440a034eada723b3a96626d96e82e2260e19045c908244`  
		Last Modified: Wed, 02 Mar 2022 22:45:24 GMT  
		Size: 4.3 KB (4283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27be21c9f36c8dd0dd6a5ffe89d67cfa1aaadf4f0d60187a929c47ec39e8cc0e`  
		Last Modified: Wed, 02 Mar 2022 22:45:24 GMT  
		Size: 5.1 KB (5113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027335b646680c31b30565614800da9721e8af46d8c3942b90ca619d751dcbed`  
		Last Modified: Wed, 02 Mar 2022 22:45:42 GMT  
		Size: 218.2 MB (218232131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabb32c503e58ca1c3cab5a5aaa095c06b91a6e16047a52d6231ab30ff14e8ca`  
		Last Modified: Wed, 02 Mar 2022 22:45:24 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8-slim` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:2a0ce69b5a158791a04d1111e720089a2dd205cc3c7681c0c5ccca44e22003b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.5 MB (302500069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2a045d5f6543dfad2855761382e4852a6f4f0e4c0d1c6384400354dd3b03d56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:29 GMT
ADD file:9816c9c29627693c34afda4fa5e1a5e8a0f5aa3c5d5cfd920a4d89c77aab997d in / 
# Tue, 01 Mar 2022 02:11:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:48:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:55:42 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 01 Mar 2022 13:55:43 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 01 Mar 2022 13:55:44 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 13:55:45 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 13:55:46 GMT
ENV JAVA_VERSION=11.0.14.1
# Tue, 01 Mar 2022 13:58:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Wed, 02 Mar 2022 10:25:09 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 02 Mar 2022 10:25:10 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 02 Mar 2022 10:25:11 GMT
ARG SOLR_VERSION=8.11.1
# Wed, 02 Mar 2022 10:25:12 GMT
ARG SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45
# Wed, 02 Mar 2022 10:25:13 GMT
ARG SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E
# Wed, 02 Mar 2022 10:25:14 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 02 Mar 2022 10:25:15 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 02 Mar 2022 10:25:23 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 02 Mar 2022 10:25:23 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.1/solr-8.11.1.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 02 Mar 2022 10:25:24 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 02 Mar 2022 10:25:42 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 02 Mar 2022 10:26:44 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 02 Mar 2022 10:26:45 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 02 Mar 2022 10:26:45 GMT
VOLUME [/var/solr]
# Wed, 02 Mar 2022 10:26:46 GMT
EXPOSE 8983
# Wed, 02 Mar 2022 10:26:47 GMT
WORKDIR /opt/solr
# Wed, 02 Mar 2022 10:26:48 GMT
USER solr
# Wed, 02 Mar 2022 10:26:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Mar 2022 10:26:50 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:279a020076a7fbddfc996e4c55e605a8f322810c3eca21cdedbcb06beb0e1305`  
		Last Modified: Tue, 01 Mar 2022 02:18:24 GMT  
		Size: 30.1 MB (30057008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eee4a8201309b4b9bb0e0e0efc8d45265ae39d932512f5edb149b65eaf107d9`  
		Last Modified: Tue, 01 Mar 2022 14:12:59 GMT  
		Size: 1.6 MB (1565936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10681f9e29336bf4b9d3ce1ab7d3e21c5e5443d865dd506aa9916d227405eaa0`  
		Last Modified: Tue, 01 Mar 2022 14:22:23 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818c6d19bbc2745a3c657e2c1817002e564b298bad28a387c497de4e28c16b0a`  
		Last Modified: Tue, 01 Mar 2022 14:25:49 GMT  
		Size: 46.0 MB (46029806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580104e9c7a60acee6634691c623afb8faf5f04d66be9211cb7c9f4f70ad8233`  
		Last Modified: Wed, 02 Mar 2022 11:04:36 GMT  
		Size: 6.6 MB (6600943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3dee041c44ce236d8a2b5e1b29a2cd6b15c2c70426813c0df83c0f577cec98`  
		Last Modified: Wed, 02 Mar 2022 11:04:35 GMT  
		Size: 4.2 KB (4197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d22f9a2157ad8bdf089ed56202cbe941074a57387d3dcf06e4a7523dfa03e4`  
		Last Modified: Wed, 02 Mar 2022 11:04:35 GMT  
		Size: 5.1 KB (5081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548b29c6a7922b2f514216f66dc30d22fe064fd395401cb3ddfbba897c82305c`  
		Last Modified: Wed, 02 Mar 2022 11:04:55 GMT  
		Size: 218.2 MB (218230607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:313e9f917fe007d0e8a2ec5d4e2a169732013d396b4b5bb799a6b01a2a34f77f`  
		Last Modified: Wed, 02 Mar 2022 11:04:35 GMT  
		Size: 6.3 KB (6280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
