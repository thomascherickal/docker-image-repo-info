## `solr:5-slim`

```console
$ docker pull solr@sha256:3d8a1486432577494efdf31c2006b558a49d7792e8fcfc9be3092a100311ba00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `solr:5-slim` - linux; amd64

```console
$ docker pull solr@sha256:9905ff39d3b396521884bb9e148ed91a5a6126180bf5f26e8ad2210afb3ef9cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.3 MB (209328264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a7f69d2545b7659ddf5c4ba6a15dfbd2867f80a2408dd4d703cf6ecb87abb23`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 21:00:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 21:00:03 GMT
ENV LANG=C.UTF-8
# Fri, 15 May 2020 21:04:30 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 15 May 2020 21:04:30 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 21:04:31 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 15 May 2020 21:04:31 GMT
ENV JAVA_VERSION=8u252
# Fri, 15 May 2020 21:05:14 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Fri, 15 May 2020 21:05:15 GMT
ENV JAVA_URL_VERSION=8u252b09
# Fri, 15 May 2020 21:05:29 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Mon, 08 Jun 2020 19:33:17 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Mon, 08 Jun 2020 19:33:18 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Mon, 08 Jun 2020 19:34:20 GMT
ARG SOLR_VERSION=5.5.5
# Mon, 08 Jun 2020 19:34:20 GMT
ARG SOLR_SHA512=9aa02a362b75fc2af8c01d7b7d37d04450787902397644ca2d950836aa9efc8447922255d23de1d228c96f442ec82b08be64c590438dbf5f71da04616ab022f2
# Mon, 08 Jun 2020 19:34:21 GMT
ARG SOLR_KEYS=5F55943E13D49059D3F342777186B06E1ED139E7
# Mon, 08 Jun 2020 19:34:21 GMT
ARG SOLR_DOWNLOAD_URL
# Mon, 08 Jun 2020 19:34:21 GMT
ARG SOLR_DOWNLOAD_SERVER
# Mon, 08 Jun 2020 19:34:28 GMT
# ARGS: SOLR_KEYS=5F55943E13D49059D3F342777186B06E1ED139E7 SOLR_SHA512=9aa02a362b75fc2af8c01d7b7d37d04450787902397644ca2d950836aa9efc8447922255d23de1d228c96f442ec82b08be64c590438dbf5f71da04616ab022f2 SOLR_VERSION=5.5.5
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Mon, 08 Jun 2020 19:34:28 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/5.5.5/solr-5.5.5.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/5.5.5/solr-5.5.5.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/5.5.5/solr-5.5.5.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 08 Jun 2020 19:34:29 GMT
# ARGS: SOLR_KEYS=5F55943E13D49059D3F342777186B06E1ED139E7 SOLR_SHA512=9aa02a362b75fc2af8c01d7b7d37d04450787902397644ca2d950836aa9efc8447922255d23de1d228c96f442ec82b08be64c590438dbf5f71da04616ab022f2 SOLR_VERSION=5.5.5
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Mon, 08 Jun 2020 19:34:30 GMT
# ARGS: SOLR_KEYS=5F55943E13D49059D3F342777186B06E1ED139E7 SOLR_SHA512=9aa02a362b75fc2af8c01d7b7d37d04450787902397644ca2d950836aa9efc8447922255d23de1d228c96f442ec82b08be64c590438dbf5f71da04616ab022f2 SOLR_VERSION=5.5.5
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Mon, 08 Jun 2020 19:34:43 GMT
# ARGS: SOLR_KEYS=5F55943E13D49059D3F342777186B06E1ED139E7 SOLR_SHA512=9aa02a362b75fc2af8c01d7b7d37d04450787902397644ca2d950836aa9efc8447922255d23de1d228c96f442ec82b08be64c590438dbf5f71da04616ab022f2 SOLR_VERSION=5.5.5
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   mv "/opt/solr-$SOLR_VERSION" /opt/solr;   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   mkdir -p /opt/solr/server/solr/mycores /opt/solr/server/logs /opt/mysolrhome;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   if [ -f "/opt/solr/contrib/prometheus-exporter/bin/solr-exporter" ]; then chmod 0755 "/opt/solr/contrib/prometheus-exporter/bin/solr-exporter"; fi;   chmod -R 0755 /opt/solr/server/scripts/cloud-scripts;   chown -R "$SOLR_USER:$SOLR_GROUP" /opt/solr /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:$SOLR_GROUP" /opt/mysolrhome;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Mon, 08 Jun 2020 19:34:43 GMT
COPY --chown=solr:solrdir:24d14aedda51f56007d2c3091bd65f0167210afaf1c88aa50fac48af9e1d6037 in /opt/docker-solr/scripts 
# Mon, 08 Jun 2020 19:34:44 GMT
EXPOSE 8983
# Mon, 08 Jun 2020 19:34:44 GMT
WORKDIR /opt/solr
# Mon, 08 Jun 2020 19:34:44 GMT
USER solr
# Mon, 08 Jun 2020 19:34:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 08 Jun 2020 19:34:44 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee19e84e8bd1140527176689c9c1a75f28c0462c0c714e549536452708cbfb64`  
		Last Modified: Fri, 15 May 2020 21:07:16 GMT  
		Size: 3.2 MB (3249166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832173019a2785ef0aa682f31c851a09a93d6542ea2b407f04d031890ba1021d`  
		Last Modified: Fri, 15 May 2020 21:11:13 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80ec331ade78d7817cd87cd69b42eb0d6554adc7c4cbe2c673029e290923d6e`  
		Last Modified: Fri, 15 May 2020 21:11:56 GMT  
		Size: 40.6 MB (40592844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f9e7b05806cea62077a93baeafa4b02e9034ac32f8fe16332c18176f84a7da`  
		Last Modified: Mon, 08 Jun 2020 20:05:33 GMT  
		Size: 6.5 MB (6453252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4815bedaf52aa3ac7a09612db658c8fc15381048b373aaf9ba53989148085d`  
		Last Modified: Mon, 08 Jun 2020 20:05:31 GMT  
		Size: 4.3 KB (4291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ecfc939150ea35199c2feb8828852168308a256aff41765b9c4c7460ba77c4`  
		Last Modified: Mon, 08 Jun 2020 20:05:32 GMT  
		Size: 4.0 KB (3958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0d43b41607f6769e2fc114b5c6b3d24a7f0081f8d6256109b71cfae99834ce`  
		Last Modified: Mon, 08 Jun 2020 20:06:02 GMT  
		Size: 131.9 MB (131919728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f50f82c6068520ca59eeab9e30d988a0d52487f32eff5c7699a1d4c20bf9d03`  
		Last Modified: Mon, 08 Jun 2020 20:05:31 GMT  
		Size: 6.1 KB (6058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
