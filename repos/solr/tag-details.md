<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `solr`

-	[`solr:8`](#solr8)
-	[`solr:8-slim`](#solr8-slim)
-	[`solr:8.11`](#solr811)
-	[`solr:8.11-slim`](#solr811-slim)
-	[`solr:8.11.1`](#solr8111)
-	[`solr:8.11.1-slim`](#solr8111-slim)
-	[`solr:9`](#solr9)
-	[`solr:9.0`](#solr90)
-	[`solr:9.0.0`](#solr900)
-	[`solr:latest`](#solrlatest)

## `solr:8`

```console
$ docker pull solr@sha256:3a133043d41bd2e5cbcba254c55a411b69dd253d5e2d8c89cf2c73a19787f7c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `solr:8` - linux; amd64

```console
$ docker pull solr@sha256:2c66975dcafca15d30e81108df32884e008be50b149204f23974fe7667193235
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.5 MB (345521177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b151d8eb0f3a56f030c01fd51525857594d567f754dd506355fc10708299f6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 11 May 2022 01:20:05 GMT
ADD file:68a5d7d0db592625159865110c1b7dcb15cf70ecf71b5fd541ef89584cd734ba in / 
# Wed, 11 May 2022 01:20:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:49:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 05:51:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:51:22 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 11 May 2022 05:51:23 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 11 May 2022 05:51:23 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 05:51:23 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 05:51:23 GMT
ENV JAVA_VERSION=11.0.15
# Wed, 11 May 2022 05:51:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_linux_11.0.15_10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_aarch64_linux_11.0.15_10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Wed, 11 May 2022 22:57:04 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 11 May 2022 22:57:04 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 11 May 2022 22:57:04 GMT
ARG SOLR_VERSION=8.11.1
# Wed, 11 May 2022 22:57:04 GMT
ARG SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45
# Wed, 11 May 2022 22:57:04 GMT
ARG SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E
# Wed, 11 May 2022 22:57:04 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 11 May 2022 22:57:04 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 11 May 2022 22:57:10 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 11 May 2022 22:57:10 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.1/solr-8.11.1.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 11 May 2022 22:57:10 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 11 May 2022 22:57:46 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 11 May 2022 22:58:17 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 11 May 2022 22:58:18 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 11 May 2022 22:58:18 GMT
VOLUME [/var/solr]
# Wed, 11 May 2022 22:58:18 GMT
EXPOSE 8983
# Wed, 11 May 2022 22:58:18 GMT
WORKDIR /opt/solr
# Wed, 11 May 2022 22:58:18 GMT
USER solr
# Wed, 11 May 2022 22:58:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 22:58:18 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:67e8aa6c8bbc76b1f2bccb3864b0887671833b8667dc1f6c965fcb0eac7e6402`  
		Last Modified: Wed, 11 May 2022 01:24:45 GMT  
		Size: 54.9 MB (54945622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627e6c1e105548ea4a08354eea581f137cf368d91aeb0ad47dcb706fca54fd8b`  
		Last Modified: Wed, 11 May 2022 01:57:17 GMT  
		Size: 5.2 MB (5155721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0670968926f6461e3135c82ba2c0ad3ebdedc0d0f41b18bda4a1e41104b8be8a`  
		Last Modified: Wed, 11 May 2022 01:57:18 GMT  
		Size: 10.9 MB (10875052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e458027cc21c1550d8d2ca4b36cd45889abb22dc7945f460014254e4276c6a`  
		Last Modified: Wed, 11 May 2022 06:06:24 GMT  
		Size: 5.7 MB (5657524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e07b100903dfabd0c5ee512f754810fee8af4d6189459d873c8753a98663ad7`  
		Last Modified: Wed, 11 May 2022 06:06:23 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf92622a61b817a7696e452f66d238710c0e7722f6fed7d0d8f4e224762a0a5`  
		Last Modified: Wed, 11 May 2022 06:06:30 GMT  
		Size: 47.2 MB (47198730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c21cd57394c4aab15f163ea13538ce93e223bd50181806a200ac3dc6e0bcdba`  
		Last Modified: Wed, 11 May 2022 23:35:41 GMT  
		Size: 3.4 MB (3440458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d608fa7995a4a6b0bbcac190fe189146e2a1394f814f05214a48a22dc74b9fd9`  
		Last Modified: Wed, 11 May 2022 23:35:40 GMT  
		Size: 4.3 KB (4282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962d92982b4e8a2b8bc05b817c6696a223e7334b9c4ec3445baf4685d8b0f323`  
		Last Modified: Wed, 11 May 2022 23:35:40 GMT  
		Size: 5.1 KB (5110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dbccb2ac1e6766c99230255ce612d47e3ebcdb0ca992b85f3963b3d967e9dc4`  
		Last Modified: Wed, 11 May 2022 23:35:51 GMT  
		Size: 218.2 MB (218232160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1d95c484d02d8496add3cfec66efaa1ea314e323673ea10eb415cb4efb018e`  
		Last Modified: Wed, 11 May 2022 23:35:40 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:ad074897320306b910603f21996d0aea3e4174a0082308f06254d73a02ec2345
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.7 MB (342743504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5301008b13d28ce3eeb395e6b0e41662bcd1beb222cb624cc7efd68e756d32d4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 11 May 2022 00:46:44 GMT
ADD file:239aa42118877a929b2fbfc0d5793fee7815289280affa5286de2459385c0679 in / 
# Wed, 11 May 2022 00:46:44 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:25:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:25:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 14:22:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:22:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 11 May 2022 14:22:12 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 11 May 2022 14:22:13 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 14:22:14 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 14:22:15 GMT
ENV JAVA_VERSION=11.0.15
# Wed, 11 May 2022 14:22:23 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_linux_11.0.15_10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_aarch64_linux_11.0.15_10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 12 May 2022 02:12:07 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Thu, 12 May 2022 02:12:08 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Thu, 12 May 2022 02:12:09 GMT
ARG SOLR_VERSION=8.11.1
# Thu, 12 May 2022 02:12:10 GMT
ARG SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45
# Thu, 12 May 2022 02:12:11 GMT
ARG SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E
# Thu, 12 May 2022 02:12:12 GMT
ARG SOLR_DOWNLOAD_URL
# Thu, 12 May 2022 02:12:13 GMT
ARG SOLR_DOWNLOAD_SERVER
# Thu, 12 May 2022 02:12:19 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Thu, 12 May 2022 02:12:19 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.1/solr-8.11.1.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Thu, 12 May 2022 02:12:20 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Thu, 12 May 2022 02:13:04 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Thu, 12 May 2022 02:13:26 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Thu, 12 May 2022 02:13:27 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Thu, 12 May 2022 02:13:27 GMT
VOLUME [/var/solr]
# Thu, 12 May 2022 02:13:28 GMT
EXPOSE 8983
# Thu, 12 May 2022 02:13:29 GMT
WORKDIR /opt/solr
# Thu, 12 May 2022 02:13:30 GMT
USER solr
# Thu, 12 May 2022 02:13:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 02:13:32 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:3a36574378e6cece2dd3a839e1c0220eaccc4063b61d7481d1a19d3990c1f2c2`  
		Last Modified: Wed, 11 May 2022 00:53:15 GMT  
		Size: 53.6 MB (53634337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61d3345afba43846f3e638752cce2f0d1d47b21cc667ba08b00db10767a4702`  
		Last Modified: Wed, 11 May 2022 01:35:45 GMT  
		Size: 4.9 MB (4938615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e267d6aa58f93a513352a3b46c7addbf9335d7d43bfa4f1df4026d21785181c`  
		Last Modified: Wed, 11 May 2022 01:35:46 GMT  
		Size: 10.7 MB (10656992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5439fd20344c5c55f97bb56a04aa465872f8e2580137cb005195d35936950f75`  
		Last Modified: Wed, 11 May 2022 14:43:42 GMT  
		Size: 5.6 MB (5649585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f268ed86b71d7954ee3fa8233dae25af56b71c45c319d1bd7bcd8a65818a53d8`  
		Last Modified: Wed, 11 May 2022 14:43:41 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653e0946e82da4e55efe283bc854acbcfe8f7321b34506c3626dffa425a29e88`  
		Last Modified: Wed, 11 May 2022 14:43:48 GMT  
		Size: 46.5 MB (46498919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e64b26b31a3b36082a2312d52f264100b8e01eb695953eb7dd62397bd27e6f`  
		Last Modified: Thu, 12 May 2022 02:52:31 GMT  
		Size: 3.1 MB (3118706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba7694645a7d23e85e21e795ce09f3b7280e453b7d95e3e1df7ded45f0fae90`  
		Last Modified: Thu, 12 May 2022 02:52:30 GMT  
		Size: 4.2 KB (4195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9e55d39f6468a4201ff5f50ff67994050bfd9135b7c4c0e337017bcd90e491`  
		Last Modified: Thu, 12 May 2022 02:52:30 GMT  
		Size: 5.1 KB (5077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b6974f7a28b470f103307aa391536457a06544ef4da72fd75a2d25d62675d5`  
		Last Modified: Thu, 12 May 2022 02:52:45 GMT  
		Size: 218.2 MB (218230586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a13ee434d2f0014ff89e01b98f97486e31fe8ccab220fb76c390111d80c94f`  
		Last Modified: Thu, 12 May 2022 02:52:30 GMT  
		Size: 6.3 KB (6281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:8-slim`

```console
$ docker pull solr@sha256:90850c834781d0bb756109bb7c8c6c092c2dd7d2e5fd46ff4efdd1caa258b251
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `solr:8-slim` - linux; amd64

```console
$ docker pull solr@sha256:4dcdadfa9e3df84930a0f2beebf26967b12d33b531378d17d8445add24307190
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.6 MB (305584248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83185b7bb0a2aa673dab74180435844d6f9421034a18a31c195f3d8e538d945f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:46:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:49:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 11 May 2022 05:49:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 11 May 2022 05:49:49 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 05:49:50 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 05:49:50 GMT
ENV JAVA_VERSION=11.0.15
# Wed, 11 May 2022 05:51:46 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_linux_11.0.15_10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_aarch64_linux_11.0.15_10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Wed, 11 May 2022 22:58:27 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 11 May 2022 22:58:27 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 11 May 2022 22:58:27 GMT
ARG SOLR_VERSION=8.11.1
# Wed, 11 May 2022 22:58:27 GMT
ARG SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45
# Wed, 11 May 2022 22:58:27 GMT
ARG SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E
# Wed, 11 May 2022 22:58:27 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 11 May 2022 22:58:27 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 11 May 2022 22:58:34 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 11 May 2022 22:58:35 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.1/solr-8.11.1.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 11 May 2022 22:58:35 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 11 May 2022 22:59:14 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 11 May 2022 22:59:47 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 11 May 2022 22:59:47 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 11 May 2022 22:59:47 GMT
VOLUME [/var/solr]
# Wed, 11 May 2022 22:59:47 GMT
EXPOSE 8983
# Wed, 11 May 2022 22:59:48 GMT
WORKDIR /opt/solr
# Wed, 11 May 2022 22:59:48 GMT
USER solr
# Wed, 11 May 2022 22:59:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 22:59:48 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf31789c5c1a5e3676cbd7a34472d61217c52c819552f5b116565c22cb6d2f1`  
		Last Modified: Wed, 11 May 2022 05:58:33 GMT  
		Size: 1.6 MB (1582150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8741521b2ba4d4d676c7a992cb54627c0eb9fdce1b4f68ad17da4f8b2abf103a`  
		Last Modified: Wed, 11 May 2022 06:04:24 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e6176efc301cb3ae865b2acdb15a1442271368cc6e37ed5295b98a86430071`  
		Last Modified: Wed, 11 May 2022 06:06:50 GMT  
		Size: 47.5 MB (47471986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b5ac43518e9969d5fa6bce2c2bccf79f1651094adff450e1304154b7f06b49`  
		Last Modified: Wed, 11 May 2022 23:36:08 GMT  
		Size: 6.9 MB (6902627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19d70a1a092e0ea180a3f36d8e03b3d669593a13a052fb9c2576f1b3def4ead`  
		Last Modified: Wed, 11 May 2022 23:36:07 GMT  
		Size: 4.3 KB (4281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92949b24285df742f1bd9cf1c0e4a12f313db2aba9a3d5a640c252861d0f2b3b`  
		Last Modified: Wed, 11 May 2022 23:36:06 GMT  
		Size: 5.1 KB (5114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0dfe027ca64e0579cdc691c8f744566a30c04558a8bf63fccb69de07087fc4c`  
		Last Modified: Wed, 11 May 2022 23:36:17 GMT  
		Size: 218.2 MB (218232096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc735747472c30e7f84ef0a12e67e3c73c44584fe96a5a8da88c2caba82457f`  
		Last Modified: Wed, 11 May 2022 23:36:07 GMT  
		Size: 6.3 KB (6307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8-slim` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:dc875016e82139d6745ac84496d5082e26c643e0ef889fda05694999d522fc84
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.8 MB (302830559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e69f69fd8b937c4c00e381dd43d27b23676275a893409dabb448006c7e7b4d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 14:15:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:20:16 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 11 May 2022 14:20:17 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 11 May 2022 14:20:18 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 14:20:19 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 14:20:20 GMT
ENV JAVA_VERSION=11.0.15
# Wed, 11 May 2022 14:22:40 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_linux_11.0.15_10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_aarch64_linux_11.0.15_10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 12 May 2022 02:13:49 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Thu, 12 May 2022 02:13:50 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Thu, 12 May 2022 02:13:51 GMT
ARG SOLR_VERSION=8.11.1
# Thu, 12 May 2022 02:13:52 GMT
ARG SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45
# Thu, 12 May 2022 02:13:53 GMT
ARG SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E
# Thu, 12 May 2022 02:13:54 GMT
ARG SOLR_DOWNLOAD_URL
# Thu, 12 May 2022 02:13:55 GMT
ARG SOLR_DOWNLOAD_SERVER
# Thu, 12 May 2022 02:14:03 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Thu, 12 May 2022 02:14:04 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.1/solr-8.11.1.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Thu, 12 May 2022 02:14:05 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Thu, 12 May 2022 02:14:47 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Thu, 12 May 2022 02:15:08 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Thu, 12 May 2022 02:15:09 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Thu, 12 May 2022 02:15:09 GMT
VOLUME [/var/solr]
# Thu, 12 May 2022 02:15:10 GMT
EXPOSE 8983
# Thu, 12 May 2022 02:15:11 GMT
WORKDIR /opt/solr
# Thu, 12 May 2022 02:15:12 GMT
USER solr
# Thu, 12 May 2022 02:15:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 02:15:14 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5ad7be01b68fe78dada799da391fe706a6e51b7a0ec158e40069f53de08619`  
		Last Modified: Wed, 11 May 2022 14:33:48 GMT  
		Size: 1.4 MB (1361175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8acb5edbf912b614d8422de4c52b9ce05abfd1b213fa1f211981f0ccf726f18`  
		Last Modified: Wed, 11 May 2022 14:41:15 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41aadabd6a0e6ee394320c2556bde036004cb45c3964dd1b8c52f66d5ec6243f`  
		Last Modified: Wed, 11 May 2022 14:44:09 GMT  
		Size: 46.6 MB (46556265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af9311ee2ee7548e3de146bcb122287367b75977a1f043fd084685818a3df70`  
		Last Modified: Thu, 12 May 2022 02:53:04 GMT  
		Size: 6.6 MB (6601115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e31e7ea7dbdba328836874b1a82f7e0f4b55e12e85595f4040e3d8bceaf56c7`  
		Last Modified: Thu, 12 May 2022 02:53:03 GMT  
		Size: 4.2 KB (4194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c30f84e7368e8984f717c947b94d2ff43d896bf5b882bf41d69d39ea91069e`  
		Last Modified: Thu, 12 May 2022 02:53:03 GMT  
		Size: 5.1 KB (5079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ee99a189e42f73c21a4343dbb66791ca5c11aaae7e1a003bb7e3c2bd025211`  
		Last Modified: Thu, 12 May 2022 02:53:23 GMT  
		Size: 218.2 MB (218230545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693fdb26574ff1ceb75c54cdf8c6e83253c08f9d8d9d134517afe62e1c380b1a`  
		Last Modified: Thu, 12 May 2022 02:53:03 GMT  
		Size: 6.3 KB (6281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:8.11`

```console
$ docker pull solr@sha256:3a133043d41bd2e5cbcba254c55a411b69dd253d5e2d8c89cf2c73a19787f7c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `solr:8.11` - linux; amd64

```console
$ docker pull solr@sha256:2c66975dcafca15d30e81108df32884e008be50b149204f23974fe7667193235
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.5 MB (345521177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b151d8eb0f3a56f030c01fd51525857594d567f754dd506355fc10708299f6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 11 May 2022 01:20:05 GMT
ADD file:68a5d7d0db592625159865110c1b7dcb15cf70ecf71b5fd541ef89584cd734ba in / 
# Wed, 11 May 2022 01:20:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:49:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 05:51:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:51:22 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 11 May 2022 05:51:23 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 11 May 2022 05:51:23 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 05:51:23 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 05:51:23 GMT
ENV JAVA_VERSION=11.0.15
# Wed, 11 May 2022 05:51:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_linux_11.0.15_10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_aarch64_linux_11.0.15_10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Wed, 11 May 2022 22:57:04 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 11 May 2022 22:57:04 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 11 May 2022 22:57:04 GMT
ARG SOLR_VERSION=8.11.1
# Wed, 11 May 2022 22:57:04 GMT
ARG SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45
# Wed, 11 May 2022 22:57:04 GMT
ARG SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E
# Wed, 11 May 2022 22:57:04 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 11 May 2022 22:57:04 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 11 May 2022 22:57:10 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 11 May 2022 22:57:10 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.1/solr-8.11.1.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 11 May 2022 22:57:10 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 11 May 2022 22:57:46 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 11 May 2022 22:58:17 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 11 May 2022 22:58:18 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 11 May 2022 22:58:18 GMT
VOLUME [/var/solr]
# Wed, 11 May 2022 22:58:18 GMT
EXPOSE 8983
# Wed, 11 May 2022 22:58:18 GMT
WORKDIR /opt/solr
# Wed, 11 May 2022 22:58:18 GMT
USER solr
# Wed, 11 May 2022 22:58:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 22:58:18 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:67e8aa6c8bbc76b1f2bccb3864b0887671833b8667dc1f6c965fcb0eac7e6402`  
		Last Modified: Wed, 11 May 2022 01:24:45 GMT  
		Size: 54.9 MB (54945622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627e6c1e105548ea4a08354eea581f137cf368d91aeb0ad47dcb706fca54fd8b`  
		Last Modified: Wed, 11 May 2022 01:57:17 GMT  
		Size: 5.2 MB (5155721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0670968926f6461e3135c82ba2c0ad3ebdedc0d0f41b18bda4a1e41104b8be8a`  
		Last Modified: Wed, 11 May 2022 01:57:18 GMT  
		Size: 10.9 MB (10875052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e458027cc21c1550d8d2ca4b36cd45889abb22dc7945f460014254e4276c6a`  
		Last Modified: Wed, 11 May 2022 06:06:24 GMT  
		Size: 5.7 MB (5657524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e07b100903dfabd0c5ee512f754810fee8af4d6189459d873c8753a98663ad7`  
		Last Modified: Wed, 11 May 2022 06:06:23 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf92622a61b817a7696e452f66d238710c0e7722f6fed7d0d8f4e224762a0a5`  
		Last Modified: Wed, 11 May 2022 06:06:30 GMT  
		Size: 47.2 MB (47198730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c21cd57394c4aab15f163ea13538ce93e223bd50181806a200ac3dc6e0bcdba`  
		Last Modified: Wed, 11 May 2022 23:35:41 GMT  
		Size: 3.4 MB (3440458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d608fa7995a4a6b0bbcac190fe189146e2a1394f814f05214a48a22dc74b9fd9`  
		Last Modified: Wed, 11 May 2022 23:35:40 GMT  
		Size: 4.3 KB (4282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962d92982b4e8a2b8bc05b817c6696a223e7334b9c4ec3445baf4685d8b0f323`  
		Last Modified: Wed, 11 May 2022 23:35:40 GMT  
		Size: 5.1 KB (5110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dbccb2ac1e6766c99230255ce612d47e3ebcdb0ca992b85f3963b3d967e9dc4`  
		Last Modified: Wed, 11 May 2022 23:35:51 GMT  
		Size: 218.2 MB (218232160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1d95c484d02d8496add3cfec66efaa1ea314e323673ea10eb415cb4efb018e`  
		Last Modified: Wed, 11 May 2022 23:35:40 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:ad074897320306b910603f21996d0aea3e4174a0082308f06254d73a02ec2345
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.7 MB (342743504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5301008b13d28ce3eeb395e6b0e41662bcd1beb222cb624cc7efd68e756d32d4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 11 May 2022 00:46:44 GMT
ADD file:239aa42118877a929b2fbfc0d5793fee7815289280affa5286de2459385c0679 in / 
# Wed, 11 May 2022 00:46:44 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:25:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:25:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 14:22:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:22:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 11 May 2022 14:22:12 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 11 May 2022 14:22:13 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 14:22:14 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 14:22:15 GMT
ENV JAVA_VERSION=11.0.15
# Wed, 11 May 2022 14:22:23 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_linux_11.0.15_10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_aarch64_linux_11.0.15_10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 12 May 2022 02:12:07 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Thu, 12 May 2022 02:12:08 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Thu, 12 May 2022 02:12:09 GMT
ARG SOLR_VERSION=8.11.1
# Thu, 12 May 2022 02:12:10 GMT
ARG SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45
# Thu, 12 May 2022 02:12:11 GMT
ARG SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E
# Thu, 12 May 2022 02:12:12 GMT
ARG SOLR_DOWNLOAD_URL
# Thu, 12 May 2022 02:12:13 GMT
ARG SOLR_DOWNLOAD_SERVER
# Thu, 12 May 2022 02:12:19 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Thu, 12 May 2022 02:12:19 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.1/solr-8.11.1.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Thu, 12 May 2022 02:12:20 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Thu, 12 May 2022 02:13:04 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Thu, 12 May 2022 02:13:26 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Thu, 12 May 2022 02:13:27 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Thu, 12 May 2022 02:13:27 GMT
VOLUME [/var/solr]
# Thu, 12 May 2022 02:13:28 GMT
EXPOSE 8983
# Thu, 12 May 2022 02:13:29 GMT
WORKDIR /opt/solr
# Thu, 12 May 2022 02:13:30 GMT
USER solr
# Thu, 12 May 2022 02:13:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 02:13:32 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:3a36574378e6cece2dd3a839e1c0220eaccc4063b61d7481d1a19d3990c1f2c2`  
		Last Modified: Wed, 11 May 2022 00:53:15 GMT  
		Size: 53.6 MB (53634337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61d3345afba43846f3e638752cce2f0d1d47b21cc667ba08b00db10767a4702`  
		Last Modified: Wed, 11 May 2022 01:35:45 GMT  
		Size: 4.9 MB (4938615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e267d6aa58f93a513352a3b46c7addbf9335d7d43bfa4f1df4026d21785181c`  
		Last Modified: Wed, 11 May 2022 01:35:46 GMT  
		Size: 10.7 MB (10656992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5439fd20344c5c55f97bb56a04aa465872f8e2580137cb005195d35936950f75`  
		Last Modified: Wed, 11 May 2022 14:43:42 GMT  
		Size: 5.6 MB (5649585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f268ed86b71d7954ee3fa8233dae25af56b71c45c319d1bd7bcd8a65818a53d8`  
		Last Modified: Wed, 11 May 2022 14:43:41 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653e0946e82da4e55efe283bc854acbcfe8f7321b34506c3626dffa425a29e88`  
		Last Modified: Wed, 11 May 2022 14:43:48 GMT  
		Size: 46.5 MB (46498919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e64b26b31a3b36082a2312d52f264100b8e01eb695953eb7dd62397bd27e6f`  
		Last Modified: Thu, 12 May 2022 02:52:31 GMT  
		Size: 3.1 MB (3118706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba7694645a7d23e85e21e795ce09f3b7280e453b7d95e3e1df7ded45f0fae90`  
		Last Modified: Thu, 12 May 2022 02:52:30 GMT  
		Size: 4.2 KB (4195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9e55d39f6468a4201ff5f50ff67994050bfd9135b7c4c0e337017bcd90e491`  
		Last Modified: Thu, 12 May 2022 02:52:30 GMT  
		Size: 5.1 KB (5077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b6974f7a28b470f103307aa391536457a06544ef4da72fd75a2d25d62675d5`  
		Last Modified: Thu, 12 May 2022 02:52:45 GMT  
		Size: 218.2 MB (218230586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a13ee434d2f0014ff89e01b98f97486e31fe8ccab220fb76c390111d80c94f`  
		Last Modified: Thu, 12 May 2022 02:52:30 GMT  
		Size: 6.3 KB (6281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:8.11-slim`

```console
$ docker pull solr@sha256:90850c834781d0bb756109bb7c8c6c092c2dd7d2e5fd46ff4efdd1caa258b251
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `solr:8.11-slim` - linux; amd64

```console
$ docker pull solr@sha256:4dcdadfa9e3df84930a0f2beebf26967b12d33b531378d17d8445add24307190
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.6 MB (305584248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83185b7bb0a2aa673dab74180435844d6f9421034a18a31c195f3d8e538d945f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:46:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:49:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 11 May 2022 05:49:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 11 May 2022 05:49:49 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 05:49:50 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 05:49:50 GMT
ENV JAVA_VERSION=11.0.15
# Wed, 11 May 2022 05:51:46 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_linux_11.0.15_10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_aarch64_linux_11.0.15_10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Wed, 11 May 2022 22:58:27 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 11 May 2022 22:58:27 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 11 May 2022 22:58:27 GMT
ARG SOLR_VERSION=8.11.1
# Wed, 11 May 2022 22:58:27 GMT
ARG SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45
# Wed, 11 May 2022 22:58:27 GMT
ARG SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E
# Wed, 11 May 2022 22:58:27 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 11 May 2022 22:58:27 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 11 May 2022 22:58:34 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 11 May 2022 22:58:35 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.1/solr-8.11.1.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 11 May 2022 22:58:35 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 11 May 2022 22:59:14 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 11 May 2022 22:59:47 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 11 May 2022 22:59:47 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 11 May 2022 22:59:47 GMT
VOLUME [/var/solr]
# Wed, 11 May 2022 22:59:47 GMT
EXPOSE 8983
# Wed, 11 May 2022 22:59:48 GMT
WORKDIR /opt/solr
# Wed, 11 May 2022 22:59:48 GMT
USER solr
# Wed, 11 May 2022 22:59:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 22:59:48 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf31789c5c1a5e3676cbd7a34472d61217c52c819552f5b116565c22cb6d2f1`  
		Last Modified: Wed, 11 May 2022 05:58:33 GMT  
		Size: 1.6 MB (1582150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8741521b2ba4d4d676c7a992cb54627c0eb9fdce1b4f68ad17da4f8b2abf103a`  
		Last Modified: Wed, 11 May 2022 06:04:24 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e6176efc301cb3ae865b2acdb15a1442271368cc6e37ed5295b98a86430071`  
		Last Modified: Wed, 11 May 2022 06:06:50 GMT  
		Size: 47.5 MB (47471986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b5ac43518e9969d5fa6bce2c2bccf79f1651094adff450e1304154b7f06b49`  
		Last Modified: Wed, 11 May 2022 23:36:08 GMT  
		Size: 6.9 MB (6902627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19d70a1a092e0ea180a3f36d8e03b3d669593a13a052fb9c2576f1b3def4ead`  
		Last Modified: Wed, 11 May 2022 23:36:07 GMT  
		Size: 4.3 KB (4281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92949b24285df742f1bd9cf1c0e4a12f313db2aba9a3d5a640c252861d0f2b3b`  
		Last Modified: Wed, 11 May 2022 23:36:06 GMT  
		Size: 5.1 KB (5114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0dfe027ca64e0579cdc691c8f744566a30c04558a8bf63fccb69de07087fc4c`  
		Last Modified: Wed, 11 May 2022 23:36:17 GMT  
		Size: 218.2 MB (218232096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc735747472c30e7f84ef0a12e67e3c73c44584fe96a5a8da88c2caba82457f`  
		Last Modified: Wed, 11 May 2022 23:36:07 GMT  
		Size: 6.3 KB (6307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11-slim` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:dc875016e82139d6745ac84496d5082e26c643e0ef889fda05694999d522fc84
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.8 MB (302830559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e69f69fd8b937c4c00e381dd43d27b23676275a893409dabb448006c7e7b4d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 14:15:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:20:16 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 11 May 2022 14:20:17 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 11 May 2022 14:20:18 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 14:20:19 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 14:20:20 GMT
ENV JAVA_VERSION=11.0.15
# Wed, 11 May 2022 14:22:40 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_linux_11.0.15_10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_aarch64_linux_11.0.15_10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 12 May 2022 02:13:49 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Thu, 12 May 2022 02:13:50 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Thu, 12 May 2022 02:13:51 GMT
ARG SOLR_VERSION=8.11.1
# Thu, 12 May 2022 02:13:52 GMT
ARG SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45
# Thu, 12 May 2022 02:13:53 GMT
ARG SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E
# Thu, 12 May 2022 02:13:54 GMT
ARG SOLR_DOWNLOAD_URL
# Thu, 12 May 2022 02:13:55 GMT
ARG SOLR_DOWNLOAD_SERVER
# Thu, 12 May 2022 02:14:03 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Thu, 12 May 2022 02:14:04 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.1/solr-8.11.1.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Thu, 12 May 2022 02:14:05 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Thu, 12 May 2022 02:14:47 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Thu, 12 May 2022 02:15:08 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Thu, 12 May 2022 02:15:09 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Thu, 12 May 2022 02:15:09 GMT
VOLUME [/var/solr]
# Thu, 12 May 2022 02:15:10 GMT
EXPOSE 8983
# Thu, 12 May 2022 02:15:11 GMT
WORKDIR /opt/solr
# Thu, 12 May 2022 02:15:12 GMT
USER solr
# Thu, 12 May 2022 02:15:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 02:15:14 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5ad7be01b68fe78dada799da391fe706a6e51b7a0ec158e40069f53de08619`  
		Last Modified: Wed, 11 May 2022 14:33:48 GMT  
		Size: 1.4 MB (1361175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8acb5edbf912b614d8422de4c52b9ce05abfd1b213fa1f211981f0ccf726f18`  
		Last Modified: Wed, 11 May 2022 14:41:15 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41aadabd6a0e6ee394320c2556bde036004cb45c3964dd1b8c52f66d5ec6243f`  
		Last Modified: Wed, 11 May 2022 14:44:09 GMT  
		Size: 46.6 MB (46556265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af9311ee2ee7548e3de146bcb122287367b75977a1f043fd084685818a3df70`  
		Last Modified: Thu, 12 May 2022 02:53:04 GMT  
		Size: 6.6 MB (6601115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e31e7ea7dbdba328836874b1a82f7e0f4b55e12e85595f4040e3d8bceaf56c7`  
		Last Modified: Thu, 12 May 2022 02:53:03 GMT  
		Size: 4.2 KB (4194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c30f84e7368e8984f717c947b94d2ff43d896bf5b882bf41d69d39ea91069e`  
		Last Modified: Thu, 12 May 2022 02:53:03 GMT  
		Size: 5.1 KB (5079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ee99a189e42f73c21a4343dbb66791ca5c11aaae7e1a003bb7e3c2bd025211`  
		Last Modified: Thu, 12 May 2022 02:53:23 GMT  
		Size: 218.2 MB (218230545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693fdb26574ff1ceb75c54cdf8c6e83253c08f9d8d9d134517afe62e1c380b1a`  
		Last Modified: Thu, 12 May 2022 02:53:03 GMT  
		Size: 6.3 KB (6281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:8.11.1`

```console
$ docker pull solr@sha256:3a133043d41bd2e5cbcba254c55a411b69dd253d5e2d8c89cf2c73a19787f7c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `solr:8.11.1` - linux; amd64

```console
$ docker pull solr@sha256:2c66975dcafca15d30e81108df32884e008be50b149204f23974fe7667193235
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.5 MB (345521177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b151d8eb0f3a56f030c01fd51525857594d567f754dd506355fc10708299f6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 11 May 2022 01:20:05 GMT
ADD file:68a5d7d0db592625159865110c1b7dcb15cf70ecf71b5fd541ef89584cd734ba in / 
# Wed, 11 May 2022 01:20:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:49:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 05:51:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:51:22 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 11 May 2022 05:51:23 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 11 May 2022 05:51:23 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 05:51:23 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 05:51:23 GMT
ENV JAVA_VERSION=11.0.15
# Wed, 11 May 2022 05:51:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_linux_11.0.15_10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_aarch64_linux_11.0.15_10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Wed, 11 May 2022 22:57:04 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 11 May 2022 22:57:04 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 11 May 2022 22:57:04 GMT
ARG SOLR_VERSION=8.11.1
# Wed, 11 May 2022 22:57:04 GMT
ARG SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45
# Wed, 11 May 2022 22:57:04 GMT
ARG SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E
# Wed, 11 May 2022 22:57:04 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 11 May 2022 22:57:04 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 11 May 2022 22:57:10 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 11 May 2022 22:57:10 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.1/solr-8.11.1.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 11 May 2022 22:57:10 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 11 May 2022 22:57:46 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 11 May 2022 22:58:17 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 11 May 2022 22:58:18 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 11 May 2022 22:58:18 GMT
VOLUME [/var/solr]
# Wed, 11 May 2022 22:58:18 GMT
EXPOSE 8983
# Wed, 11 May 2022 22:58:18 GMT
WORKDIR /opt/solr
# Wed, 11 May 2022 22:58:18 GMT
USER solr
# Wed, 11 May 2022 22:58:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 22:58:18 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:67e8aa6c8bbc76b1f2bccb3864b0887671833b8667dc1f6c965fcb0eac7e6402`  
		Last Modified: Wed, 11 May 2022 01:24:45 GMT  
		Size: 54.9 MB (54945622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627e6c1e105548ea4a08354eea581f137cf368d91aeb0ad47dcb706fca54fd8b`  
		Last Modified: Wed, 11 May 2022 01:57:17 GMT  
		Size: 5.2 MB (5155721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0670968926f6461e3135c82ba2c0ad3ebdedc0d0f41b18bda4a1e41104b8be8a`  
		Last Modified: Wed, 11 May 2022 01:57:18 GMT  
		Size: 10.9 MB (10875052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e458027cc21c1550d8d2ca4b36cd45889abb22dc7945f460014254e4276c6a`  
		Last Modified: Wed, 11 May 2022 06:06:24 GMT  
		Size: 5.7 MB (5657524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e07b100903dfabd0c5ee512f754810fee8af4d6189459d873c8753a98663ad7`  
		Last Modified: Wed, 11 May 2022 06:06:23 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf92622a61b817a7696e452f66d238710c0e7722f6fed7d0d8f4e224762a0a5`  
		Last Modified: Wed, 11 May 2022 06:06:30 GMT  
		Size: 47.2 MB (47198730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c21cd57394c4aab15f163ea13538ce93e223bd50181806a200ac3dc6e0bcdba`  
		Last Modified: Wed, 11 May 2022 23:35:41 GMT  
		Size: 3.4 MB (3440458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d608fa7995a4a6b0bbcac190fe189146e2a1394f814f05214a48a22dc74b9fd9`  
		Last Modified: Wed, 11 May 2022 23:35:40 GMT  
		Size: 4.3 KB (4282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962d92982b4e8a2b8bc05b817c6696a223e7334b9c4ec3445baf4685d8b0f323`  
		Last Modified: Wed, 11 May 2022 23:35:40 GMT  
		Size: 5.1 KB (5110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dbccb2ac1e6766c99230255ce612d47e3ebcdb0ca992b85f3963b3d967e9dc4`  
		Last Modified: Wed, 11 May 2022 23:35:51 GMT  
		Size: 218.2 MB (218232160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1d95c484d02d8496add3cfec66efaa1ea314e323673ea10eb415cb4efb018e`  
		Last Modified: Wed, 11 May 2022 23:35:40 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11.1` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:ad074897320306b910603f21996d0aea3e4174a0082308f06254d73a02ec2345
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.7 MB (342743504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5301008b13d28ce3eeb395e6b0e41662bcd1beb222cb624cc7efd68e756d32d4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 11 May 2022 00:46:44 GMT
ADD file:239aa42118877a929b2fbfc0d5793fee7815289280affa5286de2459385c0679 in / 
# Wed, 11 May 2022 00:46:44 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:25:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:25:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 14:22:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:22:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 11 May 2022 14:22:12 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 11 May 2022 14:22:13 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 14:22:14 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 14:22:15 GMT
ENV JAVA_VERSION=11.0.15
# Wed, 11 May 2022 14:22:23 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_linux_11.0.15_10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_aarch64_linux_11.0.15_10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 12 May 2022 02:12:07 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Thu, 12 May 2022 02:12:08 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Thu, 12 May 2022 02:12:09 GMT
ARG SOLR_VERSION=8.11.1
# Thu, 12 May 2022 02:12:10 GMT
ARG SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45
# Thu, 12 May 2022 02:12:11 GMT
ARG SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E
# Thu, 12 May 2022 02:12:12 GMT
ARG SOLR_DOWNLOAD_URL
# Thu, 12 May 2022 02:12:13 GMT
ARG SOLR_DOWNLOAD_SERVER
# Thu, 12 May 2022 02:12:19 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Thu, 12 May 2022 02:12:19 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.1/solr-8.11.1.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Thu, 12 May 2022 02:12:20 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Thu, 12 May 2022 02:13:04 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Thu, 12 May 2022 02:13:26 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Thu, 12 May 2022 02:13:27 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Thu, 12 May 2022 02:13:27 GMT
VOLUME [/var/solr]
# Thu, 12 May 2022 02:13:28 GMT
EXPOSE 8983
# Thu, 12 May 2022 02:13:29 GMT
WORKDIR /opt/solr
# Thu, 12 May 2022 02:13:30 GMT
USER solr
# Thu, 12 May 2022 02:13:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 02:13:32 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:3a36574378e6cece2dd3a839e1c0220eaccc4063b61d7481d1a19d3990c1f2c2`  
		Last Modified: Wed, 11 May 2022 00:53:15 GMT  
		Size: 53.6 MB (53634337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61d3345afba43846f3e638752cce2f0d1d47b21cc667ba08b00db10767a4702`  
		Last Modified: Wed, 11 May 2022 01:35:45 GMT  
		Size: 4.9 MB (4938615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e267d6aa58f93a513352a3b46c7addbf9335d7d43bfa4f1df4026d21785181c`  
		Last Modified: Wed, 11 May 2022 01:35:46 GMT  
		Size: 10.7 MB (10656992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5439fd20344c5c55f97bb56a04aa465872f8e2580137cb005195d35936950f75`  
		Last Modified: Wed, 11 May 2022 14:43:42 GMT  
		Size: 5.6 MB (5649585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f268ed86b71d7954ee3fa8233dae25af56b71c45c319d1bd7bcd8a65818a53d8`  
		Last Modified: Wed, 11 May 2022 14:43:41 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653e0946e82da4e55efe283bc854acbcfe8f7321b34506c3626dffa425a29e88`  
		Last Modified: Wed, 11 May 2022 14:43:48 GMT  
		Size: 46.5 MB (46498919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e64b26b31a3b36082a2312d52f264100b8e01eb695953eb7dd62397bd27e6f`  
		Last Modified: Thu, 12 May 2022 02:52:31 GMT  
		Size: 3.1 MB (3118706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba7694645a7d23e85e21e795ce09f3b7280e453b7d95e3e1df7ded45f0fae90`  
		Last Modified: Thu, 12 May 2022 02:52:30 GMT  
		Size: 4.2 KB (4195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9e55d39f6468a4201ff5f50ff67994050bfd9135b7c4c0e337017bcd90e491`  
		Last Modified: Thu, 12 May 2022 02:52:30 GMT  
		Size: 5.1 KB (5077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b6974f7a28b470f103307aa391536457a06544ef4da72fd75a2d25d62675d5`  
		Last Modified: Thu, 12 May 2022 02:52:45 GMT  
		Size: 218.2 MB (218230586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a13ee434d2f0014ff89e01b98f97486e31fe8ccab220fb76c390111d80c94f`  
		Last Modified: Thu, 12 May 2022 02:52:30 GMT  
		Size: 6.3 KB (6281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:8.11.1-slim`

```console
$ docker pull solr@sha256:90850c834781d0bb756109bb7c8c6c092c2dd7d2e5fd46ff4efdd1caa258b251
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `solr:8.11.1-slim` - linux; amd64

```console
$ docker pull solr@sha256:4dcdadfa9e3df84930a0f2beebf26967b12d33b531378d17d8445add24307190
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.6 MB (305584248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83185b7bb0a2aa673dab74180435844d6f9421034a18a31c195f3d8e538d945f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:46:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:49:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 11 May 2022 05:49:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 11 May 2022 05:49:49 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 05:49:50 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 05:49:50 GMT
ENV JAVA_VERSION=11.0.15
# Wed, 11 May 2022 05:51:46 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_linux_11.0.15_10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_aarch64_linux_11.0.15_10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Wed, 11 May 2022 22:58:27 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 11 May 2022 22:58:27 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 11 May 2022 22:58:27 GMT
ARG SOLR_VERSION=8.11.1
# Wed, 11 May 2022 22:58:27 GMT
ARG SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45
# Wed, 11 May 2022 22:58:27 GMT
ARG SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E
# Wed, 11 May 2022 22:58:27 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 11 May 2022 22:58:27 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 11 May 2022 22:58:34 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 11 May 2022 22:58:35 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.1/solr-8.11.1.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 11 May 2022 22:58:35 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 11 May 2022 22:59:14 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 11 May 2022 22:59:47 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 11 May 2022 22:59:47 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Wed, 11 May 2022 22:59:47 GMT
VOLUME [/var/solr]
# Wed, 11 May 2022 22:59:47 GMT
EXPOSE 8983
# Wed, 11 May 2022 22:59:48 GMT
WORKDIR /opt/solr
# Wed, 11 May 2022 22:59:48 GMT
USER solr
# Wed, 11 May 2022 22:59:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 22:59:48 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf31789c5c1a5e3676cbd7a34472d61217c52c819552f5b116565c22cb6d2f1`  
		Last Modified: Wed, 11 May 2022 05:58:33 GMT  
		Size: 1.6 MB (1582150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8741521b2ba4d4d676c7a992cb54627c0eb9fdce1b4f68ad17da4f8b2abf103a`  
		Last Modified: Wed, 11 May 2022 06:04:24 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e6176efc301cb3ae865b2acdb15a1442271368cc6e37ed5295b98a86430071`  
		Last Modified: Wed, 11 May 2022 06:06:50 GMT  
		Size: 47.5 MB (47471986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b5ac43518e9969d5fa6bce2c2bccf79f1651094adff450e1304154b7f06b49`  
		Last Modified: Wed, 11 May 2022 23:36:08 GMT  
		Size: 6.9 MB (6902627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19d70a1a092e0ea180a3f36d8e03b3d669593a13a052fb9c2576f1b3def4ead`  
		Last Modified: Wed, 11 May 2022 23:36:07 GMT  
		Size: 4.3 KB (4281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92949b24285df742f1bd9cf1c0e4a12f313db2aba9a3d5a640c252861d0f2b3b`  
		Last Modified: Wed, 11 May 2022 23:36:06 GMT  
		Size: 5.1 KB (5114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0dfe027ca64e0579cdc691c8f744566a30c04558a8bf63fccb69de07087fc4c`  
		Last Modified: Wed, 11 May 2022 23:36:17 GMT  
		Size: 218.2 MB (218232096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc735747472c30e7f84ef0a12e67e3c73c44584fe96a5a8da88c2caba82457f`  
		Last Modified: Wed, 11 May 2022 23:36:07 GMT  
		Size: 6.3 KB (6307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8.11.1-slim` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:dc875016e82139d6745ac84496d5082e26c643e0ef889fda05694999d522fc84
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.8 MB (302830559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e69f69fd8b937c4c00e381dd43d27b23676275a893409dabb448006c7e7b4d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 14:15:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:20:16 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 11 May 2022 14:20:17 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 11 May 2022 14:20:18 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 14:20:19 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 14:20:20 GMT
ENV JAVA_VERSION=11.0.15
# Wed, 11 May 2022 14:22:40 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_linux_11.0.15_10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_aarch64_linux_11.0.15_10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 12 May 2022 02:13:49 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Thu, 12 May 2022 02:13:50 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Thu, 12 May 2022 02:13:51 GMT
ARG SOLR_VERSION=8.11.1
# Thu, 12 May 2022 02:13:52 GMT
ARG SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45
# Thu, 12 May 2022 02:13:53 GMT
ARG SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E
# Thu, 12 May 2022 02:13:54 GMT
ARG SOLR_DOWNLOAD_URL
# Thu, 12 May 2022 02:13:55 GMT
ARG SOLR_DOWNLOAD_SERVER
# Thu, 12 May 2022 02:14:03 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Thu, 12 May 2022 02:14:04 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.11.1/solr-8.11.1.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.11.1/solr-8.11.1.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Thu, 12 May 2022 02:14:05 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Thu, 12 May 2022 02:14:47 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Thu, 12 May 2022 02:15:08 GMT
# ARGS: SOLR_KEYS=2CECBFBA181601547B654B9FFA81AC8A490F538E SOLR_SHA512=4893f836aec84b03d7bfe574e59e305c03b5ede4a48020034fbe81440b8feee79e55fd9ead230e5b89b3f25124e9b56c1ddc4bb5c7f631cf4e846b9cab5f9a45 SOLR_VERSION=8.11.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Thu, 12 May 2022 02:15:09 GMT
COPY --chown=0:0dir:fa78a99fcb12fc7f149f5ca608174160823420c330ad466b81ecc42bac19f7d6 in /opt/docker-solr/scripts 
# Thu, 12 May 2022 02:15:09 GMT
VOLUME [/var/solr]
# Thu, 12 May 2022 02:15:10 GMT
EXPOSE 8983
# Thu, 12 May 2022 02:15:11 GMT
WORKDIR /opt/solr
# Thu, 12 May 2022 02:15:12 GMT
USER solr
# Thu, 12 May 2022 02:15:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 02:15:14 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5ad7be01b68fe78dada799da391fe706a6e51b7a0ec158e40069f53de08619`  
		Last Modified: Wed, 11 May 2022 14:33:48 GMT  
		Size: 1.4 MB (1361175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8acb5edbf912b614d8422de4c52b9ce05abfd1b213fa1f211981f0ccf726f18`  
		Last Modified: Wed, 11 May 2022 14:41:15 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41aadabd6a0e6ee394320c2556bde036004cb45c3964dd1b8c52f66d5ec6243f`  
		Last Modified: Wed, 11 May 2022 14:44:09 GMT  
		Size: 46.6 MB (46556265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af9311ee2ee7548e3de146bcb122287367b75977a1f043fd084685818a3df70`  
		Last Modified: Thu, 12 May 2022 02:53:04 GMT  
		Size: 6.6 MB (6601115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e31e7ea7dbdba328836874b1a82f7e0f4b55e12e85595f4040e3d8bceaf56c7`  
		Last Modified: Thu, 12 May 2022 02:53:03 GMT  
		Size: 4.2 KB (4194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c30f84e7368e8984f717c947b94d2ff43d896bf5b882bf41d69d39ea91069e`  
		Last Modified: Thu, 12 May 2022 02:53:03 GMT  
		Size: 5.1 KB (5079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ee99a189e42f73c21a4343dbb66791ca5c11aaae7e1a003bb7e3c2bd025211`  
		Last Modified: Thu, 12 May 2022 02:53:23 GMT  
		Size: 218.2 MB (218230545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693fdb26574ff1ceb75c54cdf8c6e83253c08f9d8d9d134517afe62e1c380b1a`  
		Last Modified: Thu, 12 May 2022 02:53:03 GMT  
		Size: 6.3 KB (6281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:9`

```console
$ docker pull solr@sha256:78cb909e5389ad8c2145219cd5dc26ab0be2a86035d43aafb299102f5b379023
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `solr:9` - linux; amd64

```console
$ docker pull solr@sha256:f72f67b0508995dff6202faec6cf598e5431e53adca4df0d40afc6063b9387cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.8 MB (324773439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5948c99fe303f72be967e390639935b5845cca537a84f3c0a29c4ee67dcb6529`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:22:32 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 30 Apr 2022 00:24:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:24:14 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Sat, 30 Apr 2022 00:24:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b32bf4e18a0befea32c0ff377da7a1753b91477617a9921ceb3dee6964d2799b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.3_7.tar.gz';          ;;        armhf|arm)          ESUM='fda34743f1ad8b629f42773f6519e87d13876d4b10f98b76cd47b1aa9ad18572';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.3_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='257325f38546ce34645f6e8d7e566df401c97a9ae5f107583f9ac71f0f1b04e9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.3_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6790e3995a7fb8db99974d213f750bfd1631bfc0dad9946334be34d7b78fdbee';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.3_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='446b1ac5504d51c2ff9b0cccff079be3ce800cf8c3a3f13bab07f2656aa1fd27';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.3_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 30 Apr 2022 00:24:41 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 30 Apr 2022 00:24:42 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 13 May 2022 23:27:55 GMT
ARG SOLR_VERSION=9.0.0
# Fri, 13 May 2022 23:27:55 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 13 May 2022 23:28:44 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.version=9.0.0
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 13 May 2022 23:28:45 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 13 May 2022 23:28:46 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 13 May 2022 23:28:46 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 13 May 2022 23:28:47 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 13 May 2022 23:28:56 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 13 May 2022 23:28:56 GMT
VOLUME [/var/solr]
# Fri, 13 May 2022 23:28:56 GMT
EXPOSE 8983
# Fri, 13 May 2022 23:28:56 GMT
WORKDIR /opt/solr
# Fri, 13 May 2022 23:28:56 GMT
USER solr
# Fri, 13 May 2022 23:28:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 May 2022 23:28:56 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5dc755b592da4b1124b1e234ecb462608d017290110a0193b350cec9a521e55`  
		Last Modified: Sat, 30 Apr 2022 00:27:40 GMT  
		Size: 19.8 MB (19772006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6121641ef15b3e95a1d7cf3f8ceb4230504204a59d6b3ef215d622a1390d4290`  
		Last Modified: Sat, 30 Apr 2022 00:28:12 GMT  
		Size: 46.8 MB (46840983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd235344a1d823ad4dca7a1aed272023bcc8b52d1ecf8d87cc2b6243af7b304b`  
		Last Modified: Sat, 30 Apr 2022 00:28:05 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876c62096d25857295729333b6636b768068d91f3eae91b7f972dbfed6283c05`  
		Last Modified: Fri, 13 May 2022 23:29:26 GMT  
		Size: 228.0 MB (227999939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04749675b1131ff08b7111a7a327e508233b0174895211163f9888c58ab284f0`  
		Last Modified: Fri, 13 May 2022 23:29:15 GMT  
		Size: 4.3 KB (4294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8307e4b86e0bf2f370d632a7ed0130854dedf4fc645702ab30cda86ce54d567`  
		Last Modified: Fri, 13 May 2022 23:29:15 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f239a48b417671aa0d734353e3ad43658e7488ec17a7464d1a6231a695270f6`  
		Last Modified: Fri, 13 May 2022 23:29:14 GMT  
		Size: 7.9 KB (7901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4842e1eca208649f917d4608d77294831603a5abcd10a125605afcc47c7bc7`  
		Last Modified: Fri, 13 May 2022 23:29:15 GMT  
		Size: 1.6 MB (1581707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:e44f54bbc95549fa903a9eee75263187dfccfb3a293e89e0bbe3c0a8bfff9f4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322893300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d34bf588eb3f16436745ef573253623c3832b70a107848059728f28f40f958f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:28:34 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 29 Apr 2022 23:30:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:30:47 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Fri, 29 Apr 2022 23:31:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b32bf4e18a0befea32c0ff377da7a1753b91477617a9921ceb3dee6964d2799b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.3_7.tar.gz';          ;;        armhf|arm)          ESUM='fda34743f1ad8b629f42773f6519e87d13876d4b10f98b76cd47b1aa9ad18572';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.3_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='257325f38546ce34645f6e8d7e566df401c97a9ae5f107583f9ac71f0f1b04e9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.3_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6790e3995a7fb8db99974d213f750bfd1631bfc0dad9946334be34d7b78fdbee';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.3_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='446b1ac5504d51c2ff9b0cccff079be3ce800cf8c3a3f13bab07f2656aa1fd27';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.3_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 29 Apr 2022 23:31:29 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Apr 2022 23:31:30 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Sat, 14 May 2022 00:10:48 GMT
ARG SOLR_VERSION=9.0.0
# Sat, 14 May 2022 00:10:48 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Sat, 14 May 2022 00:10:49 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Sat, 14 May 2022 00:10:50 GMT
ARG SOLR_DOWNLOAD_URL
# Sat, 14 May 2022 00:10:51 GMT
ARG SOLR_DOWNLOAD_SERVER
# Sat, 14 May 2022 00:10:52 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Sat, 14 May 2022 00:10:53 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Sat, 14 May 2022 00:10:54 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Sat, 14 May 2022 00:11:25 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Sat, 14 May 2022 00:11:26 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Sat, 14 May 2022 00:11:27 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Sat, 14 May 2022 00:11:28 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Sat, 14 May 2022 00:11:29 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Sat, 14 May 2022 00:11:30 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Sat, 14 May 2022 00:11:31 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Sat, 14 May 2022 00:11:32 GMT
LABEL org.opencontainers.image.version=9.0.0
# Sat, 14 May 2022 00:11:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 14 May 2022 00:11:34 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Sat, 14 May 2022 00:11:35 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Sat, 14 May 2022 00:11:36 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Sat, 14 May 2022 00:11:37 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Sat, 14 May 2022 00:11:45 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Sat, 14 May 2022 00:11:46 GMT
VOLUME [/var/solr]
# Sat, 14 May 2022 00:11:47 GMT
EXPOSE 8983
# Sat, 14 May 2022 00:11:48 GMT
WORKDIR /opt/solr
# Sat, 14 May 2022 00:11:49 GMT
USER solr
# Sat, 14 May 2022 00:11:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 May 2022 00:11:51 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b467f4b58f0fff42ab91803fe1a7c56675eed1a58f67991e9e7b0e445b91c1`  
		Last Modified: Fri, 29 Apr 2022 23:35:19 GMT  
		Size: 20.5 MB (20499354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec67f097ff34e42214a096abc801c87c94bf54ec712dd7c8c7cfa9c4cce2294`  
		Last Modified: Fri, 29 Apr 2022 23:36:00 GMT  
		Size: 46.3 MB (46273208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bba9689c028433e009befa69f8a6455447aa1ec9b056853669def5568774a96`  
		Last Modified: Fri, 29 Apr 2022 23:35:53 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b415d1ddaefb5d8027d56cad310b0c216bd1b46ac8eb0a61f99c533f58bd6f31`  
		Last Modified: Sat, 14 May 2022 00:12:43 GMT  
		Size: 227.7 MB (227732234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9cba1dc37bf0586566c8b69a261d88e47b94701e7f5b5036e4af25d44cf275`  
		Last Modified: Sat, 14 May 2022 00:12:28 GMT  
		Size: 4.3 KB (4306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1bf4097d07f0c3d5ad8afdfc49840a282fe780cfe7637207b7af4662e6b440`  
		Last Modified: Sat, 14 May 2022 00:12:29 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5d38a48836106d55623322e3baf4accd348fe2f1927c1c11fc336b86d09321`  
		Last Modified: Sat, 14 May 2022 00:12:28 GMT  
		Size: 7.8 KB (7816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2641ab12cd29715f6877ecf9e42554c1922f9fb42bfc1d36e7a707f3032e59`  
		Last Modified: Sat, 14 May 2022 00:12:29 GMT  
		Size: 1.2 MB (1206656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:9.0`

```console
$ docker pull solr@sha256:78cb909e5389ad8c2145219cd5dc26ab0be2a86035d43aafb299102f5b379023
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `solr:9.0` - linux; amd64

```console
$ docker pull solr@sha256:f72f67b0508995dff6202faec6cf598e5431e53adca4df0d40afc6063b9387cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.8 MB (324773439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5948c99fe303f72be967e390639935b5845cca537a84f3c0a29c4ee67dcb6529`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:22:32 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 30 Apr 2022 00:24:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:24:14 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Sat, 30 Apr 2022 00:24:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b32bf4e18a0befea32c0ff377da7a1753b91477617a9921ceb3dee6964d2799b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.3_7.tar.gz';          ;;        armhf|arm)          ESUM='fda34743f1ad8b629f42773f6519e87d13876d4b10f98b76cd47b1aa9ad18572';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.3_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='257325f38546ce34645f6e8d7e566df401c97a9ae5f107583f9ac71f0f1b04e9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.3_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6790e3995a7fb8db99974d213f750bfd1631bfc0dad9946334be34d7b78fdbee';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.3_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='446b1ac5504d51c2ff9b0cccff079be3ce800cf8c3a3f13bab07f2656aa1fd27';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.3_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 30 Apr 2022 00:24:41 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 30 Apr 2022 00:24:42 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 13 May 2022 23:27:55 GMT
ARG SOLR_VERSION=9.0.0
# Fri, 13 May 2022 23:27:55 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 13 May 2022 23:28:44 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.version=9.0.0
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 13 May 2022 23:28:45 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 13 May 2022 23:28:46 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 13 May 2022 23:28:46 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 13 May 2022 23:28:47 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 13 May 2022 23:28:56 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 13 May 2022 23:28:56 GMT
VOLUME [/var/solr]
# Fri, 13 May 2022 23:28:56 GMT
EXPOSE 8983
# Fri, 13 May 2022 23:28:56 GMT
WORKDIR /opt/solr
# Fri, 13 May 2022 23:28:56 GMT
USER solr
# Fri, 13 May 2022 23:28:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 May 2022 23:28:56 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5dc755b592da4b1124b1e234ecb462608d017290110a0193b350cec9a521e55`  
		Last Modified: Sat, 30 Apr 2022 00:27:40 GMT  
		Size: 19.8 MB (19772006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6121641ef15b3e95a1d7cf3f8ceb4230504204a59d6b3ef215d622a1390d4290`  
		Last Modified: Sat, 30 Apr 2022 00:28:12 GMT  
		Size: 46.8 MB (46840983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd235344a1d823ad4dca7a1aed272023bcc8b52d1ecf8d87cc2b6243af7b304b`  
		Last Modified: Sat, 30 Apr 2022 00:28:05 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876c62096d25857295729333b6636b768068d91f3eae91b7f972dbfed6283c05`  
		Last Modified: Fri, 13 May 2022 23:29:26 GMT  
		Size: 228.0 MB (227999939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04749675b1131ff08b7111a7a327e508233b0174895211163f9888c58ab284f0`  
		Last Modified: Fri, 13 May 2022 23:29:15 GMT  
		Size: 4.3 KB (4294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8307e4b86e0bf2f370d632a7ed0130854dedf4fc645702ab30cda86ce54d567`  
		Last Modified: Fri, 13 May 2022 23:29:15 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f239a48b417671aa0d734353e3ad43658e7488ec17a7464d1a6231a695270f6`  
		Last Modified: Fri, 13 May 2022 23:29:14 GMT  
		Size: 7.9 KB (7901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4842e1eca208649f917d4608d77294831603a5abcd10a125605afcc47c7bc7`  
		Last Modified: Fri, 13 May 2022 23:29:15 GMT  
		Size: 1.6 MB (1581707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.0` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:e44f54bbc95549fa903a9eee75263187dfccfb3a293e89e0bbe3c0a8bfff9f4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322893300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d34bf588eb3f16436745ef573253623c3832b70a107848059728f28f40f958f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:28:34 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 29 Apr 2022 23:30:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:30:47 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Fri, 29 Apr 2022 23:31:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b32bf4e18a0befea32c0ff377da7a1753b91477617a9921ceb3dee6964d2799b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.3_7.tar.gz';          ;;        armhf|arm)          ESUM='fda34743f1ad8b629f42773f6519e87d13876d4b10f98b76cd47b1aa9ad18572';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.3_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='257325f38546ce34645f6e8d7e566df401c97a9ae5f107583f9ac71f0f1b04e9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.3_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6790e3995a7fb8db99974d213f750bfd1631bfc0dad9946334be34d7b78fdbee';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.3_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='446b1ac5504d51c2ff9b0cccff079be3ce800cf8c3a3f13bab07f2656aa1fd27';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.3_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 29 Apr 2022 23:31:29 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Apr 2022 23:31:30 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Sat, 14 May 2022 00:10:48 GMT
ARG SOLR_VERSION=9.0.0
# Sat, 14 May 2022 00:10:48 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Sat, 14 May 2022 00:10:49 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Sat, 14 May 2022 00:10:50 GMT
ARG SOLR_DOWNLOAD_URL
# Sat, 14 May 2022 00:10:51 GMT
ARG SOLR_DOWNLOAD_SERVER
# Sat, 14 May 2022 00:10:52 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Sat, 14 May 2022 00:10:53 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Sat, 14 May 2022 00:10:54 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Sat, 14 May 2022 00:11:25 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Sat, 14 May 2022 00:11:26 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Sat, 14 May 2022 00:11:27 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Sat, 14 May 2022 00:11:28 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Sat, 14 May 2022 00:11:29 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Sat, 14 May 2022 00:11:30 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Sat, 14 May 2022 00:11:31 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Sat, 14 May 2022 00:11:32 GMT
LABEL org.opencontainers.image.version=9.0.0
# Sat, 14 May 2022 00:11:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 14 May 2022 00:11:34 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Sat, 14 May 2022 00:11:35 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Sat, 14 May 2022 00:11:36 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Sat, 14 May 2022 00:11:37 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Sat, 14 May 2022 00:11:45 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Sat, 14 May 2022 00:11:46 GMT
VOLUME [/var/solr]
# Sat, 14 May 2022 00:11:47 GMT
EXPOSE 8983
# Sat, 14 May 2022 00:11:48 GMT
WORKDIR /opt/solr
# Sat, 14 May 2022 00:11:49 GMT
USER solr
# Sat, 14 May 2022 00:11:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 May 2022 00:11:51 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b467f4b58f0fff42ab91803fe1a7c56675eed1a58f67991e9e7b0e445b91c1`  
		Last Modified: Fri, 29 Apr 2022 23:35:19 GMT  
		Size: 20.5 MB (20499354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec67f097ff34e42214a096abc801c87c94bf54ec712dd7c8c7cfa9c4cce2294`  
		Last Modified: Fri, 29 Apr 2022 23:36:00 GMT  
		Size: 46.3 MB (46273208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bba9689c028433e009befa69f8a6455447aa1ec9b056853669def5568774a96`  
		Last Modified: Fri, 29 Apr 2022 23:35:53 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b415d1ddaefb5d8027d56cad310b0c216bd1b46ac8eb0a61f99c533f58bd6f31`  
		Last Modified: Sat, 14 May 2022 00:12:43 GMT  
		Size: 227.7 MB (227732234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9cba1dc37bf0586566c8b69a261d88e47b94701e7f5b5036e4af25d44cf275`  
		Last Modified: Sat, 14 May 2022 00:12:28 GMT  
		Size: 4.3 KB (4306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1bf4097d07f0c3d5ad8afdfc49840a282fe780cfe7637207b7af4662e6b440`  
		Last Modified: Sat, 14 May 2022 00:12:29 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5d38a48836106d55623322e3baf4accd348fe2f1927c1c11fc336b86d09321`  
		Last Modified: Sat, 14 May 2022 00:12:28 GMT  
		Size: 7.8 KB (7816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2641ab12cd29715f6877ecf9e42554c1922f9fb42bfc1d36e7a707f3032e59`  
		Last Modified: Sat, 14 May 2022 00:12:29 GMT  
		Size: 1.2 MB (1206656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:9.0.0`

```console
$ docker pull solr@sha256:78cb909e5389ad8c2145219cd5dc26ab0be2a86035d43aafb299102f5b379023
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `solr:9.0.0` - linux; amd64

```console
$ docker pull solr@sha256:f72f67b0508995dff6202faec6cf598e5431e53adca4df0d40afc6063b9387cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.8 MB (324773439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5948c99fe303f72be967e390639935b5845cca537a84f3c0a29c4ee67dcb6529`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:22:32 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 30 Apr 2022 00:24:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:24:14 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Sat, 30 Apr 2022 00:24:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b32bf4e18a0befea32c0ff377da7a1753b91477617a9921ceb3dee6964d2799b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.3_7.tar.gz';          ;;        armhf|arm)          ESUM='fda34743f1ad8b629f42773f6519e87d13876d4b10f98b76cd47b1aa9ad18572';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.3_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='257325f38546ce34645f6e8d7e566df401c97a9ae5f107583f9ac71f0f1b04e9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.3_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6790e3995a7fb8db99974d213f750bfd1631bfc0dad9946334be34d7b78fdbee';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.3_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='446b1ac5504d51c2ff9b0cccff079be3ce800cf8c3a3f13bab07f2656aa1fd27';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.3_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 30 Apr 2022 00:24:41 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 30 Apr 2022 00:24:42 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 13 May 2022 23:27:55 GMT
ARG SOLR_VERSION=9.0.0
# Fri, 13 May 2022 23:27:55 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 13 May 2022 23:28:44 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.version=9.0.0
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 13 May 2022 23:28:45 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 13 May 2022 23:28:46 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 13 May 2022 23:28:46 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 13 May 2022 23:28:47 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 13 May 2022 23:28:56 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 13 May 2022 23:28:56 GMT
VOLUME [/var/solr]
# Fri, 13 May 2022 23:28:56 GMT
EXPOSE 8983
# Fri, 13 May 2022 23:28:56 GMT
WORKDIR /opt/solr
# Fri, 13 May 2022 23:28:56 GMT
USER solr
# Fri, 13 May 2022 23:28:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 May 2022 23:28:56 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5dc755b592da4b1124b1e234ecb462608d017290110a0193b350cec9a521e55`  
		Last Modified: Sat, 30 Apr 2022 00:27:40 GMT  
		Size: 19.8 MB (19772006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6121641ef15b3e95a1d7cf3f8ceb4230504204a59d6b3ef215d622a1390d4290`  
		Last Modified: Sat, 30 Apr 2022 00:28:12 GMT  
		Size: 46.8 MB (46840983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd235344a1d823ad4dca7a1aed272023bcc8b52d1ecf8d87cc2b6243af7b304b`  
		Last Modified: Sat, 30 Apr 2022 00:28:05 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876c62096d25857295729333b6636b768068d91f3eae91b7f972dbfed6283c05`  
		Last Modified: Fri, 13 May 2022 23:29:26 GMT  
		Size: 228.0 MB (227999939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04749675b1131ff08b7111a7a327e508233b0174895211163f9888c58ab284f0`  
		Last Modified: Fri, 13 May 2022 23:29:15 GMT  
		Size: 4.3 KB (4294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8307e4b86e0bf2f370d632a7ed0130854dedf4fc645702ab30cda86ce54d567`  
		Last Modified: Fri, 13 May 2022 23:29:15 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f239a48b417671aa0d734353e3ad43658e7488ec17a7464d1a6231a695270f6`  
		Last Modified: Fri, 13 May 2022 23:29:14 GMT  
		Size: 7.9 KB (7901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4842e1eca208649f917d4608d77294831603a5abcd10a125605afcc47c7bc7`  
		Last Modified: Fri, 13 May 2022 23:29:15 GMT  
		Size: 1.6 MB (1581707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:9.0.0` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:e44f54bbc95549fa903a9eee75263187dfccfb3a293e89e0bbe3c0a8bfff9f4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322893300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d34bf588eb3f16436745ef573253623c3832b70a107848059728f28f40f958f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:28:34 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 29 Apr 2022 23:30:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:30:47 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Fri, 29 Apr 2022 23:31:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b32bf4e18a0befea32c0ff377da7a1753b91477617a9921ceb3dee6964d2799b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.3_7.tar.gz';          ;;        armhf|arm)          ESUM='fda34743f1ad8b629f42773f6519e87d13876d4b10f98b76cd47b1aa9ad18572';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.3_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='257325f38546ce34645f6e8d7e566df401c97a9ae5f107583f9ac71f0f1b04e9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.3_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6790e3995a7fb8db99974d213f750bfd1631bfc0dad9946334be34d7b78fdbee';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.3_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='446b1ac5504d51c2ff9b0cccff079be3ce800cf8c3a3f13bab07f2656aa1fd27';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.3_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 29 Apr 2022 23:31:29 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Apr 2022 23:31:30 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Sat, 14 May 2022 00:10:48 GMT
ARG SOLR_VERSION=9.0.0
# Sat, 14 May 2022 00:10:48 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Sat, 14 May 2022 00:10:49 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Sat, 14 May 2022 00:10:50 GMT
ARG SOLR_DOWNLOAD_URL
# Sat, 14 May 2022 00:10:51 GMT
ARG SOLR_DOWNLOAD_SERVER
# Sat, 14 May 2022 00:10:52 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Sat, 14 May 2022 00:10:53 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Sat, 14 May 2022 00:10:54 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Sat, 14 May 2022 00:11:25 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Sat, 14 May 2022 00:11:26 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Sat, 14 May 2022 00:11:27 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Sat, 14 May 2022 00:11:28 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Sat, 14 May 2022 00:11:29 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Sat, 14 May 2022 00:11:30 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Sat, 14 May 2022 00:11:31 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Sat, 14 May 2022 00:11:32 GMT
LABEL org.opencontainers.image.version=9.0.0
# Sat, 14 May 2022 00:11:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 14 May 2022 00:11:34 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Sat, 14 May 2022 00:11:35 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Sat, 14 May 2022 00:11:36 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Sat, 14 May 2022 00:11:37 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Sat, 14 May 2022 00:11:45 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Sat, 14 May 2022 00:11:46 GMT
VOLUME [/var/solr]
# Sat, 14 May 2022 00:11:47 GMT
EXPOSE 8983
# Sat, 14 May 2022 00:11:48 GMT
WORKDIR /opt/solr
# Sat, 14 May 2022 00:11:49 GMT
USER solr
# Sat, 14 May 2022 00:11:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 May 2022 00:11:51 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b467f4b58f0fff42ab91803fe1a7c56675eed1a58f67991e9e7b0e445b91c1`  
		Last Modified: Fri, 29 Apr 2022 23:35:19 GMT  
		Size: 20.5 MB (20499354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec67f097ff34e42214a096abc801c87c94bf54ec712dd7c8c7cfa9c4cce2294`  
		Last Modified: Fri, 29 Apr 2022 23:36:00 GMT  
		Size: 46.3 MB (46273208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bba9689c028433e009befa69f8a6455447aa1ec9b056853669def5568774a96`  
		Last Modified: Fri, 29 Apr 2022 23:35:53 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b415d1ddaefb5d8027d56cad310b0c216bd1b46ac8eb0a61f99c533f58bd6f31`  
		Last Modified: Sat, 14 May 2022 00:12:43 GMT  
		Size: 227.7 MB (227732234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9cba1dc37bf0586566c8b69a261d88e47b94701e7f5b5036e4af25d44cf275`  
		Last Modified: Sat, 14 May 2022 00:12:28 GMT  
		Size: 4.3 KB (4306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1bf4097d07f0c3d5ad8afdfc49840a282fe780cfe7637207b7af4662e6b440`  
		Last Modified: Sat, 14 May 2022 00:12:29 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5d38a48836106d55623322e3baf4accd348fe2f1927c1c11fc336b86d09321`  
		Last Modified: Sat, 14 May 2022 00:12:28 GMT  
		Size: 7.8 KB (7816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2641ab12cd29715f6877ecf9e42554c1922f9fb42bfc1d36e7a707f3032e59`  
		Last Modified: Sat, 14 May 2022 00:12:29 GMT  
		Size: 1.2 MB (1206656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `solr:latest`

```console
$ docker pull solr@sha256:407aa42a9762b357fec33c997f3d6349dca0c616f5930b57bb4bd2777fd8b9cb
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
$ docker pull solr@sha256:f72f67b0508995dff6202faec6cf598e5431e53adca4df0d40afc6063b9387cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.8 MB (324773439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5948c99fe303f72be967e390639935b5845cca537a84f3c0a29c4ee67dcb6529`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:22:32 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 30 Apr 2022 00:24:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:24:14 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Sat, 30 Apr 2022 00:24:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b32bf4e18a0befea32c0ff377da7a1753b91477617a9921ceb3dee6964d2799b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.3_7.tar.gz';          ;;        armhf|arm)          ESUM='fda34743f1ad8b629f42773f6519e87d13876d4b10f98b76cd47b1aa9ad18572';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.3_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='257325f38546ce34645f6e8d7e566df401c97a9ae5f107583f9ac71f0f1b04e9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.3_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6790e3995a7fb8db99974d213f750bfd1631bfc0dad9946334be34d7b78fdbee';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.3_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='446b1ac5504d51c2ff9b0cccff079be3ce800cf8c3a3f13bab07f2656aa1fd27';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.3_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 30 Apr 2022 00:24:41 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 30 Apr 2022 00:24:42 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 13 May 2022 23:27:55 GMT
ARG SOLR_VERSION=9.0.0
# Fri, 13 May 2022 23:27:55 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_DOWNLOAD_URL
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_DOWNLOAD_SERVER
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 13 May 2022 23:27:56 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Fri, 13 May 2022 23:28:44 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.version=9.0.0
# Fri, 13 May 2022 23:28:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 13 May 2022 23:28:45 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Fri, 13 May 2022 23:28:46 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Fri, 13 May 2022 23:28:46 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Fri, 13 May 2022 23:28:47 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Fri, 13 May 2022 23:28:56 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Fri, 13 May 2022 23:28:56 GMT
VOLUME [/var/solr]
# Fri, 13 May 2022 23:28:56 GMT
EXPOSE 8983
# Fri, 13 May 2022 23:28:56 GMT
WORKDIR /opt/solr
# Fri, 13 May 2022 23:28:56 GMT
USER solr
# Fri, 13 May 2022 23:28:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 May 2022 23:28:56 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5dc755b592da4b1124b1e234ecb462608d017290110a0193b350cec9a521e55`  
		Last Modified: Sat, 30 Apr 2022 00:27:40 GMT  
		Size: 19.8 MB (19772006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6121641ef15b3e95a1d7cf3f8ceb4230504204a59d6b3ef215d622a1390d4290`  
		Last Modified: Sat, 30 Apr 2022 00:28:12 GMT  
		Size: 46.8 MB (46840983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd235344a1d823ad4dca7a1aed272023bcc8b52d1ecf8d87cc2b6243af7b304b`  
		Last Modified: Sat, 30 Apr 2022 00:28:05 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876c62096d25857295729333b6636b768068d91f3eae91b7f972dbfed6283c05`  
		Last Modified: Fri, 13 May 2022 23:29:26 GMT  
		Size: 228.0 MB (227999939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04749675b1131ff08b7111a7a327e508233b0174895211163f9888c58ab284f0`  
		Last Modified: Fri, 13 May 2022 23:29:15 GMT  
		Size: 4.3 KB (4294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8307e4b86e0bf2f370d632a7ed0130854dedf4fc645702ab30cda86ce54d567`  
		Last Modified: Fri, 13 May 2022 23:29:15 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f239a48b417671aa0d734353e3ad43658e7488ec17a7464d1a6231a695270f6`  
		Last Modified: Fri, 13 May 2022 23:29:14 GMT  
		Size: 7.9 KB (7901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4842e1eca208649f917d4608d77294831603a5abcd10a125605afcc47c7bc7`  
		Last Modified: Fri, 13 May 2022 23:29:15 GMT  
		Size: 1.6 MB (1581707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:latest` - linux; arm variant v7

```console
$ docker pull solr@sha256:033c9a89c5a6b600f75c36a6317f5f0452622a468c6d2320a3fdd0264398be74
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.3 MB (348309333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4449f465ea74895a41ce58ee5828eca0a29d9374913d5411baa3fdffcd7f5f2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 May 2019 12:03:26 GMT
ADD file:7e8dcc40e246d53b86266855a2de8080d26e6b4ed9f594c1acc565784405735b in / 
# Wed, 08 May 2019 12:03:27 GMT
CMD ["bash"]
# Wed, 08 May 2019 13:04:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 08 May 2019 13:04:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 08 May 2019 14:10:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 08 May 2019 14:10:10 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/stretch-backports.list
# Wed, 08 May 2019 14:10:11 GMT
ENV LANG=C.UTF-8
# Wed, 08 May 2019 14:10:15 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 08 May 2019 14:10:19 GMT
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 08 May 2019 14:10:20 GMT
ENV JAVA_HOME=/docker-java-home
# Wed, 08 May 2019 14:10:20 GMT
ENV JAVA_VERSION=11.0.3
# Wed, 08 May 2019 14:10:21 GMT
ENV JAVA_DEBIAN_VERSION=11.0.3+1-1~bpo9+1
# Wed, 08 May 2019 14:11:25 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		ln -svT /docker-java-home/bin/java /usr/local/bin/java; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-11-jre="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		rm -v /usr/local/bin/java; 		keytool -importkeystore -srckeystore /etc/ssl/certs/java/cacerts -destkeystore /etc/ssl/certs/java/cacerts.jks -deststoretype JKS -srcstorepass changeit -deststorepass changeit -noprompt; 	mv /etc/ssl/certs/java/cacerts.jks /etc/ssl/certs/java/cacerts; 	/var/lib/dpkg/info/ca-certificates-java.postinst configure; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Wed, 08 May 2019 17:58:41 GMT
LABEL maintainer=Martijn Koster "mak-docker@greenhills.co.uk"
# Wed, 08 May 2019 17:58:42 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 08 May 2019 17:58:42 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 08 May 2019 17:58:53 GMT
RUN apt-get update &&   apt-get -y install acl dirmngr gpg lsof procps wget &&   rm -rf /var/lib/apt/lists/*
# Wed, 08 May 2019 17:58:53 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_VERSION=8.0.0 SOLR_URL=https://archive.apache.org/dist/lucene/solr/8.0.0/solr-8.0.0.tgz SOLR_SHA256=0e6392d3b980ab917c731b054101aafcebceacc0e5063cb1e305aeeaec911d12 SOLR_KEYS=052C5B48A480B9CEA9E218A5F98C13CFA5A135D8 PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 08 May 2019 17:58:54 GMT
ENV GOSU_VERSION=1.11
# Wed, 08 May 2019 17:58:54 GMT
ENV GOSU_KEY=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Wed, 08 May 2019 17:58:56 GMT
RUN groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP" &&   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 08 May 2019 17:58:58 GMT
RUN set -e;   export GNUPGHOME="/tmp/gnupg_home" &&   mkdir -p "$GNUPGHOME" &&   chmod 700 "$GNUPGHOME" &&   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf" &&   for key in $SOLR_KEYS $GOSU_KEY; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 08 May 2019 18:00:21 GMT
RUN set -e;   export GNUPGHOME="/tmp/gnupg_home" &&   pkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')" &&   wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$pkgArch" &&   wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$pkgArch.asc" &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&   rm /usr/local/bin/gosu.asc &&   chmod +x /usr/local/bin/gosu &&   gosu nobody true &&   echo "downloading $SOLR_URL" &&   wget -nv "$SOLR_URL" -O "/opt/solr-$SOLR_VERSION.tgz" &&   echo "downloading $SOLR_URL.asc" &&   wget -nv "$SOLR_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc" &&   echo "$SOLR_SHA256 */opt/solr-$SOLR_VERSION.tgz" | sha256sum -c - &&   (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc") &&   gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz" &&   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz" &&   (cd /opt && ln -s "solr-$SOLR_VERSION" solr) &&   rm "/opt/solr-$SOLR_VERSION.tgz"* &&   rm -Rf /opt/solr/docs/ &&   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr &&   chown -R 0:0 "/opt/solr-$SOLR_VERSION" &&   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755 &&   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644 &&   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" &&   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh &&   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig &&   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig &&   chown root:0 /etc/default/solr.in.sh &&   chmod 0664 /etc/default/solr.in.sh &&   mkdir -p /var/solr/data /var/solr/logs &&   (cd /opt/solr/server/solr && cp solr.xml zoo.cfg /var/solr/data/) &&   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml &&   find /var/solr -type d -print0 | xargs -0 chmod 0770 &&   find /var/solr -type f -print0 | xargs -0 chmod 0660 &&   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr &&   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr &&   sed -i -e "/-Dsolr.clustering.enabled=true/ a SOLR_OPTS=\"\$SOLR_OPTS -Dsun.net.inetaddr.ttl=60 -Dsun.net.inetaddr.negative.ttl=60\"" /etc/default/solr.in.sh &&   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr &&   chown -R "$SOLR_USER:0" /var/solr
# Wed, 08 May 2019 18:00:22 GMT
COPY --chown=0:0dir:9826d1d133e0629ced7a9dfcb2401e9d607866337f15d2bdeecc49d308c6dfde in /opt/docker-solr/scripts 
# Wed, 08 May 2019 18:00:23 GMT
VOLUME [/var/solr]
# Wed, 08 May 2019 18:00:23 GMT
EXPOSE 8983
# Wed, 08 May 2019 18:00:24 GMT
WORKDIR /opt/solr
# Wed, 08 May 2019 18:00:24 GMT
USER solr
# Wed, 08 May 2019 18:00:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 May 2019 18:00:25 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:f2a2fd7c1ab35cd1b5ea6fcc2b801f3877852797e2698ecdb9556e0dee3accb5`  
		Last Modified: Wed, 08 May 2019 12:09:40 GMT  
		Size: 42.1 MB (42082604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047df9a92c9f7376283a8d6af526f5126d95995ba48dd7de49979ef57da3e15b`  
		Last Modified: Wed, 08 May 2019 13:12:20 GMT  
		Size: 9.5 MB (9485167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddeed4ac8d1e2c751afd6fd3517f1d154365467039353c377c8206fd5eb81d4b`  
		Last Modified: Wed, 08 May 2019 13:12:18 GMT  
		Size: 3.9 MB (3918605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c646a29b8c83d854b86dccdbf390a7b296f5144aef4e38276c8a7b649e0804`  
		Last Modified: Wed, 08 May 2019 14:31:13 GMT  
		Size: 830.4 KB (830410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6f0d217548ad4fca27f3fca1ad13e1d42b51dfdc66efe11ca75bec1768f91e`  
		Last Modified: Wed, 08 May 2019 14:31:12 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835b3a1a9cf41d4f4ba6bd276263e9aa9d9510a7f587316f5128b4b8848a3fb8`  
		Last Modified: Wed, 08 May 2019 14:31:12 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5554c002ae1621fa85e450b809bb153315535856beedc3a4de016e7f8088ee3`  
		Last Modified: Wed, 08 May 2019 14:31:12 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74989df1042192176323ee1dd7ec5a173ef7c944e14eb3192d1cd38ca6750c97`  
		Last Modified: Wed, 08 May 2019 14:31:44 GMT  
		Size: 116.2 MB (116170095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4048eb07d226a7de812b2b5f3499754b3758053879d532a9ec71f51904b0fc`  
		Last Modified: Wed, 08 May 2019 18:22:12 GMT  
		Size: 2.9 MB (2853092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc86f898449d3157c73ecb30a7a612f26d0476b25d34a70b760fc2e09d3871d`  
		Last Modified: Wed, 08 May 2019 18:22:11 GMT  
		Size: 4.2 KB (4222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0e63a29cdbd2d97774f8caa5d937468ab48c95178e5a6d5afab45f6bafc0be`  
		Last Modified: Wed, 08 May 2019 18:22:11 GMT  
		Size: 75.4 KB (75386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5a01eac31d50dd94de5d1479033e6e8ea22f7665b40d276713ef2eab317b68`  
		Last Modified: Wed, 08 May 2019 18:22:36 GMT  
		Size: 172.9 MB (172885308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194c8ce6c5808178b4c47a1d5a6e7c3116a30661f5e9860979f6d043589c3921`  
		Last Modified: Wed, 08 May 2019 18:22:11 GMT  
		Size: 3.8 KB (3839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:latest` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:e44f54bbc95549fa903a9eee75263187dfccfb3a293e89e0bbe3c0a8bfff9f4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322893300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d34bf588eb3f16436745ef573253623c3832b70a107848059728f28f40f958f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:28:34 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 29 Apr 2022 23:30:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:30:47 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Fri, 29 Apr 2022 23:31:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b32bf4e18a0befea32c0ff377da7a1753b91477617a9921ceb3dee6964d2799b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.3_7.tar.gz';          ;;        armhf|arm)          ESUM='fda34743f1ad8b629f42773f6519e87d13876d4b10f98b76cd47b1aa9ad18572';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.3_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='257325f38546ce34645f6e8d7e566df401c97a9ae5f107583f9ac71f0f1b04e9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.3_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6790e3995a7fb8db99974d213f750bfd1631bfc0dad9946334be34d7b78fdbee';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.3_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='446b1ac5504d51c2ff9b0cccff079be3ce800cf8c3a3f13bab07f2656aa1fd27';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.3_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 29 Apr 2022 23:31:29 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Apr 2022 23:31:30 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Sat, 14 May 2022 00:10:48 GMT
ARG SOLR_VERSION=9.0.0
# Sat, 14 May 2022 00:10:48 GMT
ARG SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5
# Sat, 14 May 2022 00:10:49 GMT
ARG SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93
# Sat, 14 May 2022 00:10:50 GMT
ARG SOLR_DOWNLOAD_URL
# Sat, 14 May 2022 00:10:51 GMT
ARG SOLR_DOWNLOAD_SERVER
# Sat, 14 May 2022 00:10:52 GMT
ARG SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz
# Sat, 14 May 2022 00:10:53 GMT
ARG SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Sat, 14 May 2022 00:10:54 GMT
ARG SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz
# Sat, 14 May 2022 00:11:25 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   apt-get update;   apt-get -y install wget gpg dirmngr;   rm -rf /var/lib/apt/lists/*;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   if [ -n "$SOLR_KEYS" ]; then     wget -nv "https://downloads.apache.org/solr/KEYS" -O- |       gpg --batch --import --key-origin 'url,https://downloads.apache.org/solr/KEYS';     release_keys="$(gpg --batch --export -a ${SOLR_KEYS})";     rm -rf "$GNUPGHOME"/*;     echo "${release_keys}" | gpg --batch --import;   fi;   MAX_REDIRECTS=2;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME";   tar -C /opt --extract --preserve-permissions --file "/opt/solr-$SOLR_VERSION.tgz";   rm "/opt/solr-$SOLR_VERSION.tgz"*;
# Sat, 14 May 2022 00:11:26 GMT
LABEL org.opencontainers.image.title=Apache Solr
# Sat, 14 May 2022 00:11:27 GMT
LABEL org.opencontainers.image.description=Apache Solr is the popular, blazing-fast, open source search platform built on Apache Lucene.
# Sat, 14 May 2022 00:11:28 GMT
LABEL org.opencontainers.image.authors=The Apache Solr Project
# Sat, 14 May 2022 00:11:29 GMT
LABEL org.opencontainers.image.url=https://solr.apache.org
# Sat, 14 May 2022 00:11:30 GMT
LABEL org.opencontainers.image.source=https://github.com/apache/solr
# Sat, 14 May 2022 00:11:31 GMT
LABEL org.opencontainers.image.documentation=https://solr.apache.org/guide/
# Sat, 14 May 2022 00:11:32 GMT
LABEL org.opencontainers.image.version=9.0.0
# Sat, 14 May 2022 00:11:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 14 May 2022 00:11:34 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 PATH=/opt/solr/bin:/opt/solr/docker/scripts:/opt/solr/prometheus-exporter/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml SOLR_JETTY_HOST=0.0.0.0
# Sat, 14 May 2022 00:11:35 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Sat, 14 May 2022 00:11:36 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   (cd /opt; ln -s solr-*/ solr);   rm -Rf /opt/solr/docs /opt/solr/docker/Dockerfile;
# Sat, 14 May 2022 00:11:37 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p -m0770 /var/solr;   chown -R "$SOLR_USER:0" /var/solr;   ln -s /opt/solr/modules /opt/solr/contrib;   ln -s /opt/solr/prometheus-exporter /opt/solr/modules/prometheus-exporter;
# Sat, 14 May 2022 00:11:45 GMT
# ARGS: SOLR_ARCHIVE_URL=https://archive.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?action=download&filename=/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_DIST_URL=https://www.apache.org/dist/solr/solr/9.0.0/solr-9.0.0.tgz SOLR_KEYS=3558857D1F5754B78C7F8B5A71A45A3D0D8D0B93 SOLR_SHA512=383c6b6f352f2a385ece99b2b0a82e1552430aea65c6c33e5569da422138844192db4e06f58699325af55ee631694e16f836a5bbf8556f86fdeabc0cfa0533d5 SOLR_VERSION=9.0.0
RUN set -ex;     apt-get update;     apt-get -y install acl dirmngr lsof procps wget netcat gosu tini jattach;     rm -rf /var/lib/apt/lists/*;
# Sat, 14 May 2022 00:11:46 GMT
VOLUME [/var/solr]
# Sat, 14 May 2022 00:11:47 GMT
EXPOSE 8983
# Sat, 14 May 2022 00:11:48 GMT
WORKDIR /opt/solr
# Sat, 14 May 2022 00:11:49 GMT
USER solr
# Sat, 14 May 2022 00:11:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 May 2022 00:11:51 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b467f4b58f0fff42ab91803fe1a7c56675eed1a58f67991e9e7b0e445b91c1`  
		Last Modified: Fri, 29 Apr 2022 23:35:19 GMT  
		Size: 20.5 MB (20499354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec67f097ff34e42214a096abc801c87c94bf54ec712dd7c8c7cfa9c4cce2294`  
		Last Modified: Fri, 29 Apr 2022 23:36:00 GMT  
		Size: 46.3 MB (46273208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bba9689c028433e009befa69f8a6455447aa1ec9b056853669def5568774a96`  
		Last Modified: Fri, 29 Apr 2022 23:35:53 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b415d1ddaefb5d8027d56cad310b0c216bd1b46ac8eb0a61f99c533f58bd6f31`  
		Last Modified: Sat, 14 May 2022 00:12:43 GMT  
		Size: 227.7 MB (227732234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9cba1dc37bf0586566c8b69a261d88e47b94701e7f5b5036e4af25d44cf275`  
		Last Modified: Sat, 14 May 2022 00:12:28 GMT  
		Size: 4.3 KB (4306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1bf4097d07f0c3d5ad8afdfc49840a282fe780cfe7637207b7af4662e6b440`  
		Last Modified: Sat, 14 May 2022 00:12:29 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5d38a48836106d55623322e3baf4accd348fe2f1927c1c11fc336b86d09321`  
		Last Modified: Sat, 14 May 2022 00:12:28 GMT  
		Size: 7.8 KB (7816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2641ab12cd29715f6877ecf9e42554c1922f9fb42bfc1d36e7a707f3032e59`  
		Last Modified: Sat, 14 May 2022 00:12:29 GMT  
		Size: 1.2 MB (1206656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:latest` - linux; ppc64le

```console
$ docker pull solr@sha256:621d3a1c4bedccf2787f2a84168556b943119861ba91bc65fa00adbdbda9e884
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **356.1 MB (356146320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d49fb3d7602942af34615a12c37e3bc76d31eb7c5d19c07147c39f47ce86a82f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 May 2019 09:03:26 GMT
ADD file:844cea0aa071f0f6b2640d4c452590a8777485fa27a0aad789553110eaeb7081 in / 
# Wed, 08 May 2019 09:03:33 GMT
CMD ["bash"]
# Wed, 08 May 2019 12:06:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 08 May 2019 12:07:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 08 May 2019 12:39:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 08 May 2019 12:39:34 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/stretch-backports.list
# Wed, 08 May 2019 12:39:37 GMT
ENV LANG=C.UTF-8
# Wed, 08 May 2019 12:39:45 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 08 May 2019 12:39:54 GMT
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 08 May 2019 12:39:57 GMT
ENV JAVA_HOME=/docker-java-home
# Wed, 08 May 2019 12:40:00 GMT
ENV JAVA_VERSION=11.0.3
# Wed, 08 May 2019 12:40:04 GMT
ENV JAVA_DEBIAN_VERSION=11.0.3+1-1~bpo9+1
# Wed, 08 May 2019 12:45:53 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		ln -svT /docker-java-home/bin/java /usr/local/bin/java; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-11-jre="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		rm -v /usr/local/bin/java; 		keytool -importkeystore -srckeystore /etc/ssl/certs/java/cacerts -destkeystore /etc/ssl/certs/java/cacerts.jks -deststoretype JKS -srcstorepass changeit -deststorepass changeit -noprompt; 	mv /etc/ssl/certs/java/cacerts.jks /etc/ssl/certs/java/cacerts; 	/var/lib/dpkg/info/ca-certificates-java.postinst configure; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Wed, 08 May 2019 22:12:49 GMT
LABEL maintainer=Martijn Koster "mak-docker@greenhills.co.uk"
# Wed, 08 May 2019 22:12:52 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 08 May 2019 22:12:54 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 08 May 2019 22:13:36 GMT
RUN apt-get update &&   apt-get -y install acl dirmngr gpg lsof procps wget &&   rm -rf /var/lib/apt/lists/*
# Wed, 08 May 2019 22:13:40 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_VERSION=8.0.0 SOLR_URL=https://archive.apache.org/dist/lucene/solr/8.0.0/solr-8.0.0.tgz SOLR_SHA256=0e6392d3b980ab917c731b054101aafcebceacc0e5063cb1e305aeeaec911d12 SOLR_KEYS=052C5B48A480B9CEA9E218A5F98C13CFA5A135D8 PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 08 May 2019 22:13:44 GMT
ENV GOSU_VERSION=1.11
# Wed, 08 May 2019 22:13:48 GMT
ENV GOSU_KEY=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Wed, 08 May 2019 22:14:02 GMT
RUN groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP" &&   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 08 May 2019 22:14:12 GMT
RUN set -e;   export GNUPGHOME="/tmp/gnupg_home" &&   mkdir -p "$GNUPGHOME" &&   chmod 700 "$GNUPGHOME" &&   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf" &&   for key in $SOLR_KEYS $GOSU_KEY; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 08 May 2019 22:16:17 GMT
RUN set -e;   export GNUPGHOME="/tmp/gnupg_home" &&   pkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')" &&   wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$pkgArch" &&   wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$pkgArch.asc" &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&   rm /usr/local/bin/gosu.asc &&   chmod +x /usr/local/bin/gosu &&   gosu nobody true &&   echo "downloading $SOLR_URL" &&   wget -nv "$SOLR_URL" -O "/opt/solr-$SOLR_VERSION.tgz" &&   echo "downloading $SOLR_URL.asc" &&   wget -nv "$SOLR_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc" &&   echo "$SOLR_SHA256 */opt/solr-$SOLR_VERSION.tgz" | sha256sum -c - &&   (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc") &&   gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz" &&   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz" &&   (cd /opt && ln -s "solr-$SOLR_VERSION" solr) &&   rm "/opt/solr-$SOLR_VERSION.tgz"* &&   rm -Rf /opt/solr/docs/ &&   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr &&   chown -R 0:0 "/opt/solr-$SOLR_VERSION" &&   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755 &&   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644 &&   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" &&   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh &&   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig &&   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig &&   chown root:0 /etc/default/solr.in.sh &&   chmod 0664 /etc/default/solr.in.sh &&   mkdir -p /var/solr/data /var/solr/logs &&   (cd /opt/solr/server/solr && cp solr.xml zoo.cfg /var/solr/data/) &&   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml &&   find /var/solr -type d -print0 | xargs -0 chmod 0770 &&   find /var/solr -type f -print0 | xargs -0 chmod 0660 &&   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr &&   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr &&   sed -i -e "/-Dsolr.clustering.enabled=true/ a SOLR_OPTS=\"\$SOLR_OPTS -Dsun.net.inetaddr.ttl=60 -Dsun.net.inetaddr.negative.ttl=60\"" /etc/default/solr.in.sh &&   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr &&   chown -R "$SOLR_USER:0" /var/solr
# Wed, 08 May 2019 22:16:22 GMT
COPY --chown=0:0dir:9826d1d133e0629ced7a9dfcb2401e9d607866337f15d2bdeecc49d308c6dfde in /opt/docker-solr/scripts 
# Wed, 08 May 2019 22:16:27 GMT
VOLUME [/var/solr]
# Wed, 08 May 2019 22:16:33 GMT
EXPOSE 8983
# Wed, 08 May 2019 22:16:36 GMT
WORKDIR /opt/solr
# Wed, 08 May 2019 22:16:39 GMT
USER solr
# Wed, 08 May 2019 22:16:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 May 2019 22:16:54 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:c6c4df30bc4ffa8fb97a3dda6f8758fb0ddeb8929d159369cf5974dd3f2ac117`  
		Last Modified: Wed, 08 May 2019 09:21:32 GMT  
		Size: 45.6 MB (45603184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8b6d64c78121ab5074c55b90272e1a13e72e3b7854d6a6c7e638eff77307ba`  
		Last Modified: Wed, 08 May 2019 12:24:57 GMT  
		Size: 10.0 MB (9991084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663d68dc2e1243453bf4b04afcb5394452ca5371b05a1c96f41a0df4189631e8`  
		Last Modified: Wed, 08 May 2019 12:24:54 GMT  
		Size: 4.3 MB (4296597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98e4e060b9a0f1aadc5647d44be482b1363697a3fd8a4aeb6a4b9c53e17ecc4`  
		Last Modified: Wed, 08 May 2019 13:14:21 GMT  
		Size: 848.6 KB (848616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afcad30d91e6ef6a6235e8ee8ea34984a8a03714f83006880a27d23e1ec6b07`  
		Last Modified: Wed, 08 May 2019 13:14:21 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17792a5a83e70e4555affd27a076727218038ebe3722cbcecde52eb8d81e41e8`  
		Last Modified: Wed, 08 May 2019 13:14:21 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743f9ba8d5fbd6557dc6ece9e230fd856733b23a5d6477a9a669a4f68c61da85`  
		Last Modified: Wed, 08 May 2019 13:14:21 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f4c5964ec2a98758cf78dd517a7d26b5badaa386bdfb0386d00ef2df17dd4bd`  
		Last Modified: Wed, 08 May 2019 13:16:33 GMT  
		Size: 119.5 MB (119451690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0e1da789389fc7e35d2f133c80c0807f324c94cc9fe0f59924b5d5dfb92887`  
		Last Modified: Wed, 08 May 2019 23:10:42 GMT  
		Size: 3.0 MB (3014133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbcf38b9ba911472ec8af46877490ad7f4df59041ab1297e7b068807f799edc`  
		Last Modified: Wed, 08 May 2019 23:10:36 GMT  
		Size: 4.3 KB (4301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a2f262f9bc74de93c19f7b710b17afa33ff62d43daaafc73c0179c4ca6825c`  
		Last Modified: Wed, 08 May 2019 23:10:36 GMT  
		Size: 75.4 KB (75411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598f1bef79d4165be42bbce14df49fdd8c822df8f04f99b39267b5a1feb1c012`  
		Last Modified: Wed, 08 May 2019 23:11:16 GMT  
		Size: 172.9 MB (172856855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d971dcbc1bda5243a914ca0e940428fc852da25e4524e2b18b313ae3dcd5ef`  
		Last Modified: Wed, 08 May 2019 23:10:36 GMT  
		Size: 3.8 KB (3841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:latest` - linux; s390x

```console
$ docker pull solr@sha256:c753e1cb2595ffd88366b9c16731d55fd60e6bde40ac3856a1da391826bb6eae
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.9 MB (355934433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57bf28c3ae9e2843158153ca8b51c75625fb7448fb3d939f76072a828b4fef68`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Wed, 08 May 2019 11:46:30 GMT
ADD file:35b243252442c1fc6a9e4f7bea498f5b7302c530eb804ed6a79c5b84a68a96fd in / 
# Wed, 08 May 2019 11:46:31 GMT
CMD ["bash"]
# Wed, 08 May 2019 13:48:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 08 May 2019 13:48:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 08 May 2019 14:42:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 08 May 2019 14:42:15 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/stretch-backports.list
# Wed, 08 May 2019 14:42:16 GMT
ENV LANG=C.UTF-8
# Wed, 08 May 2019 14:42:20 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 08 May 2019 14:42:23 GMT
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 08 May 2019 14:42:24 GMT
ENV JAVA_HOME=/docker-java-home
# Wed, 08 May 2019 14:42:25 GMT
ENV JAVA_VERSION=11.0.3
# Wed, 08 May 2019 14:42:25 GMT
ENV JAVA_DEBIAN_VERSION=11.0.3+1-1~bpo9+1
# Wed, 08 May 2019 14:45:19 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		ln -svT /docker-java-home/bin/java /usr/local/bin/java; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-11-jre="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		rm -v /usr/local/bin/java; 		keytool -importkeystore -srckeystore /etc/ssl/certs/java/cacerts -destkeystore /etc/ssl/certs/java/cacerts.jks -deststoretype JKS -srcstorepass changeit -deststorepass changeit -noprompt; 	mv /etc/ssl/certs/java/cacerts.jks /etc/ssl/certs/java/cacerts; 	/var/lib/dpkg/info/ca-certificates-java.postinst configure; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Thu, 09 May 2019 05:38:38 GMT
LABEL maintainer=Martijn Koster "mak-docker@greenhills.co.uk"
# Thu, 09 May 2019 05:38:40 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Thu, 09 May 2019 05:38:43 GMT
ARG SOLR_DOWNLOAD_SERVER
# Thu, 09 May 2019 05:39:37 GMT
RUN apt-get update &&   apt-get -y install acl dirmngr gpg lsof procps wget &&   rm -rf /var/lib/apt/lists/*
# Thu, 09 May 2019 05:39:38 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_VERSION=8.0.0 SOLR_URL=https://archive.apache.org/dist/lucene/solr/8.0.0/solr-8.0.0.tgz SOLR_SHA256=0e6392d3b980ab917c731b054101aafcebceacc0e5063cb1e305aeeaec911d12 SOLR_KEYS=052C5B48A480B9CEA9E218A5F98C13CFA5A135D8 PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Thu, 09 May 2019 05:39:39 GMT
ENV GOSU_VERSION=1.11
# Thu, 09 May 2019 05:39:40 GMT
ENV GOSU_KEY=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Thu, 09 May 2019 05:39:46 GMT
RUN groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP" &&   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Thu, 09 May 2019 05:39:59 GMT
RUN set -e;   export GNUPGHOME="/tmp/gnupg_home" &&   mkdir -p "$GNUPGHOME" &&   chmod 700 "$GNUPGHOME" &&   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf" &&   for key in $SOLR_KEYS $GOSU_KEY; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Thu, 09 May 2019 05:41:00 GMT
RUN set -e;   export GNUPGHOME="/tmp/gnupg_home" &&   pkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')" &&   wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$pkgArch" &&   wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$pkgArch.asc" &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&   rm /usr/local/bin/gosu.asc &&   chmod +x /usr/local/bin/gosu &&   gosu nobody true &&   echo "downloading $SOLR_URL" &&   wget -nv "$SOLR_URL" -O "/opt/solr-$SOLR_VERSION.tgz" &&   echo "downloading $SOLR_URL.asc" &&   wget -nv "$SOLR_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc" &&   echo "$SOLR_SHA256 */opt/solr-$SOLR_VERSION.tgz" | sha256sum -c - &&   (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc") &&   gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz" &&   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz" &&   (cd /opt && ln -s "solr-$SOLR_VERSION" solr) &&   rm "/opt/solr-$SOLR_VERSION.tgz"* &&   rm -Rf /opt/solr/docs/ &&   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr &&   chown -R 0:0 "/opt/solr-$SOLR_VERSION" &&   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755 &&   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644 &&   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" &&   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh &&   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig &&   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig &&   chown root:0 /etc/default/solr.in.sh &&   chmod 0664 /etc/default/solr.in.sh &&   mkdir -p /var/solr/data /var/solr/logs &&   (cd /opt/solr/server/solr && cp solr.xml zoo.cfg /var/solr/data/) &&   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml &&   find /var/solr -type d -print0 | xargs -0 chmod 0770 &&   find /var/solr -type f -print0 | xargs -0 chmod 0660 &&   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr &&   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr &&   sed -i -e "/-Dsolr.clustering.enabled=true/ a SOLR_OPTS=\"\$SOLR_OPTS -Dsun.net.inetaddr.ttl=60 -Dsun.net.inetaddr.negative.ttl=60\"" /etc/default/solr.in.sh &&   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr &&   chown -R "$SOLR_USER:0" /var/solr
# Thu, 09 May 2019 05:41:02 GMT
COPY --chown=0:0dir:9826d1d133e0629ced7a9dfcb2401e9d607866337f15d2bdeecc49d308c6dfde in /opt/docker-solr/scripts 
# Thu, 09 May 2019 05:41:03 GMT
VOLUME [/var/solr]
# Thu, 09 May 2019 05:41:05 GMT
EXPOSE 8983
# Thu, 09 May 2019 05:41:07 GMT
WORKDIR /opt/solr
# Thu, 09 May 2019 05:41:09 GMT
USER solr
# Thu, 09 May 2019 05:41:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 May 2019 05:41:15 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:3602dd773e45048fcb10569c368bf7ddac54267760f371efbe1bb65ba8d67361`  
		Last Modified: Wed, 08 May 2019 11:52:15 GMT  
		Size: 45.2 MB (45197648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a17b553a57c91ed490be0279a1aafa108b9a60b10f8c482ed85ca94de3a3c`  
		Last Modified: Wed, 08 May 2019 14:00:34 GMT  
		Size: 10.3 MB (10314565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5007dca2cc2afa05648742b75324a09e45eae504d384750ed7c6de3e5e5d65d2`  
		Last Modified: Wed, 08 May 2019 14:00:30 GMT  
		Size: 4.4 MB (4372280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf61465b03d8ec5e8064ba91220d0e97c4dd5b75a7d2fe644aab7cc4a0a514c`  
		Last Modified: Wed, 08 May 2019 15:01:34 GMT  
		Size: 863.9 KB (863943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7875682bb43ee4dfedb0db2f5ffa045803895445c3434edfed0723d3f4dd700`  
		Last Modified: Wed, 08 May 2019 15:01:33 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7406aa79a5f911227056620e3ae81aaf33a7c207f34292a287bda26a00db256a`  
		Last Modified: Wed, 08 May 2019 15:01:33 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82c65756cebc86ea719c2cabfae397ed4030a5a942dc03f44dd0f91272fb555`  
		Last Modified: Wed, 08 May 2019 15:01:33 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b85b1ac77736c32a8c794742d393f3ab32897f6833cba700dd680ab8fd406f2`  
		Last Modified: Wed, 08 May 2019 15:02:08 GMT  
		Size: 119.2 MB (119161534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc5089230f270d077e78a57736b75a3e6ad4358b62323713d14eab00bb263ea`  
		Last Modified: Thu, 09 May 2019 06:03:49 GMT  
		Size: 3.0 MB (3017234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e51afb6451ed55deef6d588f779da220ba051d4cdc2232cb83c707c3fb82441`  
		Last Modified: Thu, 09 May 2019 06:03:46 GMT  
		Size: 4.3 KB (4330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeb128c687e4d3d85520d2b326e78555217a8cbebaa35193fbc8185bfba797f`  
		Last Modified: Thu, 09 May 2019 06:03:46 GMT  
		Size: 75.4 KB (75378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7f81e27f4a98d13e8f3c96b463d6e243ff02bc65d3d713d5f582aa124651ee`  
		Last Modified: Thu, 09 May 2019 06:04:34 GMT  
		Size: 172.9 MB (172923099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8496785b2c899063f3b7a7ad3f1533951d7bd8df0e09b94a2c01f76cc505ba39`  
		Last Modified: Thu, 09 May 2019 06:03:46 GMT  
		Size: 3.8 KB (3816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
