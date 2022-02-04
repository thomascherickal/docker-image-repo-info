## `neo4j:community`

```console
$ docker pull neo4j@sha256:1752b1623e0285438ca3d9d72648f4df846f459f488418d6a96242603dafa022
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community` - linux; amd64

```console
$ docker pull neo4j@sha256:68f93f0679af1faedd208a8df8e83cabfe187960e9841c23edf792854ef48685
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **368.8 MB (368756849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:311c4c2d05bc42a48f88eaaa91c040ad7c5a7e21b85a468e70f83263d2b38a66`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 09:18:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:25:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:25:47 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:25:47 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:25:48 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:35:52 GMT
ENV JAVA_VERSION=11.0.14
# Thu, 03 Feb 2022 20:37:32 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jdk_x64_linux_11.0.14_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jdk_aarch64_linux_11.0.14_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 03 Feb 2022 20:37:33 GMT
CMD ["jshell"]
# Thu, 03 Feb 2022 22:37:10 GMT
ENV NEO4J_SHA256=87a01906c178977c082579def934afde0f806695e593fd119f237bff01cfa738 NEO4J_TARBALL=neo4j-community-4.4.3-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 03 Feb 2022 22:37:10 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.3-unix.tar.gz
# Thu, 03 Feb 2022 22:37:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.3-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 03 Feb 2022 22:37:12 GMT
COPY multi:220c2663e29181f5cd4d1cc8ff4ea55bca5bd66e60ecec0890d11b2c206bdb54 in /tmp/ 
# Thu, 03 Feb 2022 22:37:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.3-unix.tar.gz
RUN apt update     && apt install -y curl wget gosu jq     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && set -eux; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64')             tinisha="12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855";             tiniurl="https://github.com/krallin/tini/releases/download/v0.18.0/tini"; 			;; 		'arm64')             tinisha="7c5463f55393985ee22357d976758aaaecd08defb3c5294d353732018169b019";             tiniurl="https://github.com/krallin/tini/releases/download/v0.18.0/tini-arm64"; 			;; 		*) echo >&2 "Neo4j does not currently have a docker image for architecture $dpkgArch"; exit 1 ;; 	esac     && curl -L --fail --silent --show-error ${tiniurl} > /sbin/tini     && echo "${tinisha}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && apt-get -y purge --auto-remove curl     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Feb 2022 22:37:23 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Feb 2022 22:37:24 GMT
WORKDIR /var/lib/neo4j
# Thu, 03 Feb 2022 22:37:24 GMT
VOLUME [/data /logs]
# Thu, 03 Feb 2022 22:37:24 GMT
COPY file:ab7ae7f90c4a2b48d55ce46bb4b2dcdc336a04742bc26d5311b62b6d1e2ce171 in /docker-entrypoint.sh 
# Thu, 03 Feb 2022 22:37:24 GMT
EXPOSE 7473 7474 7687
# Thu, 03 Feb 2022 22:37:24 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 03 Feb 2022 22:37:25 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc79ff7de66b9ef44dc6cd4f500aa92bd1f0b09ccd13eb0ee6441084fbb719cf`  
		Last Modified: Wed, 26 Jan 2022 09:41:32 GMT  
		Size: 1.6 MB (1582049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd8e4b483dc66fafc6d3f664c2820fae67dcc216b91898060b80ff034a1c73b`  
		Last Modified: Wed, 26 Jan 2022 09:51:37 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd31164fce8d373ea92961c96503a2535f2f5dc31ccad385e60fc7c7e236139`  
		Last Modified: Thu, 03 Feb 2022 20:58:49 GMT  
		Size: 203.5 MB (203544081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7925e6a211afbd401f868c12bb04d07db2dc3b597998c06cd7aa7eb24da65ea`  
		Last Modified: Thu, 03 Feb 2022 23:21:29 GMT  
		Size: 3.9 KB (3863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c41fd0dcf4cf2a385293b217bebe5acba80607d3e8c6d8c13472db3bb17ca87`  
		Last Modified: Thu, 03 Feb 2022 23:21:29 GMT  
		Size: 603.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be605cd66682c15a2acb56ea155b5bab40dfee61a4c060822398cc67f50f9303`  
		Last Modified: Thu, 03 Feb 2022 23:21:37 GMT  
		Size: 132.3 MB (132253227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a05dbb25a8bcb390eae2223796e8da6032aeede311a7c07cf3510e421014f5`  
		Last Modified: Thu, 03 Feb 2022 23:21:29 GMT  
		Size: 6.6 KB (6556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:1d81ac33bf452b74e813b089372182a0a4f0dceb66e3c6b0c5f5796775f78aa3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.5 MB (364529106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eca50fb97212f9c399ad029aa38452e655e51983d42971216747edc87163e6ac`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:49:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:57:18 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:57:19 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:57:20 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:57:21 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:50:36 GMT
ENV JAVA_VERSION=11.0.14
# Thu, 03 Feb 2022 20:51:51 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jdk_x64_linux_11.0.14_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jdk_aarch64_linux_11.0.14_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 03 Feb 2022 20:51:52 GMT
CMD ["jshell"]
# Fri, 04 Feb 2022 00:22:39 GMT
ENV NEO4J_SHA256=87a01906c178977c082579def934afde0f806695e593fd119f237bff01cfa738 NEO4J_TARBALL=neo4j-community-4.4.3-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 04 Feb 2022 00:22:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.3-unix.tar.gz
# Fri, 04 Feb 2022 00:22:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.3-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 04 Feb 2022 00:22:43 GMT
COPY multi:220c2663e29181f5cd4d1cc8ff4ea55bca5bd66e60ecec0890d11b2c206bdb54 in /tmp/ 
# Fri, 04 Feb 2022 00:22:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.3-unix.tar.gz
RUN apt update     && apt install -y curl wget gosu jq     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && set -eux; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64')             tinisha="12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855";             tiniurl="https://github.com/krallin/tini/releases/download/v0.18.0/tini"; 			;; 		'arm64')             tinisha="7c5463f55393985ee22357d976758aaaecd08defb3c5294d353732018169b019";             tiniurl="https://github.com/krallin/tini/releases/download/v0.18.0/tini-arm64"; 			;; 		*) echo >&2 "Neo4j does not currently have a docker image for architecture $dpkgArch"; exit 1 ;; 	esac     && curl -L --fail --silent --show-error ${tiniurl} > /sbin/tini     && echo "${tinisha}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && apt-get -y purge --auto-remove curl     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Feb 2022 00:22:58 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Feb 2022 00:22:59 GMT
WORKDIR /var/lib/neo4j
# Fri, 04 Feb 2022 00:23:00 GMT
VOLUME [/data /logs]
# Fri, 04 Feb 2022 00:23:02 GMT
COPY file:ab7ae7f90c4a2b48d55ce46bb4b2dcdc336a04742bc26d5311b62b6d1e2ce171 in /docker-entrypoint.sh 
# Fri, 04 Feb 2022 00:23:02 GMT
EXPOSE 7473 7474 7687
# Fri, 04 Feb 2022 00:23:03 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Fri, 04 Feb 2022 00:23:04 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abf67e3e34eccefabf68f15c7d753f1a4c8e241beb1818f97e276186d54124e`  
		Last Modified: Wed, 26 Jan 2022 06:13:02 GMT  
		Size: 1.6 MB (1565889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f957b344357efffea3ef5d89bb0b35135ff9831c732632f178eb57736a7fcbd`  
		Last Modified: Wed, 26 Jan 2022 06:23:48 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f501c46d9c5747b396c12551593bf2e0dd8b59cb87b8f8fa6628c56df3dae26f`  
		Last Modified: Thu, 03 Feb 2022 21:13:22 GMT  
		Size: 200.9 MB (200944741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28a41df994e808280850ae9fec23df9e01aded6671c9c5ced2ae11b5d69d194`  
		Last Modified: Fri, 04 Feb 2022 00:27:22 GMT  
		Size: 3.8 KB (3841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496255ab9033e9aefc87e299035f55f7fb10766fc697c237cf87634e400fd019`  
		Last Modified: Fri, 04 Feb 2022 00:27:22 GMT  
		Size: 603.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369c2cba39e75bc016e029e6d1730ced4d5557a87025f219ec084054067f5b31`  
		Last Modified: Fri, 04 Feb 2022 00:27:31 GMT  
		Size: 132.0 MB (131950491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94274956042e312e0519d057d2433ced95aef668f462a3b90f635e32edec9fac`  
		Last Modified: Fri, 04 Feb 2022 00:27:22 GMT  
		Size: 6.6 KB (6555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
