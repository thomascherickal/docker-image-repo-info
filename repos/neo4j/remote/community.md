## `neo4j:community`

```console
$ docker pull neo4j@sha256:0ed9dcc4408f8bbf6e6ababa38b9094cf5ae6ebf316d47d787a9123e61eb3959
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community` - linux; amd64

```console
$ docker pull neo4j@sha256:84517ae9b5c0638b01052ebaba5a3af96b31d586a8f13d22db5a25862abba492
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **368.6 MB (368604838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad8b04de872ae862d3a68ab47b6238b0b373aa58b36d7de891308402ad37a498`
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
# Wed, 26 Jan 2022 09:25:48 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 26 Jan 2022 09:26:34 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 26 Jan 2022 09:26:35 GMT
CMD ["jshell"]
# Thu, 27 Jan 2022 13:33:20 GMT
ENV NEO4J_SHA256=87a01906c178977c082579def934afde0f806695e593fd119f237bff01cfa738 NEO4J_TARBALL=neo4j-community-4.4.3-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 27 Jan 2022 13:33:20 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.3-unix.tar.gz
# Thu, 27 Jan 2022 13:33:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.3-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 27 Jan 2022 13:33:21 GMT
COPY multi:220c2663e29181f5cd4d1cc8ff4ea55bca5bd66e60ecec0890d11b2c206bdb54 in /tmp/ 
# Thu, 27 Jan 2022 13:33:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.3-unix.tar.gz
RUN apt update     && apt install -y curl wget gosu jq     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && set -eux; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64')             tinisha="12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855";             tiniurl="https://github.com/krallin/tini/releases/download/v0.18.0/tini"; 			;; 		'arm64')             tinisha="7c5463f55393985ee22357d976758aaaecd08defb3c5294d353732018169b019";             tiniurl="https://github.com/krallin/tini/releases/download/v0.18.0/tini-arm64"; 			;; 		*) echo >&2 "Neo4j does not currently have a docker image for architecture $dpkgArch"; exit 1 ;; 	esac     && curl -L --fail --silent --show-error ${tiniurl} > /sbin/tini     && echo "${tinisha}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && apt-get -y purge --auto-remove curl     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 13:33:33 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Jan 2022 13:33:34 GMT
WORKDIR /var/lib/neo4j
# Thu, 27 Jan 2022 13:33:34 GMT
VOLUME [/data /logs]
# Thu, 27 Jan 2022 13:33:34 GMT
COPY file:ab7ae7f90c4a2b48d55ce46bb4b2dcdc336a04742bc26d5311b62b6d1e2ce171 in /docker-entrypoint.sh 
# Thu, 27 Jan 2022 13:33:34 GMT
EXPOSE 7473 7474 7687
# Thu, 27 Jan 2022 13:33:34 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 27 Jan 2022 13:33:35 GMT
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
	-	`sha256:0be6defd841835caeb9df272ef43448ea9f39bdb700337ff7973ff1854f2a086`  
		Last Modified: Wed, 26 Jan 2022 09:51:56 GMT  
		Size: 203.4 MB (203392014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159948bf00b450b5c56774865c01d451903fe5f843f5594d8fadf7bbfa02e198`  
		Last Modified: Thu, 27 Jan 2022 14:22:36 GMT  
		Size: 3.9 KB (3872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd6dcd0f3d638b3b9ba4aaaac3428ab5495d1e91d6f53044ef53cb04a116608`  
		Last Modified: Thu, 27 Jan 2022 14:22:36 GMT  
		Size: 604.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90cae1b1a19f4e21862b8b4ed02021e3a4cd93521ba580b1c57f35930a25e732`  
		Last Modified: Thu, 27 Jan 2022 14:22:43 GMT  
		Size: 132.3 MB (132253273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f3b3c82848239386d079f892cdd41aa50f419dbffd2c0963d5b95a4dc69d7f`  
		Last Modified: Thu, 27 Jan 2022 14:22:36 GMT  
		Size: 6.6 KB (6556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:45dc924719595bc627da8f9fe3a6fe2b1885a0dbfb218802130a7300c919cf43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.4 MB (364353139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a3b26611fd4cd039823c018a730161a2f0deba3a3ae0c1c2fd76fac7b53d2e3`
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
# Wed, 26 Jan 2022 05:57:22 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 26 Jan 2022 05:57:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 26 Jan 2022 05:57:45 GMT
CMD ["jshell"]
# Thu, 27 Jan 2022 01:24:11 GMT
ENV NEO4J_SHA256=87a01906c178977c082579def934afde0f806695e593fd119f237bff01cfa738 NEO4J_TARBALL=neo4j-community-4.4.3-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 27 Jan 2022 01:24:11 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.3-unix.tar.gz
# Thu, 27 Jan 2022 01:24:12 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.3-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 27 Jan 2022 01:24:14 GMT
COPY multi:220c2663e29181f5cd4d1cc8ff4ea55bca5bd66e60ecec0890d11b2c206bdb54 in /tmp/ 
# Thu, 27 Jan 2022 01:24:28 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.3-unix.tar.gz
RUN apt update     && apt install -y curl wget gosu jq     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && set -eux; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64')             tinisha="12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855";             tiniurl="https://github.com/krallin/tini/releases/download/v0.18.0/tini"; 			;; 		'arm64')             tinisha="7c5463f55393985ee22357d976758aaaecd08defb3c5294d353732018169b019";             tiniurl="https://github.com/krallin/tini/releases/download/v0.18.0/tini-arm64"; 			;; 		*) echo >&2 "Neo4j does not currently have a docker image for architecture $dpkgArch"; exit 1 ;; 	esac     && curl -L --fail --silent --show-error ${tiniurl} > /sbin/tini     && echo "${tinisha}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && apt-get -y purge --auto-remove curl     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 01:24:28 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Jan 2022 01:24:29 GMT
WORKDIR /var/lib/neo4j
# Thu, 27 Jan 2022 01:24:30 GMT
VOLUME [/data /logs]
# Thu, 27 Jan 2022 01:24:32 GMT
COPY file:ab7ae7f90c4a2b48d55ce46bb4b2dcdc336a04742bc26d5311b62b6d1e2ce171 in /docker-entrypoint.sh 
# Thu, 27 Jan 2022 01:24:32 GMT
EXPOSE 7473 7474 7687
# Thu, 27 Jan 2022 01:24:33 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 27 Jan 2022 01:24:34 GMT
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
	-	`sha256:23e3996cb8b1e856fc6fbb99423d5fdb73fe4f0347aa79f3db624731191db7d1`  
		Last Modified: Wed, 26 Jan 2022 06:24:08 GMT  
		Size: 200.8 MB (200768792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb458f2b0ac72457232566a9330431bc93b96f83eed3751eeb9c1c333bb1205`  
		Last Modified: Thu, 27 Jan 2022 01:29:15 GMT  
		Size: 3.8 KB (3845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d809b84f74d411a3a1125b918cf39ae3fa438324ec0b05b57c4527e70ec7f2a4`  
		Last Modified: Thu, 27 Jan 2022 01:29:15 GMT  
		Size: 603.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7c0c1a5adae6acff2c5585e52e29459309d5a9c12739e62e2e8f8d4587559b`  
		Last Modified: Thu, 27 Jan 2022 01:29:24 GMT  
		Size: 132.0 MB (131950469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e224579252e5fd94a125a1a73ad1fd5f11556d5e788b2dc6872f251645ea6e9`  
		Last Modified: Thu, 27 Jan 2022 01:29:15 GMT  
		Size: 6.6 KB (6555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
