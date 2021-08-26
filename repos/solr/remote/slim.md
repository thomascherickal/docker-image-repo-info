## `solr:slim`

```console
$ docker pull solr@sha256:dc3d0b70710a130202a7c2708183752f53a99ab10a45c4386f1a83916ce40102
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `solr:slim` - linux; amd64

```console
$ docker pull solr@sha256:d6027fdbb823cf5a06046efd5a7745f4e14e0c2fd8cce4596182088608df72e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.1 MB (290070204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e384608b110098f2a066fcefd467a2d65a208086b65db5e7bd2b784878fd84ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:40 GMT
ADD file:5e8343ab9a73edc27c2889634896e792ab289b85c206de0fc31183fdc0a32ac7 in / 
# Tue, 17 Aug 2021 01:23:41 GMT
CMD ["bash"]
# Thu, 26 Aug 2021 00:33:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Aug 2021 00:36:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 26 Aug 2021 00:36:15 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 26 Aug 2021 00:36:15 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Aug 2021 00:36:15 GMT
ENV LANG=C.UTF-8
# Thu, 26 Aug 2021 00:36:15 GMT
ENV JAVA_VERSION=11.0.12
# Thu, 26 Aug 2021 00:37:39 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 26 Aug 2021 03:22:21 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Thu, 26 Aug 2021 03:22:21 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Thu, 26 Aug 2021 03:22:21 GMT
ARG SOLR_VERSION=8.9.0
# Thu, 26 Aug 2021 03:22:21 GMT
ARG SOLR_SHA512=15150b7f191fd9e8d2c1bd8bb619dd4b3f27af2e0e94b7609031f7e745a2e263391c30f68865c208afb97ccaa9bde6d16050200e9bfccef65f762c2ed743c242
# Thu, 26 Aug 2021 03:22:21 GMT
ARG SOLR_KEYS=9722F25F650057E26C803B60A6D064D833B3A969
# Thu, 26 Aug 2021 03:22:22 GMT
ARG SOLR_DOWNLOAD_URL
# Thu, 26 Aug 2021 03:22:22 GMT
ARG SOLR_DOWNLOAD_SERVER
# Thu, 26 Aug 2021 03:22:29 GMT
# ARGS: SOLR_KEYS=9722F25F650057E26C803B60A6D064D833B3A969 SOLR_SHA512=15150b7f191fd9e8d2c1bd8bb619dd4b3f27af2e0e94b7609031f7e745a2e263391c30f68865c208afb97ccaa9bde6d16050200e9bfccef65f762c2ed743c242 SOLR_VERSION=8.9.0
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Thu, 26 Aug 2021 03:22:29 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.9.0/solr-8.9.0.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.9.0/solr-8.9.0.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.9.0/solr-8.9.0.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Thu, 26 Aug 2021 03:22:30 GMT
# ARGS: SOLR_KEYS=9722F25F650057E26C803B60A6D064D833B3A969 SOLR_SHA512=15150b7f191fd9e8d2c1bd8bb619dd4b3f27af2e0e94b7609031f7e745a2e263391c30f68865c208afb97ccaa9bde6d16050200e9bfccef65f762c2ed743c242 SOLR_VERSION=8.9.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Thu, 26 Aug 2021 03:22:32 GMT
# ARGS: SOLR_KEYS=9722F25F650057E26C803B60A6D064D833B3A969 SOLR_SHA512=15150b7f191fd9e8d2c1bd8bb619dd4b3f27af2e0e94b7609031f7e745a2e263391c30f68865c208afb97ccaa9bde6d16050200e9bfccef65f762c2ed743c242 SOLR_VERSION=8.9.0
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Thu, 26 Aug 2021 03:22:40 GMT
# ARGS: SOLR_KEYS=9722F25F650057E26C803B60A6D064D833B3A969 SOLR_SHA512=15150b7f191fd9e8d2c1bd8bb619dd4b3f27af2e0e94b7609031f7e745a2e263391c30f68865c208afb97ccaa9bde6d16050200e9bfccef65f762c2ed743c242 SOLR_VERSION=8.9.0
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Thu, 26 Aug 2021 03:22:40 GMT
COPY --chown=0:0dir:9bc5f3733a819401f8f06067a2f41713605d2c3bb03bbbe92d04dc2f83bd0265 in /opt/docker-solr/scripts 
# Thu, 26 Aug 2021 03:22:41 GMT
VOLUME [/var/solr]
# Thu, 26 Aug 2021 03:22:41 GMT
EXPOSE 8983
# Thu, 26 Aug 2021 03:22:41 GMT
WORKDIR /opt/solr
# Thu, 26 Aug 2021 03:22:41 GMT
USER solr
# Thu, 26 Aug 2021 03:22:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Aug 2021 03:22:42 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:99046ad9247f8a1cbd1048d9099d026191ad9cda63c08aadeb704b7000a51717`  
		Last Modified: Tue, 17 Aug 2021 01:29:35 GMT  
		Size: 31.4 MB (31361314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97c10298fea9915576e7ff72c6eca3d7c589aaafd6bc6481a5814c4271d2251`  
		Last Modified: Thu, 26 Aug 2021 00:43:26 GMT  
		Size: 1.6 MB (1581998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad67722a7508cc8ca694c9e75efebc7c37f65d179dc2d6f36a9a1615dc5206c`  
		Last Modified: Thu, 26 Aug 2021 00:48:02 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbeb29d69a7c2580a75906597d7cd4d59a9eff12b482810794fa01b105155358`  
		Last Modified: Thu, 26 Aug 2021 00:49:22 GMT  
		Size: 47.1 MB (47126663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552d3b6e26040a46f662414654918d023856981ca307451a46beff186807308b`  
		Last Modified: Thu, 26 Aug 2021 03:42:12 GMT  
		Size: 6.9 MB (6898017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87200e6e526a64f2e7e09a20dfc13da5cd9b8d73eb3b8e8e6fdd11de4fc63729`  
		Last Modified: Thu, 26 Aug 2021 03:42:11 GMT  
		Size: 4.3 KB (4289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f428b2eb3fd584bdfb8df916f023757e838b07f48ea7810e80005ae161a018c1`  
		Last Modified: Thu, 26 Aug 2021 03:42:11 GMT  
		Size: 2.9 KB (2925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c100b17608b7352339b14453d042ec36c52f109e1129ad944e5a7801cb53401f`  
		Last Modified: Thu, 26 Aug 2021 03:42:21 GMT  
		Size: 203.1 MB (203088512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7021ca775a54e2d52e3315bd204d05c76411ef47b31c74441b567f421a03b9a7`  
		Last Modified: Thu, 26 Aug 2021 03:42:11 GMT  
		Size: 6.3 KB (6275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:slim` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:99f3ba5c336dc216be1798326df79f062fb847600f5a4f273f30fbe2181f8357
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.7 MB (287732741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf0d41037e4c9aa73dc5f9c639329369c025c564174792f7bfb89da253ab1475`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:04 GMT
ADD file:0a42d4a201f0ac7889187c3212fbdfc2747f31f36e690d59c22eec50fe542614 in / 
# Tue, 17 Aug 2021 01:46:05 GMT
CMD ["bash"]
# Thu, 26 Aug 2021 00:33:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Aug 2021 00:37:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 26 Aug 2021 00:37:45 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 26 Aug 2021 00:37:46 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Aug 2021 00:37:46 GMT
ENV LANG=C.UTF-8
# Thu, 26 Aug 2021 00:37:46 GMT
ENV JAVA_VERSION=11.0.12
# Thu, 26 Aug 2021 00:38:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 26 Aug 2021 01:53:48 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Thu, 26 Aug 2021 01:53:49 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Thu, 26 Aug 2021 01:53:49 GMT
ARG SOLR_VERSION=8.9.0
# Thu, 26 Aug 2021 01:53:49 GMT
ARG SOLR_SHA512=15150b7f191fd9e8d2c1bd8bb619dd4b3f27af2e0e94b7609031f7e745a2e263391c30f68865c208afb97ccaa9bde6d16050200e9bfccef65f762c2ed743c242
# Thu, 26 Aug 2021 01:53:49 GMT
ARG SOLR_KEYS=9722F25F650057E26C803B60A6D064D833B3A969
# Thu, 26 Aug 2021 01:53:49 GMT
ARG SOLR_DOWNLOAD_URL
# Thu, 26 Aug 2021 01:53:49 GMT
ARG SOLR_DOWNLOAD_SERVER
# Thu, 26 Aug 2021 01:53:56 GMT
# ARGS: SOLR_KEYS=9722F25F650057E26C803B60A6D064D833B3A969 SOLR_SHA512=15150b7f191fd9e8d2c1bd8bb619dd4b3f27af2e0e94b7609031f7e745a2e263391c30f68865c208afb97ccaa9bde6d16050200e9bfccef65f762c2ed743c242 SOLR_VERSION=8.9.0
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Thu, 26 Aug 2021 01:53:56 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.9.0/solr-8.9.0.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.9.0/solr-8.9.0.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.9.0/solr-8.9.0.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Thu, 26 Aug 2021 01:53:57 GMT
# ARGS: SOLR_KEYS=9722F25F650057E26C803B60A6D064D833B3A969 SOLR_SHA512=15150b7f191fd9e8d2c1bd8bb619dd4b3f27af2e0e94b7609031f7e745a2e263391c30f68865c208afb97ccaa9bde6d16050200e9bfccef65f762c2ed743c242 SOLR_VERSION=8.9.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Thu, 26 Aug 2021 01:53:59 GMT
# ARGS: SOLR_KEYS=9722F25F650057E26C803B60A6D064D833B3A969 SOLR_SHA512=15150b7f191fd9e8d2c1bd8bb619dd4b3f27af2e0e94b7609031f7e745a2e263391c30f68865c208afb97ccaa9bde6d16050200e9bfccef65f762c2ed743c242 SOLR_VERSION=8.9.0
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Thu, 26 Aug 2021 01:54:07 GMT
# ARGS: SOLR_KEYS=9722F25F650057E26C803B60A6D064D833B3A969 SOLR_SHA512=15150b7f191fd9e8d2c1bd8bb619dd4b3f27af2e0e94b7609031f7e745a2e263391c30f68865c208afb97ccaa9bde6d16050200e9bfccef65f762c2ed743c242 SOLR_VERSION=8.9.0
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Thu, 26 Aug 2021 01:54:07 GMT
COPY --chown=0:0dir:9bc5f3733a819401f8f06067a2f41713605d2c3bb03bbbe92d04dc2f83bd0265 in /opt/docker-solr/scripts 
# Thu, 26 Aug 2021 01:54:07 GMT
VOLUME [/var/solr]
# Thu, 26 Aug 2021 01:54:08 GMT
EXPOSE 8983
# Thu, 26 Aug 2021 01:54:08 GMT
WORKDIR /opt/solr
# Thu, 26 Aug 2021 01:54:08 GMT
USER solr
# Thu, 26 Aug 2021 01:54:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Aug 2021 01:54:08 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:3716b9f3c2f9e7592f5b47c2e6e13e64132071620c7551e0aa3c5c248e106139`  
		Last Modified: Tue, 17 Aug 2021 01:53:29 GMT  
		Size: 30.0 MB (30048801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c8aacccebb7931a5eafbf1992d4ce71f633f062d73ac3b147a0f85c5fc090f`  
		Last Modified: Thu, 26 Aug 2021 00:50:06 GMT  
		Size: 1.6 MB (1566164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755ccaa625a123c329c7e206cb9ebf65d1c8f6072840287354fb4b7ea3987582`  
		Last Modified: Thu, 26 Aug 2021 00:56:09 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cbc77e59f773d04c7b72e3b1e2af97aa4186344be71e3b0d4808ccd964524b`  
		Last Modified: Thu, 26 Aug 2021 00:57:50 GMT  
		Size: 46.2 MB (46201784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed0200573decb49101a10178f8101ce41672670140a04f5af654d07514c0d36`  
		Last Modified: Thu, 26 Aug 2021 02:16:07 GMT  
		Size: 6.8 MB (6813779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4da246131c937f26eb74fd582c10a4e7253ae44c7b766c22f38ac6e4be954e`  
		Last Modified: Thu, 26 Aug 2021 02:16:07 GMT  
		Size: 4.3 KB (4323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ab54ed2d80a847fe35c3bf33171a4bd3cccb184e00425ee3dde22e18e53b8d`  
		Last Modified: Thu, 26 Aug 2021 02:16:06 GMT  
		Size: 2.9 KB (2925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7070ef7688c9436e47a7ea7282d5320e0320598a2816999e496e23a9414e7b6d`  
		Last Modified: Thu, 26 Aug 2021 02:16:19 GMT  
		Size: 203.1 MB (203088478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d61e45c5d350939b5f97c8b42ec058e9d709f381b64e894dc5656d04f12485b`  
		Last Modified: Thu, 26 Aug 2021 02:16:06 GMT  
		Size: 6.3 KB (6276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
