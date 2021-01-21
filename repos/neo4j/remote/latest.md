## `neo4j:latest`

```console
$ docker pull neo4j@sha256:c7f24de1dc1d2020ab24a884b8a39538937c1b14bc0ca1da3ddb2573b6fc412f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:latest` - linux; amd64

```console
$ docker pull neo4j@sha256:f67e578fa0fa3f55cd18447b885689047dcf786097f8e7536912739dc489eae8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.4 MB (346413268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9edee9e153abe24856ff3586bc969f01a1e9c78d57e68a12ac3869753f4bdffc`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 10:53:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 10:53:01 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 10:58:17 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 12 Jan 2021 10:58:17 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 10:58:18 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 21 Jan 2021 02:38:27 GMT
ENV JAVA_VERSION=11.0.10
# Thu, 21 Jan 2021 02:38:53 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_aarch64_linux_11.0.10_9.tar.gz ;; 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_x64_linux_11.0.10_9.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 21 Jan 2021 02:38:53 GMT
CMD ["jshell"]
# Thu, 21 Jan 2021 05:54:59 GMT
ENV NEO4J_SHA256=6bbd385fea4b23f4447926209168499b361774f1cadae71ad4a960e648821359 NEO4J_TARBALL=neo4j-community-4.2.2-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 21 Jan 2021 05:54:59 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.2.2-unix.tar.gz
# Thu, 21 Jan 2021 05:54:59 GMT
ARG TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 21 Jan 2021 05:55:00 GMT
ARG TINI_URI=https://github.com/krallin/tini/releases/download/v0.18.0/tini
# Thu, 21 Jan 2021 05:55:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.2.2-unix.tar.gz TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855 TINI_URI=https://github.com/krallin/tini/releases/download/v0.18.0/tini
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 21 Jan 2021 05:55:01 GMT
COPY multi:1191f2c2f6370a31e5ebabb252b693639097aaeb5d54b38b45698e028dab3756 in /tmp/ 
# Thu, 21 Jan 2021 05:55:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.2.2-unix.tar.gz TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855 TINI_URI=https://github.com/krallin/tini/releases/download/v0.18.0/tini
RUN apt update     && apt install -y curl wget gosu jq     && curl -L --fail --silent --show-error ${TINI_URI} > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*     && apt-get -y purge --auto-remove curl
# Thu, 21 Jan 2021 05:55:14 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 21 Jan 2021 05:55:14 GMT
WORKDIR /var/lib/neo4j
# Thu, 21 Jan 2021 05:55:14 GMT
VOLUME [/data /logs]
# Thu, 21 Jan 2021 05:55:14 GMT
COPY file:9a89d97c25ee9015dde842a187432d2c15da00c93acc4fc894e399c78822272a in /docker-entrypoint.sh 
# Thu, 21 Jan 2021 05:55:14 GMT
EXPOSE 7473 7474 7687
# Thu, 21 Jan 2021 05:55:15 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:55:15 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943d8acaac04a2b66af03bcc85abe1cd3f50e06d7e193634e04d4e55c4fc7cc8`  
		Last Modified: Tue, 12 Jan 2021 11:07:22 GMT  
		Size: 3.2 MB (3248558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9998d19c11696925915d7583990a0b9e239265533655abc5376d117ec9cfe3c`  
		Last Modified: Tue, 12 Jan 2021 11:14:44 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba5b958e0416b8e5d7b2ae81a51f33cfba67f5d9ea139a5ffd099b8956dfdec`  
		Last Modified: Thu, 21 Jan 2021 02:48:35 GMT  
		Size: 197.2 MB (197200421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d0884b547fd320f335228338a7a4d05eddb73bf48c0eb80c2dee9fbd733b13`  
		Last Modified: Thu, 21 Jan 2021 06:30:40 GMT  
		Size: 3.9 KB (3864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3572cb50798269301b38627abfe3ae37dc07cde039c93f8053d325a894df6d`  
		Last Modified: Thu, 21 Jan 2021 06:30:37 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e743ea4f2800c12aff43ddae3bc6b11f50df481c93af664b0128b15d403abe63`  
		Last Modified: Thu, 21 Jan 2021 06:30:46 GMT  
		Size: 118.8 MB (118845711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020ba241c01171086d08f0aec09a88979cd43cc47f82ade1c805adb09afde0ec`  
		Last Modified: Thu, 21 Jan 2021 06:30:37 GMT  
		Size: 5.9 KB (5935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
