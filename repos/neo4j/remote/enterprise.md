## `neo4j:enterprise`

```console
$ docker pull neo4j@sha256:9638bb65356d3118260a85243e614a274475a1a2b37015eacd4b338eaff02c1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:8447603a7b6110616f141ee21935a92ec91271fb6a936619aa540e81443c8c25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.4 MB (384393308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e569a37ff0134a5c1647e1d15bc5bdf34fc70e50a2a2c5f4ada241f037f2203`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 22:10:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:14:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Fri, 12 Mar 2021 22:14:10 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 12 Mar 2021 22:14:10 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 22:14:10 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 22:14:10 GMT
ENV JAVA_VERSION=11.0.10
# Fri, 12 Mar 2021 22:14:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_x64_linux_11.0.10_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_aarch64_linux_11.0.10_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 12 Mar 2021 22:14:30 GMT
CMD ["jshell"]
# Fri, 19 Mar 2021 19:17:30 GMT
ENV NEO4J_SHA256=27a6f5a5d3a2196c8f450a7a985d7ca7ec737c48ddb228fb3ec10e50ef546f40 NEO4J_TARBALL=neo4j-enterprise-4.2.4-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 19 Mar 2021 19:17:30 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.2.4-unix.tar.gz
# Fri, 19 Mar 2021 19:17:30 GMT
ARG TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Fri, 19 Mar 2021 19:17:30 GMT
ARG TINI_URI=https://github.com/krallin/tini/releases/download/v0.18.0/tini
# Fri, 19 Mar 2021 19:17:32 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.2.4-unix.tar.gz TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855 TINI_URI=https://github.com/krallin/tini/releases/download/v0.18.0/tini
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 19 Mar 2021 19:17:32 GMT
COPY multi:036df619eeee70a762e1c411f9386c81834e8c049e5b509d291c299dd3c27252 in /tmp/ 
# Fri, 19 Mar 2021 19:17:49 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.2.4-unix.tar.gz TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855 TINI_URI=https://github.com/krallin/tini/releases/download/v0.18.0/tini
RUN apt update     && apt install -y curl wget gosu jq     && curl -L --fail --silent --show-error ${TINI_URI} > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*     && apt-get -y purge --auto-remove curl
# Fri, 19 Mar 2021 19:17:50 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 19 Mar 2021 19:17:50 GMT
WORKDIR /var/lib/neo4j
# Fri, 19 Mar 2021 19:17:50 GMT
VOLUME [/data /logs]
# Fri, 19 Mar 2021 19:17:50 GMT
COPY file:1f612e4a1e8c1ac46ddb26d08eacd2e329f1f6f81fea1862bc5fcd3a8d302a54 in /docker-entrypoint.sh 
# Fri, 19 Mar 2021 19:17:50 GMT
EXPOSE 7473 7474 7687
# Fri, 19 Mar 2021 19:17:51 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Fri, 19 Mar 2021 19:17:51 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3555c3885852c38ecf4a297b798053677bc7553f9c7631788ef75e35cb4262c`  
		Last Modified: Fri, 12 Mar 2021 22:22:18 GMT  
		Size: 3.3 MB (3268564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42965fccf40100a915fa0b4b20946987c4e330948b82f687f22d7b6575473af0`  
		Last Modified: Fri, 12 Mar 2021 22:27:57 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a08f33239498a8db24a0c238534d24b52e37444323df2afb8a25076d905f5a`  
		Last Modified: Fri, 12 Mar 2021 22:28:15 GMT  
		Size: 203.1 MB (203079182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9bf32ede506ce8398dad6e0f1739778cd3e0adadc66bd647ca844e585601af`  
		Last Modified: Fri, 19 Mar 2021 19:24:34 GMT  
		Size: 3.9 KB (3869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921b614f96febf1fb6e443ce404e9e37010259b7ec2d20d11453be3311bf829c`  
		Last Modified: Fri, 19 Mar 2021 19:24:34 GMT  
		Size: 573.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36799f2ce888633a74e8affe715636aeb797c589b7ddae5cab1889c59146637b`  
		Last Modified: Fri, 19 Mar 2021 19:24:42 GMT  
		Size: 150.9 MB (150933952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfadff307ee37709e20928894a019bd5ed2fcf08b7c190faafa88b09e0e1605`  
		Last Modified: Fri, 19 Mar 2021 19:24:34 GMT  
		Size: 6.0 KB (5955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
