## `solr:latest`

```console
$ docker pull solr@sha256:e66f86993770de10f89659aa8b48b99ae8899c39c6305bd98159b83e4d5bf805
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `solr:latest` - linux; amd64

```console
$ docker pull solr@sha256:babaf4deaeb0d033e55f1b4b9383b241d000b381f4d2000d5164682af526aee5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.6 MB (319577948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ba0efd00cde85145824ac19401e3dfd70ebdcd019b9695c866c44e0aa81e79c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:40 GMT
ADD file:8f75f11b2bd2d50e5912359ae750de06a7b49506df3756c19baf4cc63d900c4f in / 
# Tue, 09 Feb 2021 02:20:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:35:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:35:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Mar 2021 21:03:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Mar 2021 21:03:31 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 09 Mar 2021 21:03:32 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 09 Mar 2021 21:03:32 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 21:03:32 GMT
ENV LANG=C.UTF-8
# Tue, 09 Mar 2021 21:03:32 GMT
ENV JAVA_VERSION=11.0.10
# Tue, 09 Mar 2021 21:03:39 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jre_x64_linux_11.0.10_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jre_aarch64_linux_11.0.10_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 09 Mar 2021 23:26:19 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Tue, 09 Mar 2021 23:26:20 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Tue, 09 Mar 2021 23:26:20 GMT
ARG SOLR_VERSION=8.8.1
# Tue, 09 Mar 2021 23:26:20 GMT
ARG SOLR_SHA512=a13ad0f8d67e6465d01bd50b9965a042849395e84024cd1093f9e44b9c602ab43b7bbc2f2bc5c1161178ac6bb0c3f717573c69d51baf0aa8f97fb8b5a97a9ffd
# Tue, 09 Mar 2021 23:26:20 GMT
ARG SOLR_KEYS=fbc25d7e1712025294fe66590a6aa179b9bbf45e
# Tue, 09 Mar 2021 23:26:20 GMT
ARG SOLR_DOWNLOAD_URL
# Tue, 09 Mar 2021 23:26:21 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 09 Mar 2021 23:26:27 GMT
# ARGS: SOLR_KEYS=fbc25d7e1712025294fe66590a6aa179b9bbf45e SOLR_SHA512=a13ad0f8d67e6465d01bd50b9965a042849395e84024cd1093f9e44b9c602ab43b7bbc2f2bc5c1161178ac6bb0c3f717573c69d51baf0aa8f97fb8b5a97a9ffd SOLR_VERSION=8.8.1
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Tue, 09 Mar 2021 23:26:27 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.8.1/solr-8.8.1.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.8.1/solr-8.8.1.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.8.1/solr-8.8.1.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Tue, 09 Mar 2021 23:26:28 GMT
# ARGS: SOLR_KEYS=fbc25d7e1712025294fe66590a6aa179b9bbf45e SOLR_SHA512=a13ad0f8d67e6465d01bd50b9965a042849395e84024cd1093f9e44b9c602ab43b7bbc2f2bc5c1161178ac6bb0c3f717573c69d51baf0aa8f97fb8b5a97a9ffd SOLR_VERSION=8.8.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 09 Mar 2021 23:26:37 GMT
# ARGS: SOLR_KEYS=fbc25d7e1712025294fe66590a6aa179b9bbf45e SOLR_SHA512=a13ad0f8d67e6465d01bd50b9965a042849395e84024cd1093f9e44b9c602ab43b7bbc2f2bc5c1161178ac6bb0c3f717573c69d51baf0aa8f97fb8b5a97a9ffd SOLR_VERSION=8.8.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Tue, 09 Mar 2021 23:27:07 GMT
# ARGS: SOLR_KEYS=fbc25d7e1712025294fe66590a6aa179b9bbf45e SOLR_SHA512=a13ad0f8d67e6465d01bd50b9965a042849395e84024cd1093f9e44b9c602ab43b7bbc2f2bc5c1161178ac6bb0c3f717573c69d51baf0aa8f97fb8b5a97a9ffd SOLR_VERSION=8.8.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Tue, 09 Mar 2021 23:27:08 GMT
COPY --chown=0:0dir:9bc5f3733a819401f8f06067a2f41713605d2c3bb03bbbe92d04dc2f83bd0265 in /opt/docker-solr/scripts 
# Tue, 09 Mar 2021 23:27:08 GMT
VOLUME [/var/solr]
# Tue, 09 Mar 2021 23:27:08 GMT
EXPOSE 8983
# Tue, 09 Mar 2021 23:27:08 GMT
WORKDIR /opt/solr
# Tue, 09 Mar 2021 23:27:09 GMT
USER solr
# Tue, 09 Mar 2021 23:27:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Mar 2021 23:27:09 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:0ecb575e629cd60aa802266a3bc6847dcf4073aa2a6d7d43f717dd61e7b90e0b`  
		Last Modified: Tue, 09 Feb 2021 02:26:22 GMT  
		Size: 50.4 MB (50400198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7467d1831b6947c294d92ee957902c3cd448b17c5ac2103ca5e79d15afb317c3`  
		Last Modified: Tue, 09 Feb 2021 04:46:00 GMT  
		Size: 7.8 MB (7830684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feab2c490a3cea21cc051ff29c33cc9857418edfa1be9966124b18abe1d5ae16`  
		Last Modified: Tue, 09 Feb 2021 04:46:00 GMT  
		Size: 10.0 MB (9996459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5172d94a54209847ce8f9621e3df148c1877f3f3c8693e93ecab275675156613`  
		Last Modified: Tue, 09 Mar 2021 21:22:01 GMT  
		Size: 5.5 MB (5531076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368beafa1bca8a199f43f2f276b93b55d49b1fe29a79ba76bc5fb794d227959b`  
		Last Modified: Tue, 09 Mar 2021 21:22:00 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f698cd6a7a8277057205b459a776323595a9ea435da25bf1f7a76ddc4570169`  
		Last Modified: Tue, 09 Mar 2021 21:22:07 GMT  
		Size: 46.8 MB (46761774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c352046b83c9f9d0063c15d859dbbf8f7540609c957c99113403a49fba12ae`  
		Last Modified: Wed, 10 Mar 2021 00:01:32 GMT  
		Size: 2.5 MB (2546141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2befb4c6bbd65267bc2f5cc7fc55f82764946eb8e35c014d911fb89a6f73c3c7`  
		Last Modified: Wed, 10 Mar 2021 00:01:32 GMT  
		Size: 4.3 KB (4288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ce58665d9e67d215c2a161ec24e02b0f271bc39bb7b018f4e05f9d1e1a3cb1`  
		Last Modified: Wed, 10 Mar 2021 00:01:32 GMT  
		Size: 2.9 KB (2928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba64dd9a2c39b3e8f231fa55bf20cb36f3fb2843284038c19b0f91c55256e50`  
		Last Modified: Wed, 10 Mar 2021 00:01:45 GMT  
		Size: 196.5 MB (196497910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c933edcd184ea1040a0dacaed5d29c8710cfa122bf17f5c7960b13baaa0d96b`  
		Last Modified: Wed, 10 Mar 2021 00:01:32 GMT  
		Size: 6.3 KB (6277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:latest` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:667fb5ff00d9ccc1ad50206184e562edb67f28b0dbb92d504a7ad368f28a64c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.2 MB (317182609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:699c6026e4604b6ad1218a033337e0708986cf113f4cc9d09bbf98decb6c82e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Tue, 09 Feb 2021 02:40:45 GMT
ADD file:78412ee35e3dc6fb5fdfce41eb05dd273ba1d49328ab327465639bfa4821aa51 in / 
# Tue, 09 Feb 2021 02:40:50 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:43:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:43:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 07:18:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 07:18:30 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 09 Feb 2021 07:18:32 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 09 Feb 2021 07:18:33 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 07:18:33 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 07:18:34 GMT
ENV JAVA_VERSION=11.0.10
# Tue, 09 Feb 2021 07:18:42 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jre_x64_linux_11.0.10_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jre_aarch64_linux_11.0.10_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Wed, 10 Feb 2021 03:13:43 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 10 Feb 2021 03:13:43 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Fri, 26 Feb 2021 22:20:24 GMT
ARG SOLR_VERSION=8.8.1
# Fri, 26 Feb 2021 22:20:24 GMT
ARG SOLR_SHA512=a13ad0f8d67e6465d01bd50b9965a042849395e84024cd1093f9e44b9c602ab43b7bbc2f2bc5c1161178ac6bb0c3f717573c69d51baf0aa8f97fb8b5a97a9ffd
# Fri, 26 Feb 2021 22:20:25 GMT
ARG SOLR_KEYS=fbc25d7e1712025294fe66590a6aa179b9bbf45e
# Fri, 26 Feb 2021 22:20:26 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 26 Feb 2021 22:20:27 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 26 Feb 2021 22:20:40 GMT
# ARGS: SOLR_KEYS=fbc25d7e1712025294fe66590a6aa179b9bbf45e SOLR_SHA512=a13ad0f8d67e6465d01bd50b9965a042849395e84024cd1093f9e44b9c602ab43b7bbc2f2bc5c1161178ac6bb0c3f717573c69d51baf0aa8f97fb8b5a97a9ffd SOLR_VERSION=8.8.1
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Fri, 26 Feb 2021 22:20:41 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.8.1/solr-8.8.1.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.8.1/solr-8.8.1.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.8.1/solr-8.8.1.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Fri, 26 Feb 2021 22:20:46 GMT
# ARGS: SOLR_KEYS=fbc25d7e1712025294fe66590a6aa179b9bbf45e SOLR_SHA512=a13ad0f8d67e6465d01bd50b9965a042849395e84024cd1093f9e44b9c602ab43b7bbc2f2bc5c1161178ac6bb0c3f717573c69d51baf0aa8f97fb8b5a97a9ffd SOLR_VERSION=8.8.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 26 Feb 2021 22:20:49 GMT
# ARGS: SOLR_KEYS=fbc25d7e1712025294fe66590a6aa179b9bbf45e SOLR_SHA512=a13ad0f8d67e6465d01bd50b9965a042849395e84024cd1093f9e44b9c602ab43b7bbc2f2bc5c1161178ac6bb0c3f717573c69d51baf0aa8f97fb8b5a97a9ffd SOLR_VERSION=8.8.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 26 Feb 2021 22:21:08 GMT
# ARGS: SOLR_KEYS=fbc25d7e1712025294fe66590a6aa179b9bbf45e SOLR_SHA512=a13ad0f8d67e6465d01bd50b9965a042849395e84024cd1093f9e44b9c602ab43b7bbc2f2bc5c1161178ac6bb0c3f717573c69d51baf0aa8f97fb8b5a97a9ffd SOLR_VERSION=8.8.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Fri, 26 Feb 2021 22:21:09 GMT
COPY --chown=0:0dir:9bc5f3733a819401f8f06067a2f41713605d2c3bb03bbbe92d04dc2f83bd0265 in /opt/docker-solr/scripts 
# Fri, 26 Feb 2021 22:21:10 GMT
VOLUME [/var/solr]
# Fri, 26 Feb 2021 22:21:11 GMT
EXPOSE 8983
# Fri, 26 Feb 2021 22:21:12 GMT
WORKDIR /opt/solr
# Fri, 26 Feb 2021 22:21:13 GMT
USER solr
# Fri, 26 Feb 2021 22:21:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Feb 2021 22:21:14 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:c78c297fb0d010ee085f95ae439636ecb167b050c1acb4273bd576998cf94a83`  
		Last Modified: Tue, 09 Feb 2021 02:47:03 GMT  
		Size: 49.2 MB (49183229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06af62193c25241eb123af8cf115c7a6298e834976fe148ac79ec11a7ca06ee5`  
		Last Modified: Tue, 09 Feb 2021 04:57:24 GMT  
		Size: 7.7 MB (7694122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b846e1b73901174c506ae5e6219ac2f356ef71eaa5896dfbc238dc67ca4bf73`  
		Last Modified: Tue, 09 Feb 2021 04:57:24 GMT  
		Size: 10.0 MB (9984281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817f391a97e0a99d45450a613edd283a71494f413f3d77831db82748eeda9902`  
		Last Modified: Tue, 09 Feb 2021 07:28:28 GMT  
		Size: 5.5 MB (5505574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0d3c30165d4e92e97bbd1950f06a292a5674037e6314b842268aa4786914dd`  
		Last Modified: Tue, 09 Feb 2021 07:28:27 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344dbb60943bcb0e83429751f15d3562db6342eab7cc173311ca8349565cb70d`  
		Last Modified: Tue, 09 Feb 2021 07:28:38 GMT  
		Size: 45.8 MB (45839909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06b016d5ef478ca87f582cec01ec5b7070fd6b6f8228c0d969f2a6df189713a`  
		Last Modified: Fri, 26 Feb 2021 22:24:39 GMT  
		Size: 2.5 MB (2463991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d37bdff40f7a07ce2d67bcc97d5e3f54be1ddd2276aeb5055483d9205426f63`  
		Last Modified: Fri, 26 Feb 2021 22:24:38 GMT  
		Size: 4.3 KB (4321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfde097f997fcb5829f359d1672239d6c1d294ff33a0aa9ddc232a4c82adcb6`  
		Last Modified: Fri, 26 Feb 2021 22:24:38 GMT  
		Size: 2.9 KB (2919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab815f3813eed05ecb121fedb7e676d180b5f0ad2fa3bc572de62c8b8f11bef3`  
		Last Modified: Fri, 26 Feb 2021 22:24:59 GMT  
		Size: 196.5 MB (196497778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f449fb1cf3159772f35655fe65a3fc0ae3fdbdfc2958902c898d3ed7d28e489`  
		Last Modified: Fri, 26 Feb 2021 22:24:38 GMT  
		Size: 6.3 KB (6274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
