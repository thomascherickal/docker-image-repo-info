## `solr:latest`

```console
$ docker pull solr@sha256:ef1f2241c1aa51746aa3ad05570123eef128d98e91bc07336c37f2a1b37df7a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `solr:latest` - linux; amd64

```console
$ docker pull solr@sha256:67a78d7177c570ef633944e322a9132e25c54bbabbfbbdc81b446afb4d50cc9f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **500.5 MB (500520414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84c537842919fde3348c357279d4a3adc34076df9516bc2f4958820667423871`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:33 GMT
ADD file:8f7dc710e276f54a3a73d34b6b8fa261950a781d68ceb7401fa18dabc601c5a5 in / 
# Sat, 28 Dec 2019 04:23:34 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:58:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:58:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 04:59:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:54:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:54:40 GMT
ENV LANG=C.UTF-8
# Sat, 28 Dec 2019 08:54:40 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Sat, 28 Dec 2019 08:54:40 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 08:54:41 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 15 Jan 2020 21:28:39 GMT
ENV JAVA_VERSION=11.0.6
# Wed, 15 Jan 2020 21:28:39 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_
# Wed, 15 Jan 2020 21:28:39 GMT
ENV JAVA_URL_VERSION=11.0.6_10
# Wed, 15 Jan 2020 21:28:54 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac --version; 	java --version
# Wed, 15 Jan 2020 21:28:54 GMT
CMD ["jshell"]
# Wed, 15 Jan 2020 22:17:35 GMT
LABEL maintainer=Martijn Koster "mak-docker@greenhills.co.uk"
# Wed, 15 Jan 2020 22:17:35 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 22 Jan 2020 04:32:02 GMT
ARG SOLR_VERSION=8.4.1
# Wed, 22 Jan 2020 04:32:03 GMT
ARG SOLR_SHA512=2f210dae8d6a07b111ede22005fbd16aa6848900cda8adb352a33e08229783a170dddb529a7eb990f5157d4f5427c199df2114b9c0ffecdf9490a2ac07c6bb09
# Wed, 22 Jan 2020 04:32:03 GMT
ARG SOLR_KEYS=2085660D9C1FCCACC4A479A3BF160FF14992A24C
# Wed, 22 Jan 2020 04:32:03 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 22 Jan 2020 04:32:04 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 22 Jan 2020 04:32:11 GMT
# ARGS: SOLR_KEYS=2085660D9C1FCCACC4A479A3BF160FF14992A24C SOLR_SHA512=2f210dae8d6a07b111ede22005fbd16aa6848900cda8adb352a33e08229783a170dddb529a7eb990f5157d4f5427c199df2114b9c0ffecdf9490a2ac07c6bb09 SOLR_VERSION=8.4.1
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat;   rm -rf /var/lib/apt/lists/*
# Wed, 22 Jan 2020 04:32:11 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.4.1/solr-8.4.1.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.4.1/solr-8.4.1.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.4.1/solr-8.4.1.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 22 Jan 2020 04:32:12 GMT
ENV GOSU_VERSION=1.11
# Wed, 22 Jan 2020 04:32:12 GMT
ENV GOSU_KEY=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Wed, 22 Jan 2020 04:32:12 GMT
ENV TINI_VERSION=v0.18.0
# Wed, 22 Jan 2020 04:32:12 GMT
ENV TINI_KEY=595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7
# Wed, 22 Jan 2020 04:32:14 GMT
# ARGS: SOLR_KEYS=2085660D9C1FCCACC4A479A3BF160FF14992A24C SOLR_SHA512=2f210dae8d6a07b111ede22005fbd16aa6848900cda8adb352a33e08229783a170dddb529a7eb990f5157d4f5427c199df2114b9c0ffecdf9490a2ac07c6bb09 SOLR_VERSION=8.4.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 22 Jan 2020 04:32:17 GMT
# ARGS: SOLR_KEYS=2085660D9C1FCCACC4A479A3BF160FF14992A24C SOLR_SHA512=2f210dae8d6a07b111ede22005fbd16aa6848900cda8adb352a33e08229783a170dddb529a7eb990f5157d4f5427c199df2114b9c0ffecdf9490a2ac07c6bb09 SOLR_VERSION=8.4.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS $GOSU_KEY $TINI_KEY; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 22 Jan 2020 04:32:33 GMT
# ARGS: SOLR_KEYS=2085660D9C1FCCACC4A479A3BF160FF14992A24C SOLR_SHA512=2f210dae8d6a07b111ede22005fbd16aa6848900cda8adb352a33e08229783a170dddb529a7eb990f5157d4f5427c199df2114b9c0ffecdf9490a2ac07c6bb09 SOLR_VERSION=8.4.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   pkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";   wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$pkgArch";   wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$pkgArch.asc";   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   rm /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true;   wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-$pkgArch";   wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-$pkgArch.asc";   gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;   rm /usr/local/bin/tini.asc;   chmod +x /usr/local/bin/tini;   tini --version;   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 22 Jan 2020 04:32:34 GMT
COPY --chown=0:0dir:893f144aff80480bafb27e38f7755b66644279bd92a61929697c16884927c247 in /opt/docker-solr/scripts 
# Wed, 22 Jan 2020 04:32:34 GMT
VOLUME [/var/solr]
# Wed, 22 Jan 2020 04:32:34 GMT
EXPOSE 8983
# Wed, 22 Jan 2020 04:32:35 GMT
WORKDIR /opt/solr
# Wed, 22 Jan 2020 04:32:35 GMT
USER solr
# Wed, 22 Jan 2020 04:32:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jan 2020 04:32:35 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:146bd6a886182fde06fbf747470b1c89814bc8ab1c96fdf1aef6107171959fe6`  
		Last Modified: Sat, 28 Dec 2019 04:28:25 GMT  
		Size: 45.4 MB (45380744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9935d0c62ace92b388be202275e222007d6cac10b9c1f2c1ea63af38c09ea7ab`  
		Last Modified: Sat, 28 Dec 2019 05:04:30 GMT  
		Size: 10.8 MB (10797221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0efb86e80601b5bbdbb7c406426982c4202d339687c14c3941b364527e2249`  
		Last Modified: Sat, 28 Dec 2019 05:04:28 GMT  
		Size: 4.3 MB (4340114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e705a4c4fd310b96bfb3d7928428e65f0d3f5bad0cd0bda1434aee1d89418468`  
		Last Modified: Sat, 28 Dec 2019 05:04:45 GMT  
		Size: 50.1 MB (50072671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3bf7f7e874cd48fbdc9e46465264782687a52022f502b1e5eaf5f73287a877`  
		Last Modified: Sat, 28 Dec 2019 09:01:37 GMT  
		Size: 4.9 MB (4935355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c5c29a2d91cefd326445c6bf873e4ab9b6cf0c956d0b810bc37d2337c5192a`  
		Last Modified: Sat, 28 Dec 2019 09:01:36 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98049c8ee7f5c560e42b6661c87b9e2092f766fe7f477162ed7439501eadd60`  
		Last Modified: Wed, 15 Jan 2020 21:34:18 GMT  
		Size: 196.1 MB (196085897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b19de2d218887bfd853e3a525079186b346bc35141859c72029d33d7f507e6`  
		Last Modified: Wed, 22 Jan 2020 04:46:30 GMT  
		Size: 840.4 KB (840369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5442c4199123eb24f82c4b16edddd3a2d1611132cfcde91053434e9dee33300`  
		Last Modified: Wed, 22 Jan 2020 04:46:30 GMT  
		Size: 4.3 KB (4309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d189baf5efbf39020dcad257b7759fc8561fb4cd1e4ee32642e85a16e6a8d7`  
		Last Modified: Wed, 22 Jan 2020 04:46:30 GMT  
		Size: 154.4 KB (154442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1769ba269f7f6ae97dfc75f3411b27c5fac644f73140a4723c02b2425c231a90`  
		Last Modified: Wed, 22 Jan 2020 04:47:07 GMT  
		Size: 187.9 MB (187902802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef0bcc83843556a9b92406112af52e8083ab0e86216ed80dae88e7af142e7df`  
		Last Modified: Wed, 22 Jan 2020 04:46:30 GMT  
		Size: 6.3 KB (6271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:latest` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:f9c5e30aed1e0ad44c2f32b80dc5e465ab716047ae023102f2ad7a81377035ab
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **492.5 MB (492466993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd62314b4933ca11b138978da45b4592b9d4658c309cc8a5bc42dadf36782e20`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:15 GMT
ADD file:e439b3c387852978811a6a5a058745ebb9392da7e8936beb4f37ff076e656213 in / 
# Sat, 28 Dec 2019 04:43:17 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:15:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:15:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:16:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:26:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:26:24 GMT
ENV LANG=C.UTF-8
# Sat, 28 Dec 2019 18:26:26 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Sat, 28 Dec 2019 18:26:27 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 18:26:32 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 15 Jan 2020 21:50:16 GMT
ENV JAVA_VERSION=11.0.6
# Wed, 15 Jan 2020 21:50:17 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_
# Wed, 15 Jan 2020 21:50:17 GMT
ENV JAVA_URL_VERSION=11.0.6_10
# Wed, 15 Jan 2020 21:51:00 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac --version; 	java --version
# Wed, 15 Jan 2020 21:51:08 GMT
CMD ["jshell"]
# Wed, 15 Jan 2020 22:26:56 GMT
LABEL maintainer=Martijn Koster "mak-docker@greenhills.co.uk"
# Wed, 15 Jan 2020 22:26:56 GMT
LABEL repository=https://github.com/docker-solr/docker-solr
# Wed, 22 Jan 2020 03:50:17 GMT
ARG SOLR_VERSION=8.4.1
# Wed, 22 Jan 2020 03:50:18 GMT
ARG SOLR_SHA512=2f210dae8d6a07b111ede22005fbd16aa6848900cda8adb352a33e08229783a170dddb529a7eb990f5157d4f5427c199df2114b9c0ffecdf9490a2ac07c6bb09
# Wed, 22 Jan 2020 03:50:19 GMT
ARG SOLR_KEYS=2085660D9C1FCCACC4A479A3BF160FF14992A24C
# Wed, 22 Jan 2020 03:50:19 GMT
ARG SOLR_DOWNLOAD_URL
# Wed, 22 Jan 2020 03:50:20 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 22 Jan 2020 03:50:28 GMT
# ARGS: SOLR_KEYS=2085660D9C1FCCACC4A479A3BF160FF14992A24C SOLR_SHA512=2f210dae8d6a07b111ede22005fbd16aa6848900cda8adb352a33e08229783a170dddb529a7eb990f5157d4f5427c199df2114b9c0ffecdf9490a2ac07c6bb09 SOLR_VERSION=8.4.1
RUN set -ex;   apt-get update;   apt-get -y install acl dirmngr gpg lsof procps wget netcat;   rm -rf /var/lib/apt/lists/*
# Wed, 22 Jan 2020 03:50:29 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_CLOSER_URL=http://www.apache.org/dyn/closer.lua?filename=lucene/solr/8.4.1/solr-8.4.1.tgz&action=download SOLR_DIST_URL=https://www.apache.org/dist/lucene/solr/8.4.1/solr-8.4.1.tgz SOLR_ARCHIVE_URL=https://archive.apache.org/dist/lucene/solr/8.4.1/solr-8.4.1.tgz PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SOLR_INCLUDE=/etc/default/solr.in.sh SOLR_HOME=/var/solr/data SOLR_PID_DIR=/var/solr SOLR_LOGS_DIR=/var/solr/logs LOG4J_PROPS=/var/solr/log4j2.xml
# Wed, 22 Jan 2020 03:50:30 GMT
ENV GOSU_VERSION=1.11
# Wed, 22 Jan 2020 03:50:30 GMT
ENV GOSU_KEY=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Wed, 22 Jan 2020 03:50:31 GMT
ENV TINI_VERSION=v0.18.0
# Wed, 22 Jan 2020 03:50:32 GMT
ENV TINI_KEY=595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7
# Wed, 22 Jan 2020 03:50:33 GMT
# ARGS: SOLR_KEYS=2085660D9C1FCCACC4A479A3BF160FF14992A24C SOLR_SHA512=2f210dae8d6a07b111ede22005fbd16aa6848900cda8adb352a33e08229783a170dddb529a7eb990f5157d4f5427c199df2114b9c0ffecdf9490a2ac07c6bb09 SOLR_VERSION=8.4.1
RUN set -ex;   groupadd -r --gid "$SOLR_GID" "$SOLR_GROUP";   useradd -r --uid "$SOLR_UID" --gid "$SOLR_GID" "$SOLR_USER"
# Wed, 22 Jan 2020 03:50:37 GMT
# ARGS: SOLR_KEYS=2085660D9C1FCCACC4A479A3BF160FF14992A24C SOLR_SHA512=2f210dae8d6a07b111ede22005fbd16aa6848900cda8adb352a33e08229783a170dddb529a7eb990f5157d4f5427c199df2114b9c0ffecdf9490a2ac07c6bb09 SOLR_VERSION=8.4.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   mkdir -p "$GNUPGHOME";   chmod 700 "$GNUPGHOME";   echo "disable-ipv6" >> "$GNUPGHOME/dirmngr.conf";   for key in $SOLR_KEYS $GOSU_KEY $TINI_KEY; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;       gpg --batch --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Wed, 22 Jan 2020 03:50:56 GMT
# ARGS: SOLR_KEYS=2085660D9C1FCCACC4A479A3BF160FF14992A24C SOLR_SHA512=2f210dae8d6a07b111ede22005fbd16aa6848900cda8adb352a33e08229783a170dddb529a7eb990f5157d4f5427c199df2114b9c0ffecdf9490a2ac07c6bb09 SOLR_VERSION=8.4.1
RUN set -ex;   export GNUPGHOME="/tmp/gnupg_home";   pkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";   wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$pkgArch";   wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$pkgArch.asc";   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   rm /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true;   wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-$pkgArch";   wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-$pkgArch.asc";   gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;   rm /usr/local/bin/tini.asc;   chmod +x /usr/local/bin/tini;   tini --version;   MAX_REDIRECTS=1;   if [ -n "$SOLR_DOWNLOAD_URL" ]; then     MAX_REDIRECTS=4;     SKIP_GPG_CHECK=true;   elif [ -n "$SOLR_DOWNLOAD_SERVER" ]; then     SOLR_DOWNLOAD_URL="$SOLR_DOWNLOAD_SERVER/$SOLR_VERSION/solr-$SOLR_VERSION.tgz";   fi;   for url in $SOLR_DOWNLOAD_URL $SOLR_CLOSER_URL $SOLR_DIST_URL $SOLR_ARCHIVE_URL; do     if [ -f "/opt/solr-$SOLR_VERSION.tgz" ]; then break; fi;     echo "downloading $url";     if wget -t 10 --max-redirect $MAX_REDIRECTS --retry-connrefused -nv "$url" -O "/opt/solr-$SOLR_VERSION.tgz"; then break; else rm -f "/opt/solr-$SOLR_VERSION.tgz"; fi;   done;   if [ ! -f "/opt/solr-$SOLR_VERSION.tgz" ]; then echo "failed all download attempts for solr-$SOLR_VERSION.tgz"; exit 1; fi;   if [ -z "$SKIP_GPG_CHECK" ]; then     echo "downloading $SOLR_ARCHIVE_URL.asc";     wget -nv "$SOLR_ARCHIVE_URL.asc" -O "/opt/solr-$SOLR_VERSION.tgz.asc";     echo "$SOLR_SHA512 */opt/solr-$SOLR_VERSION.tgz" | sha512sum -c -;     (>&2 ls -l "/opt/solr-$SOLR_VERSION.tgz" "/opt/solr-$SOLR_VERSION.tgz.asc");     gpg --batch --verify "/opt/solr-$SOLR_VERSION.tgz.asc" "/opt/solr-$SOLR_VERSION.tgz";   else     echo "Skipping GPG validation due to non-Apache build";   fi;   tar -C /opt --extract --file "/opt/solr-$SOLR_VERSION.tgz";   (cd /opt; ln -s "solr-$SOLR_VERSION" solr);   rm "/opt/solr-$SOLR_VERSION.tgz"*;   rm -Rf /opt/solr/docs/;   mkdir -p /opt/solr/server/solr/lib /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R 0:0 "/opt/solr-$SOLR_VERSION";   find "/opt/solr-$SOLR_VERSION" -type d -print0 | xargs -0 chmod 0755;   find "/opt/solr-$SOLR_VERSION" -type f -print0 | xargs -0 chmod 0644;   chmod -R 0755 "/opt/solr-$SOLR_VERSION/bin" "/opt/solr-$SOLR_VERSION/contrib/prometheus-exporter/bin/solr-exporter" /opt/solr-$SOLR_VERSION/server/scripts/cloud-scripts;   cp /opt/solr/bin/solr.in.sh /etc/default/solr.in.sh;   mv /opt/solr/bin/solr.in.sh /opt/solr/bin/solr.in.sh.orig;   mv /opt/solr/bin/solr.in.cmd /opt/solr/bin/solr.in.cmd.orig;   chown root:0 /etc/default/solr.in.sh;   chmod 0664 /etc/default/solr.in.sh;   mkdir -p /var/solr/data /var/solr/logs;   (cd /opt/solr/server/solr; cp solr.xml zoo.cfg /var/solr/data/);   cp /opt/solr/server/resources/log4j2.xml /var/solr/log4j2.xml;   find /var/solr -type d -print0 | xargs -0 chmod 0770;   find /var/solr -type f -print0 | xargs -0 chmod 0660;   sed -i -e "s/\"\$(whoami)\" == \"root\"/\$(id -u) == 0/" /opt/solr/bin/solr;   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr;   chown -R "0:0" /opt/solr-$SOLR_VERSION /docker-entrypoint-initdb.d /opt/docker-solr;   chown -R "$SOLR_USER:0" /var/solr;   { command -v gpgconf; gpgconf --kill all || :; };   rm -r "$GNUPGHOME"
# Wed, 22 Jan 2020 03:50:58 GMT
COPY --chown=0:0dir:893f144aff80480bafb27e38f7755b66644279bd92a61929697c16884927c247 in /opt/docker-solr/scripts 
# Wed, 22 Jan 2020 03:50:59 GMT
VOLUME [/var/solr]
# Wed, 22 Jan 2020 03:51:00 GMT
EXPOSE 8983
# Wed, 22 Jan 2020 03:51:01 GMT
WORKDIR /opt/solr
# Wed, 22 Jan 2020 03:51:01 GMT
USER solr
# Wed, 22 Jan 2020 03:51:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jan 2020 03:51:03 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:d07bcf5901dfa793fa6b2c4c617e86bcef315b0b092cbfd1a929eefedaf8e3f2`  
		Last Modified: Sat, 28 Dec 2019 04:48:57 GMT  
		Size: 43.2 MB (43166476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f31062581dadb1f69c43e9441040dd46788bf13ae51f20c66929fac82b506b`  
		Last Modified: Sat, 28 Dec 2019 06:24:15 GMT  
		Size: 9.7 MB (9748258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62337a296a607f48a5dc3a7c07639360d98e0e78982ca8e459c832719012f12`  
		Last Modified: Sat, 28 Dec 2019 06:24:15 GMT  
		Size: 4.1 MB (4094448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403697a3e152c7a38ddb9175a90ed2dac97d780421c35949ff80cd67a7d4e596`  
		Last Modified: Sat, 28 Dec 2019 06:24:36 GMT  
		Size: 48.0 MB (48024191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb89ca5cad13a1953df62bf1392d84738a27f915e8049436d1bfc58ab898c022`  
		Last Modified: Sat, 28 Dec 2019 18:30:25 GMT  
		Size: 4.8 MB (4843239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b50f966e01f320063d779b3cdea53b1226b0fd6704a5bb66145bbec8e0c0a6`  
		Last Modified: Sat, 28 Dec 2019 18:30:24 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab9d6d1760dc73974164c8451097afb6038c7a49abc2e2e7e23766f1c041c21`  
		Last Modified: Wed, 15 Jan 2020 21:54:19 GMT  
		Size: 193.8 MB (193754823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9468a4ba208388d427e859930e180120b7e7c67e87cf8539f1c9b4f8bb51e2e2`  
		Last Modified: Wed, 22 Jan 2020 04:05:05 GMT  
		Size: 833.8 KB (833775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa6812bf2050edcf5e9ff526c1d9f688f757ae164f448dd0305427385ba85036`  
		Last Modified: Wed, 22 Jan 2020 04:05:05 GMT  
		Size: 4.3 KB (4348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ca4d3f594923940c81730fb86cc0a5bb1953ff01c4f8eb3309697b261b3bb6`  
		Last Modified: Wed, 22 Jan 2020 04:05:05 GMT  
		Size: 154.5 KB (154471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a74a247106dde51b77c35cb608c0527ccf0025818af307adbf53af2336d659f`  
		Last Modified: Wed, 22 Jan 2020 04:05:38 GMT  
		Size: 187.8 MB (187836446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cad0a24069f431d06a50fda47a857eba860c772bca36b6f1451e8035ed75cb`  
		Last Modified: Wed, 22 Jan 2020 04:05:05 GMT  
		Size: 6.3 KB (6299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
