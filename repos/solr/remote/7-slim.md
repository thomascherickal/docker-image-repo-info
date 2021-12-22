## `solr:7-slim`

```console
$ docker pull solr@sha256:a0690cc25c7be7382c433825b2609f06f5890b4dd740ed3a14f2e7ad7bf04c98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `solr:7-slim` - linux; amd64

```console
$ docker pull solr@sha256:d2c0b92ccaffb317a3e76a2f0af03fe36cd61efe2f7dfe1947a3678f6e80039a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.5 MB (258474817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:091d974e42734e7400de10c4b41557443119cfeb43263c289295505e601964fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 22:57:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:02:54 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 21 Dec 2021 23:02:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 23:02:55 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:02:55 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:02:55 GMT
ENV JAVA_VERSION=11.0.13
# Tue, 21 Dec 2021 23:05:10 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Wed, 22 Dec 2021 16:08:22 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Wed, 22 Dec 2021 16:08:22 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 22 Dec 2021 16:28:58 GMT
ARG SOLR_VERSION=7.7.3
# Wed, 22 Dec 2021 16:28:58 GMT
ARG SOLR_SHA512=ca9200c18cc19ab723fd4d10f257e27eb81dc8bc33401ebc4eb99178faf4033a2684f0f8b12ae7b659cfeb0f4c9d9e24aaac518a4e00fd28b69854a359a666ed
# Wed, 22 Dec 2021 16:28:58 GMT
ARG SOLR_KEYS=CFCE5FBB920C3C745CEEE084C38FF5EC3FCFDB3E
# Wed, 22 Dec 2021 16:28:58 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 22 Dec 2021 16:28:58 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 22 Dec 2021 16:29:06 GMT
# ARGS: SOLR_KEYS=CFCE5FBB920C3C745CEEE084C38FF5EC3FCFDB3E SOLR_SHA512=ca9200c18cc19ab723fd4d10f257e27eb81dc8bc33401ebc4eb99178faf4033a2684f0f8b12ae7b659cfeb0f4c9d9e24aaac518a4e00fd28b69854a359a666ed SOLR_VERSION=7.7.3
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Wed, 22 Dec 2021 16:29:07 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/7.7.3/solr-7.7.3.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/7.7.3/solr-7.7.3.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/7.7.3/solr-7.7.3.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 16:29:07 GMT
# ARGS: SOLR_KEYS=CFCE5FBB920C3C745CEEE084C38FF5EC3FCFDB3E SOLR_SHA512=ca9200c18cc19ab723fd4d10f257e27eb81dc8bc33401ebc4eb99178faf4033a2684f0f8b12ae7b659cfeb0f4c9d9e24aaac518a4e00fd28b69854a359a666ed SOLR_VERSION=7.7.3
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 22 Dec 2021 16:29:11 GMT
# ARGS: SOLR_KEYS=CFCE5FBB920C3C745CEEE084C38FF5EC3FCFDB3E SOLR_SHA512=ca9200c18cc19ab723fd4d10f257e27eb81dc8bc33401ebc4eb99178faf4033a2684f0f8b12ae7b659cfeb0f4c9d9e24aaac518a4e00fd28b69854a359a666ed SOLR_VERSION=7.7.3
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 22 Dec 2021 16:29:38 GMT
# ARGS: SOLR_KEYS=CFCE5FBB920C3C745CEEE084C38FF5EC3FCFDB3E SOLR_SHA512=ca9200c18cc19ab723fd4d10f257e27eb81dc8bc33401ebc4eb99178faf4033a2684f0f8b12ae7b659cfeb0f4c9d9e24aaac518a4e00fd28b69854a359a666ed SOLR_VERSION=7.7.3
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   mv "/opt/solr-$SOLR_VERSION" /opt/solr;   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   mkdir -p /opt/solr/server/solr/mycores /opt/solr/server/logs /opt/mysolrhome;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   if [ -f "/opt/solr/contrib/prometheus-exporter/bin/solr-exporter" ]; then chmod 0755 "/opt/solr/contrib/prometheus-exporter/bin/solr-exporter"; fi;   chmod -R 0755 /opt/solr/server/scripts/cloud-scripts;   chown -R "$SOLR_USER:$SOLR_GROUP" /opt/solr /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:$SOLR_GROUP" /opt/mysolrhome;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 22 Dec 2021 16:29:39 GMT
COPY --chown=solr:solrdir:47673e85b88ff0771446ce93142f786f59e74a0232d547ae66ced7f9058c0a14 in /opt/docker-solr/scripts 
# Wed, 22 Dec 2021 16:29:39 GMT
EXPOSE 8983
# Wed, 22 Dec 2021 16:29:39 GMT
WORKDIR /opt/solr
# Wed, 22 Dec 2021 16:29:40 GMT
USER solr
# Wed, 22 Dec 2021 16:29:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 16:29:40 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbde5250315969db657b55bd8b2f5507fb659c0cf7f135edc84b684ffeab44a`  
		Last Modified: Tue, 21 Dec 2021 23:14:38 GMT  
		Size: 1.6 MB (1582039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202a34e7968ed05e00991c2da849aeaf70fca2714d1f18b942ead99ba30958dd`  
		Last Modified: Tue, 21 Dec 2021 23:23:49 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4231e30efc2126ab017a98d2510ff7a2693f257baa2160d17c8618b0d38c08`  
		Last Modified: Tue, 21 Dec 2021 23:26:39 GMT  
		Size: 47.1 MB (47104025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481baf72a636a5669cfa0510cee716b3c45515de6ec4be7f2bbf06eab1a68381`  
		Last Modified: Wed, 22 Dec 2021 16:43:27 GMT  
		Size: 6.9 MB (6902372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36b2fa015dd65398057b30875ae898dcc18378d12ffc352aae6709038593ddf`  
		Last Modified: Wed, 22 Dec 2021 16:43:26 GMT  
		Size: 4.3 KB (4286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd511b53e0c8eb80b534f4c9b3a99a894643be79e034491994d13dd9c981e55`  
		Last Modified: Wed, 22 Dec 2021 16:43:26 GMT  
		Size: 2.9 KB (2909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29310c1e63f21144e952b09203bd24dea50a959a044b41a9a3c684ce3422504f`  
		Last Modified: Wed, 22 Dec 2021 16:43:34 GMT  
		Size: 171.5 MB (171515232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590c66b75a55b2ec50255a99f746fd59bbdb7a026adeb59cbf5225c4e9a91449`  
		Last Modified: Wed, 22 Dec 2021 16:43:25 GMT  
		Size: 6.1 KB (6117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:7-slim` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:92940cb6e38bbf0e4fc6e1a8da885a54c73cc9b6fffe6f7c270ad2bb324530ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.7 MB (255720186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9317c6443339ed04c677f7e81b7d1ebaebc2606c57b69eefc9a183f55b29d1bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:53:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:00:21 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 21 Dec 2021 03:00:22 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 03:00:23 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 03:00:24 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:00:25 GMT
ENV JAVA_VERSION=11.0.13
# Tue, 21 Dec 2021 03:03:01 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 21 Dec 2021 22:47:31 GMT
LABEL maintainer=The Apache Lucene/Solr Project
# Tue, 21 Dec 2021 22:47:32 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Tue, 21 Dec 2021 23:23:54 GMT
ARG SOLR_VERSION=7.7.3
# Tue, 21 Dec 2021 23:23:54 GMT
ARG SOLR_SHA512=ca9200c18cc19ab723fd4d10f257e27eb81dc8bc33401ebc4eb99178faf4033a2684f0f8b12ae7b659cfeb0f4c9d9e24aaac518a4e00fd28b69854a359a666ed
# Tue, 21 Dec 2021 23:23:55 GMT
ARG SOLR_KEYS=CFCE5FBB920C3C745CEEE084C38FF5EC3FCFDB3E
# Tue, 21 Dec 2021 23:23:56 GMT
ARG SOLR_DOWNLOAD_URL
# Tue, 21 Dec 2021 23:23:57 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 21 Dec 2021 23:24:04 GMT
# ARGS: SOLR_KEYS=CFCE5FBB920C3C745CEEE084C38FF5EC3FCFDB3E SOLR_SHA512=ca9200c18cc19ab723fd4d10f257e27eb81dc8bc33401ebc4eb99178faf4033a2684f0f8b12ae7b659cfeb0f4c9d9e24aaac518a4e00fd28b69854a359a666ed SOLR_VERSION=7.7.3
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat gosu tini;   rm -rf /var/lib/apt/lists/*;   cd /usr/local/bin; wget -nv https://github.com/apangin/jattach/releases/download/v1.5/jattach; chmod 755 jattach;   echo >jattach.sha512 "d8eedbb3e192a8596c08efedff99b9acf1075331e1747107c07cdb1718db2abe259ef168109e46bd4cf80d47d43028ff469f95e6ddcbdda4d7ffa73a20e852f9  jattach";   sha512sum -c jattach.sha512; rm jattach.sha512
# Tue, 21 Dec 2021 23:24:05 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/7.7.3/solr-7.7.3.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/7.7.3/solr-7.7.3.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/7.7.3/solr-7.7.3.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:24:06 GMT
# ARGS: SOLR_KEYS=CFCE5FBB920C3C745CEEE084C38FF5EC3FCFDB3E SOLR_SHA512=ca9200c18cc19ab723fd4d10f257e27eb81dc8bc33401ebc4eb99178faf4033a2684f0f8b12ae7b659cfeb0f4c9d9e24aaac518a4e00fd28b69854a359a666ed SOLR_VERSION=7.7.3
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Tue, 21 Dec 2021 23:24:11 GMT
# ARGS: SOLR_KEYS=CFCE5FBB920C3C745CEEE084C38FF5EC3FCFDB3E SOLR_SHA512=ca9200c18cc19ab723fd4d10f257e27eb81dc8bc33401ebc4eb99178faf4033a2684f0f8b12ae7b659cfeb0f4c9d9e24aaac518a4e00fd28b69854a359a666ed SOLR_VERSION=7.7.3
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Tue, 21 Dec 2021 23:25:39 GMT
# ARGS: SOLR_KEYS=CFCE5FBB920C3C745CEEE084C38FF5EC3FCFDB3E SOLR_SHA512=ca9200c18cc19ab723fd4d10f257e27eb81dc8bc33401ebc4eb99178faf4033a2684f0f8b12ae7b659cfeb0f4c9d9e24aaac518a4e00fd28b69854a359a666ed SOLR_VERSION=7.7.3
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   mv "/opt/solr-$SOLR_VERSION" /opt/solr;   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/ /opt/solr/dist/{solr-core-$SOLR_VERSION.jar,solr-solrj-$SOLR_VERSION.jar,solrj-lib,solr-test-framework-$SOLR_VERSION.jar,test-framework};   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   mkdir -p /opt/solr/server/solr/mycores /opt/solr/server/logs /opt/mysolrhome;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   if [ -f "/opt/solr/contrib/prometheus-exporter/bin/solr-exporter" ]; then chmod 0755 "/opt/solr/contrib/prometheus-exporter/bin/solr-exporter"; fi;   chmod -R 0755 /opt/solr/server/scripts/cloud-scripts;   chown -R "$SOLR_USER:$SOLR_GROUP" /opt/solr /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:$SOLR_GROUP" /opt/mysolrhome;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Tue, 21 Dec 2021 23:25:40 GMT
COPY --chown=solr:solrdir:47673e85b88ff0771446ce93142f786f59e74a0232d547ae66ced7f9058c0a14 in /opt/docker-solr/scripts 
# Tue, 21 Dec 2021 23:25:40 GMT
EXPOSE 8983
# Tue, 21 Dec 2021 23:25:41 GMT
WORKDIR /opt/solr
# Tue, 21 Dec 2021 23:25:42 GMT
USER solr
# Tue, 21 Dec 2021 23:25:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 23:25:44 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3380d13c6c3ddd0cc31ece5496ad1481500cb07b7feb31c81bc907a9a1ad71`  
		Last Modified: Tue, 21 Dec 2021 03:15:59 GMT  
		Size: 1.6 MB (1565954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabbccc2438417914e147407ab3a9272b6ce23cf33faf491941239ed4c8a9c75`  
		Last Modified: Tue, 21 Dec 2021 03:26:29 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5912a65c12f962652970e8049fdf1736a2da8805d76bf43f8b8f716d7094dc64`  
		Last Modified: Tue, 21 Dec 2021 03:29:25 GMT  
		Size: 46.0 MB (45975698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa779eb4fe37ab0dfb4752e27705f9346ec9b56cafcd072121a534b0bf1c1c13`  
		Last Modified: Tue, 21 Dec 2021 23:39:50 GMT  
		Size: 6.6 MB (6600943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab2f8f423e5ae7770f09be1e44f376accfd951b73de5cb8d732abb7211c142c`  
		Last Modified: Tue, 21 Dec 2021 23:39:49 GMT  
		Size: 4.2 KB (4202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c2145c36e99054f9c119b0e5bc61d72f6308519aad9ca1ec197d938c28d958`  
		Last Modified: Tue, 21 Dec 2021 23:39:49 GMT  
		Size: 2.9 KB (2879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963950b33e91717aa265d5a22d7b759cd61db5d391c219d54bfabc41aaf83a24`  
		Last Modified: Tue, 21 Dec 2021 23:40:03 GMT  
		Size: 171.5 MB (171520417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1fbbd356595621aad6987d1ba085733c9920234036c5a329152f5f5415e205`  
		Last Modified: Tue, 21 Dec 2021 23:39:49 GMT  
		Size: 6.1 KB (6089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
