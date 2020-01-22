## `solr:8-slim`

```console
$ docker pull solr@sha256:deb505ff224013424ef350b6ff33327d9d30a09a8e590b5cb7e13280500f71bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `solr:8-slim` - linux; amd64

```console
$ docker pull solr@sha256:d6362dabbd8cb4e9d07a969d1c7c11aae933914354911fd3d444bcbd2d022032
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **420.1 MB (420088577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e501f4e55e34082666f52e5b4404bfa0a76df85117fab3bb7d2ace989b80e1f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 08:50:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:50:14 GMT
ENV LANG=C.UTF-8
# Sat, 28 Dec 2019 08:55:04 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Sat, 28 Dec 2019 08:55:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 08:55:05 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 15 Jan 2020 21:28:59 GMT
ENV JAVA_VERSION=11.0.6
# Wed, 15 Jan 2020 21:29:00 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_
# Wed, 15 Jan 2020 21:29:00 GMT
ENV JAVA_URL_VERSION=11.0.6_10
# Wed, 15 Jan 2020 21:29:18 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac --version; 	java --version
# Wed, 15 Jan 2020 21:29:19 GMT
CMD ["jshell"]
# Wed, 15 Jan 2020 22:18:03 GMT
LABEL maintainer=Martijn Koster "mak-docker@greenhills.co.uk"
# Wed, 15 Jan 2020 22:18:03 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 22 Jan 2020 04:32:41 GMT
ARG SOLR_VERSION=8.4.1
# Wed, 22 Jan 2020 04:32:42 GMT
ARG SOLR_SHA512=2f210dae8d6a07b111ede22005fbd16aa6848900cda8adb352a33e08229783a170dddb529a7eb990f5157d4f5427c199df2114b9c0ffecdf9490a2ac07c6bb09
# Wed, 22 Jan 2020 04:32:42 GMT
ARG SOLR_KEYS=2085660D9C1FCCACC4A479A3BF160FF14992A24C
# Wed, 22 Jan 2020 04:32:42 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 22 Jan 2020 04:32:42 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 22 Jan 2020 04:32:52 GMT
# ARGS: SOLR_KEYS=2085660D9C1FCCACC4A479A3BF160FF14992A24C SOLR_SHA512=2f210dae8d6a07b111ede22005fbd16aa6848900cda8adb352a33e08229783a170dddb529a7eb990f5157d4f5427c199df2114b9c0ffecdf9490a2ac07c6bb09 SOLR_VERSION=8.4.1
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat;   rm -rf /var/lib/apt/lists/*
# Wed, 22 Jan 2020 04:32:52 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.4.1/solr-8.4.1.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.4.1/solr-8.4.1.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.4.1/solr-8.4.1.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 22 Jan 2020 04:32:52 GMT
ENV GOSU_VERSION=1.11
# Wed, 22 Jan 2020 04:32:52 GMT
ENV GOSU_KEY=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Wed, 22 Jan 2020 04:32:52 GMT
ENV TINI_VERSION=v0.18.0
# Wed, 22 Jan 2020 04:32:52 GMT
ENV TINI_KEY=595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7
# Wed, 22 Jan 2020 04:32:53 GMT
# ARGS: SOLR_KEYS=2085660D9C1FCCACC4A479A3BF160FF14992A24C SOLR_SHA512=2f210dae8d6a07b111ede22005fbd16aa6848900cda8adb352a33e08229783a170dddb529a7eb990f5157d4f5427c199df2114b9c0ffecdf9490a2ac07c6bb09 SOLR_VERSION=8.4.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 22 Jan 2020 04:32:54 GMT
# ARGS: SOLR_KEYS=2085660D9C1FCCACC4A479A3BF160FF14992A24C SOLR_SHA512=2f210dae8d6a07b111ede22005fbd16aa6848900cda8adb352a33e08229783a170dddb529a7eb990f5157d4f5427c199df2114b9c0ffecdf9490a2ac07c6bb09 SOLR_VERSION=8.4.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS $GOSU_KEY $TINI_KEY; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 22 Jan 2020 04:33:08 GMT
# ARGS: SOLR_KEYS=2085660D9C1FCCACC4A479A3BF160FF14992A24C SOLR_SHA512=2f210dae8d6a07b111ede22005fbd16aa6848900cda8adb352a33e08229783a170dddb529a7eb990f5157d4f5427c199df2114b9c0ffecdf9490a2ac07c6bb09 SOLR_VERSION=8.4.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   pkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";   wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$pkgArch";   wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$pkgArch.asc";   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   rm /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true;   wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-$pkgArch";   wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-$pkgArch.asc";   gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;   rm /usr/local/bin/tini.asc;   chmod +x /usr/local/bin/tini;   tini --version;   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 22 Jan 2020 04:33:08 GMT
COPY --chown=0:0dir:893f144aff80480bafb27e38f7755b66644279bd92a61929697c16884927c247 in /opt/docker-solr/scripts 
# Wed, 22 Jan 2020 04:33:08 GMT
VOLUME [/var/solr]
# Wed, 22 Jan 2020 04:33:08 GMT
EXPOSE 8983
# Wed, 22 Jan 2020 04:33:09 GMT
WORKDIR /opt/solr
# Wed, 22 Jan 2020 04:33:09 GMT
USER solr
# Wed, 22 Jan 2020 04:33:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jan 2020 04:33:09 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e866b0959566a21a8fa7eb2f7f12da0d12aa3498d6c31bb25a6ede1fa632ac2`  
		Last Modified: Sat, 28 Dec 2019 08:58:53 GMT  
		Size: 3.2 MB (3249103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5d513ad8c41aa8c04e4398490b3ccfa0ee2ad433dbc3038dc96cd48a9366cf`  
		Last Modified: Sat, 28 Dec 2019 09:02:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54c89f62fafed16a614c5931a99e21ce97663558dee27c19c54051a9dfe1cf7`  
		Last Modified: Wed, 15 Jan 2020 21:34:46 GMT  
		Size: 196.3 MB (196343133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9412c27fc1eafe88d95db881089aa109818dc5e38896dc68bf58c68ce43605`  
		Last Modified: Wed, 22 Jan 2020 04:47:16 GMT  
		Size: 5.5 MB (5465814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c574891ab690467616d89bf88be0216981fdc4002dc8d0cf148835c2148dbff`  
		Last Modified: Wed, 22 Jan 2020 04:47:14 GMT  
		Size: 4.3 KB (4286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7cf8d3c76b187ac3fca7102cc1443ad012204ce1db9542b47bfbd4ff7ae1d3`  
		Last Modified: Wed, 22 Jan 2020 04:47:14 GMT  
		Size: 24.4 KB (24359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb0ba769dbbc6ff7b6bdcc8d3c7e3f8ee24b5d73ccdfa07aeb91d0af3d6a33f`  
		Last Modified: Wed, 22 Jan 2020 04:47:34 GMT  
		Size: 187.9 MB (187903123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f401a6ecd27e0736556c07167c62f1d01da527561c8b163b41584504b0ff1e7`  
		Last Modified: Wed, 22 Jan 2020 04:47:14 GMT  
		Size: 6.3 KB (6273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:8-slim` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:61a64ee57620f010853969c29b6eabdc053c3d8e909d9c5b305e39b8f3a6e189
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.3 MB (416297195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8df7b2dcf67fc5241968984e45f662e05aa47d3621fed941880f259e61affc2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 18:27:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:27:44 GMT
ENV LANG=C.UTF-8
# Sat, 28 Dec 2019 18:27:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Sat, 28 Dec 2019 18:27:46 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 18:27:48 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 15 Jan 2020 21:51:24 GMT
ENV JAVA_VERSION=11.0.6
# Wed, 15 Jan 2020 21:51:27 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_
# Wed, 15 Jan 2020 21:51:32 GMT
ENV JAVA_URL_VERSION=11.0.6_10
# Wed, 15 Jan 2020 21:52:22 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac --version; 	java --version
# Wed, 15 Jan 2020 21:52:24 GMT
CMD ["jshell"]
# Wed, 15 Jan 2020 22:27:42 GMT
LABEL maintainer=Martijn Koster "mak-docker@greenhills.co.uk"
# Wed, 15 Jan 2020 22:27:43 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 22 Jan 2020 03:51:12 GMT
ARG SOLR_VERSION=8.4.1
# Wed, 22 Jan 2020 03:51:13 GMT
ARG SOLR_SHA512=2f210dae8d6a07b111ede22005fbd16aa6848900cda8adb352a33e08229783a170dddb529a7eb990f5157d4f5427c199df2114b9c0ffecdf9490a2ac07c6bb09
# Wed, 22 Jan 2020 03:51:14 GMT
ARG SOLR_KEYS=2085660D9C1FCCACC4A479A3BF160FF14992A24C
# Wed, 22 Jan 2020 03:51:15 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 22 Jan 2020 03:51:16 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 22 Jan 2020 03:51:33 GMT
# ARGS: SOLR_KEYS=2085660D9C1FCCACC4A479A3BF160FF14992A24C SOLR_SHA512=2f210dae8d6a07b111ede22005fbd16aa6848900cda8adb352a33e08229783a170dddb529a7eb990f5157d4f5427c199df2114b9c0ffecdf9490a2ac07c6bb09 SOLR_VERSION=8.4.1
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat;   rm -rf /var/lib/apt/lists/*
# Wed, 22 Jan 2020 03:51:34 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.4.1/solr-8.4.1.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.4.1/solr-8.4.1.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.4.1/solr-8.4.1.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 22 Jan 2020 03:51:35 GMT
ENV GOSU_VERSION=1.11
# Wed, 22 Jan 2020 03:51:35 GMT
ENV GOSU_KEY=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Wed, 22 Jan 2020 03:51:36 GMT
ENV TINI_VERSION=v0.18.0
# Wed, 22 Jan 2020 03:51:36 GMT
ENV TINI_KEY=595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7
# Wed, 22 Jan 2020 03:51:38 GMT
# ARGS: SOLR_KEYS=2085660D9C1FCCACC4A479A3BF160FF14992A24C SOLR_SHA512=2f210dae8d6a07b111ede22005fbd16aa6848900cda8adb352a33e08229783a170dddb529a7eb990f5157d4f5427c199df2114b9c0ffecdf9490a2ac07c6bb09 SOLR_VERSION=8.4.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 22 Jan 2020 03:51:41 GMT
# ARGS: SOLR_KEYS=2085660D9C1FCCACC4A479A3BF160FF14992A24C SOLR_SHA512=2f210dae8d6a07b111ede22005fbd16aa6848900cda8adb352a33e08229783a170dddb529a7eb990f5157d4f5427c199df2114b9c0ffecdf9490a2ac07c6bb09 SOLR_VERSION=8.4.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS $GOSU_KEY $TINI_KEY; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 22 Jan 2020 03:51:56 GMT
# ARGS: SOLR_KEYS=2085660D9C1FCCACC4A479A3BF160FF14992A24C SOLR_SHA512=2f210dae8d6a07b111ede22005fbd16aa6848900cda8adb352a33e08229783a170dddb529a7eb990f5157d4f5427c199df2114b9c0ffecdf9490a2ac07c6bb09 SOLR_VERSION=8.4.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   pkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";   wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$pkgArch";   wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$pkgArch.asc";   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   rm /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true;   wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-$pkgArch";   wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-$pkgArch.asc";   gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;   rm /usr/local/bin/tini.asc;   chmod +x /usr/local/bin/tini;   tini --version;   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 22 Jan 2020 03:51:58 GMT
COPY --chown=0:0dir:893f144aff80480bafb27e38f7755b66644279bd92a61929697c16884927c247 in /opt/docker-solr/scripts 
# Wed, 22 Jan 2020 03:51:59 GMT
VOLUME [/var/solr]
# Wed, 22 Jan 2020 03:51:59 GMT
EXPOSE 8983
# Wed, 22 Jan 2020 03:52:00 GMT
WORKDIR /opt/solr
# Wed, 22 Jan 2020 03:52:01 GMT
USER solr
# Wed, 22 Jan 2020 03:52:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jan 2020 03:52:02 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac316ff102c6235e01468230219a62f821a499509c6730780405e333e112a586`  
		Last Modified: Sat, 28 Dec 2019 18:31:14 GMT  
		Size: 3.1 MB (3101169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f89ba1ce3f076ce617159b446596e6c42e70669a63d47a41caa23e655fb1fbb`  
		Last Modified: Sat, 28 Dec 2019 18:31:14 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47d5641004e32f3faab9cacbc487b1a0274916c187c8a6466e725f9573faa67`  
		Last Modified: Wed, 15 Jan 2020 21:54:58 GMT  
		Size: 194.0 MB (194015250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab369091b7f99df0001ef46aa6a3a96882182b8ea7f4d591075e20135966fbd`  
		Last Modified: Wed, 22 Jan 2020 04:05:49 GMT  
		Size: 5.5 MB (5458223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd79a9b3d99d194239bb942e5f1f1a4cd6e1fc96d2786c8198f4064f90f43636`  
		Last Modified: Wed, 22 Jan 2020 04:05:48 GMT  
		Size: 4.3 KB (4324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681c025980352215a6c694c97a35983f7e42a24015fb993f4ded1f1a200bd468`  
		Last Modified: Wed, 22 Jan 2020 04:05:48 GMT  
		Size: 24.4 KB (24401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10512b8301568c1aa548c67177b6cab017151b55f3f26f1e4d947ddfe9cf6089`  
		Last Modified: Wed, 22 Jan 2020 04:06:09 GMT  
		Size: 187.8 MB (187836614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67f298b20458a75188ca502765811ef1e65fe6241709ee30a03077819cf4e82`  
		Last Modified: Wed, 22 Jan 2020 04:05:48 GMT  
		Size: 6.3 KB (6300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
