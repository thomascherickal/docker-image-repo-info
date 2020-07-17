## `neo4j:latest`

```console
$ docker pull neo4j@sha256:91682adb53e701f3dfee484cc09d315e574b8e55568ce67dd7d12a205dcd4337
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:latest` - linux; amd64

```console
$ docker pull neo4j@sha256:bc729296b60c5b588a62424942a16231d00418fc160a8b936cd727263d79c08c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.4 MB (348433002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e5e80b06a82f6c802cceb957c470c71634b08302dc615dd1a9a8c76bf74fad`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:56 GMT
ADD file:4d35f6c8bbbe6801cc5f44989730fb6d349a644ecb36eca481e7df25842d6321 in / 
# Tue, 09 Jun 2020 01:20:56 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 16:34:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 16:34:37 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 16:37:19 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 09 Jun 2020 16:37:19 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 16:37:20 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Jul 2020 22:39:07 GMT
ENV JAVA_VERSION=11.0.8
# Thu, 16 Jul 2020 22:39:07 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jdk_
# Thu, 16 Jul 2020 22:39:08 GMT
ENV JAVA_URL_VERSION=11.0.8_10
# Thu, 16 Jul 2020 22:39:26 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac --version; 	java --version
# Thu, 16 Jul 2020 22:39:27 GMT
CMD ["jshell"]
# Thu, 16 Jul 2020 23:20:38 GMT
ENV NEO4J_SHA256=4f663a520bec40dfd0b1972feb3cf93af321c230b448adb6dc917717e67a1271 NEO4J_TARBALL=neo4j-community-4.1.1-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Jul 2020 23:20:38 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.1.1-unix.tar.gz
# Thu, 16 Jul 2020 23:20:38 GMT
ARG TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Jul 2020 23:20:38 GMT
ARG TINI_URI=https://github.com/krallin/tini/releases/download/v0.18.0/tini
# Thu, 16 Jul 2020 23:20:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.1.1-unix.tar.gz TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855 TINI_URI=https://github.com/krallin/tini/releases/download/v0.18.0/tini
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Jul 2020 23:20:40 GMT
COPY multi:1191f2c2f6370a31e5ebabb252b693639097aaeb5d54b38b45698e028dab3756 in /tmp/ 
# Thu, 16 Jul 2020 23:20:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.1.1-unix.tar.gz TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855 TINI_URI=https://github.com/krallin/tini/releases/download/v0.18.0/tini
RUN apt update     && apt install -y curl wget gosu jq     && curl -L --fail --silent --show-error ${TINI_URI} > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*     && apt-get -y purge --auto-remove curl
# Thu, 16 Jul 2020 23:20:52 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Jul 2020 23:20:52 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Jul 2020 23:20:52 GMT
VOLUME [/data /logs]
# Thu, 16 Jul 2020 23:20:53 GMT
COPY file:8b8c5515388aee21603a6091dadc2d3a6d4f7790a45cecce25e8ef5ed92f530d in /docker-entrypoint.sh 
# Thu, 16 Jul 2020 23:20:53 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Jul 2020 23:20:53 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Jul 2020 23:20:53 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:8559a31e96f442f2c7b6da49d6c84705f98a39d8be10b3f5f14821d0ee8417df`  
		Last Modified: Tue, 09 Jun 2020 01:25:50 GMT  
		Size: 27.1 MB (27098265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65306eca6b8ea03d29cd8d10a31e9d7a6a1cf8766fe4ca3913e75e00fc47be79`  
		Last Modified: Tue, 09 Jun 2020 16:41:33 GMT  
		Size: 3.2 MB (3248452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbf88050b6e7cbe8b76b77196134f31015ef5cb69123ba6af35da6f5b101459`  
		Last Modified: Tue, 09 Jun 2020 16:44:15 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fd11959573498746557a7424d83303d54d10ba094db44d40465936f4fe153c`  
		Last Modified: Thu, 16 Jul 2020 22:45:25 GMT  
		Size: 196.5 MB (196526149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87d8b218fb972aec7add0a2c44d5b6b0f3a8dfdd17bf8609f0e30f93e6fa390`  
		Last Modified: Thu, 16 Jul 2020 23:42:42 GMT  
		Size: 3.9 KB (3865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3932e0619243ba91de35f09294673bc8f941822f0ec25f110f13b6ab97ae840`  
		Last Modified: Thu, 16 Jul 2020 23:42:42 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32464573eb146d8df0f170d3cd33a7559724680115c9c49ec15bcebc705fa95`  
		Last Modified: Thu, 16 Jul 2020 23:42:50 GMT  
		Size: 121.5 MB (121549704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc88c1c6e23603449ad55a8ede561d89684c978ce253facf90424cdada7e8528`  
		Last Modified: Thu, 16 Jul 2020 23:42:42 GMT  
		Size: 5.9 KB (5857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
