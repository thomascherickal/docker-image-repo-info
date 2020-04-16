<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `neo4j`

-	[`neo4j:3.4`](#neo4j34)
-	[`neo4j:3.4.14`](#neo4j3414)
-	[`neo4j:3.4.14-enterprise`](#neo4j3414-enterprise)
-	[`neo4j:3.4.15`](#neo4j3415)
-	[`neo4j:3.4.15-enterprise`](#neo4j3415-enterprise)
-	[`neo4j:3.4.16`](#neo4j3416)
-	[`neo4j:3.4.16-enterprise`](#neo4j3416-enterprise)
-	[`neo4j:3.4.17`](#neo4j3417)
-	[`neo4j:3.4.17-enterprise`](#neo4j3417-enterprise)
-	[`neo4j:3.4-enterprise`](#neo4j34-enterprise)
-	[`neo4j:3.5`](#neo4j35)
-	[`neo4j:3.5.11`](#neo4j3511)
-	[`neo4j:3.5.11-enterprise`](#neo4j3511-enterprise)
-	[`neo4j:3.5.12`](#neo4j3512)
-	[`neo4j:3.5.12-enterprise`](#neo4j3512-enterprise)
-	[`neo4j:3.5.13`](#neo4j3513)
-	[`neo4j:3.5.13-enterprise`](#neo4j3513-enterprise)
-	[`neo4j:3.5.14`](#neo4j3514)
-	[`neo4j:3.5.14-enterprise`](#neo4j3514-enterprise)
-	[`neo4j:3.5.15`](#neo4j3515)
-	[`neo4j:3.5.15-enterprise`](#neo4j3515-enterprise)
-	[`neo4j:3.5.16`](#neo4j3516)
-	[`neo4j:3.5.16-enterprise`](#neo4j3516-enterprise)
-	[`neo4j:3.5.17`](#neo4j3517)
-	[`neo4j:3.5.17-enterprise`](#neo4j3517-enterprise)
-	[`neo4j:3.5.6`](#neo4j356)
-	[`neo4j:3.5.6-enterprise`](#neo4j356-enterprise)
-	[`neo4j:3.5.7`](#neo4j357)
-	[`neo4j:3.5.7-enterprise`](#neo4j357-enterprise)
-	[`neo4j:3.5.8`](#neo4j358)
-	[`neo4j:3.5.8-enterprise`](#neo4j358-enterprise)
-	[`neo4j:3.5-enterprise`](#neo4j35-enterprise)
-	[`neo4j:4.0`](#neo4j40)
-	[`neo4j:4.0.0`](#neo4j400)
-	[`neo4j:4.0.0-enterprise`](#neo4j400-enterprise)
-	[`neo4j:4.0.1`](#neo4j401)
-	[`neo4j:4.0.1-enterprise`](#neo4j401-enterprise)
-	[`neo4j:4.0.2`](#neo4j402)
-	[`neo4j:4.0.2-enterprise`](#neo4j402-enterprise)
-	[`neo4j:4.0.3`](#neo4j403)
-	[`neo4j:4.0.3-enterprise`](#neo4j403-enterprise)
-	[`neo4j:4.0-enterprise`](#neo4j40-enterprise)
-	[`neo4j:enterprise`](#neo4jenterprise)
-	[`neo4j:latest`](#neo4jlatest)

## `neo4j:3.4`

```console
$ docker pull neo4j@sha256:f1026480c56b36bd5ebd615ff3112f71e2db312f7576a7237c7a6cd790d5f170
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.4` - linux; amd64

```console
$ docker pull neo4j@sha256:dd81be4704afbb9f6b7dc630dd87f50866a96830a9cfbf677da712f80bf6c95d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.0 MB (215023097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3495c9654754890f192a45705b28a1f7b68ea78ba48ae2c080ede47a4ad8bf16`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:13:10 GMT
ENV NEO4J_SHA256=fbb03e85a09e1e8a77c496ad61e8094ef94185268098634a4aaf1d1a01b841a6 NEO4J_TARBALL=neo4j-community-3.4.17-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:13:10 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.4.17-unix.tar.gz
# Thu, 16 Apr 2020 02:13:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.4.17-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:13:11 GMT
COPY multi:70b59ed932367b04ea9c69354feb959e63e40f0dd9086b2097eaeba453964337 in /tmp/ 
# Thu, 16 Apr 2020 02:13:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.4.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:13:25 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:13:25 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:13:25 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:13:25 GMT
COPY file:d76df40f02e9ebf317a807eaee3b8b30c3997b4bca927f8a336e347e3901f7b6 in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:13:26 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:13:26 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:13:26 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a2c4d18f0faf1a2df629c1cf527ec40040e7c91eae9394efaa617203fcd6da`  
		Last Modified: Thu, 16 Apr 2020 02:29:12 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d751d0ddc50da8548e44779c9dd7b3d339e7d2f40b938e63d7cdc938ee650b0`  
		Last Modified: Thu, 16 Apr 2020 02:29:12 GMT  
		Size: 302.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db18e23c9951df504610beafa95f064959e1fa405d408f200f67e72c9a7af997`  
		Last Modified: Thu, 16 Apr 2020 02:29:25 GMT  
		Size: 144.1 MB (144082170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41531daba68636097aeea65628c00cde4f355a5822451162bfec8e032a19c5d6`  
		Last Modified: Thu, 16 Apr 2020 02:29:12 GMT  
		Size: 5.3 KB (5302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.4.14`

```console
$ docker pull neo4j@sha256:68a377425240331b4062e2f7077138d861b3795a85134a8c3993604e530938a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.4.14` - linux; amd64

```console
$ docker pull neo4j@sha256:256572284634778d40d18e2e508e871506cc66cc2bcf484651b4f4a1dc53a193
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.5 MB (225548134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821f3ee60a5650c14dd9fe6f4a3745ba28133d6fd6426c950c371b67830d7b51`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:15:24 GMT
ENV NEO4J_SHA256=fcbdd7abc28a50cca76daed96d60a6d7d03a4db5bbbfdfb8e520ee1984698461 NEO4J_TARBALL=neo4j-community-3.4.14-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:15:24 GMT
ARG NEO4J_URI=http://dist.neo4j.org/neo4j-community-3.4.14-unix.tar.gz
# Thu, 16 Apr 2020 02:15:25 GMT
# ARGS: NEO4J_URI=http://dist.neo4j.org/neo4j-community-3.4.14-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:15:25 GMT
COPY file:696befc481f5ad55a590fa577c3d4ba04c9237326d85b95b729538f95702e110 in /tmp/ 
# Thu, 16 Apr 2020 02:15:38 GMT
# ARGS: NEO4J_URI=http://dist.neo4j.org/neo4j-community-3.4.14-unix.tar.gz
RUN apt update     && apt install -y curl gosu     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs
# Thu, 16 Apr 2020 02:15:38 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:15:39 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:15:39 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:15:39 GMT
COPY file:a6df7d0365e68d6518a68c4e06867141cbce4a327fb803991d77cb4c971aed5d in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:15:39 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:15:40 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:15:40 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f909d7c142a466c4b797f1d46eaaa074f776e79112f29f088cc30f2c7e1e7c`  
		Last Modified: Thu, 16 Apr 2020 02:31:05 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee92b3744790eba9f789afeba4488918cc9704bbb94ba842dca6ac760a86a5e`  
		Last Modified: Thu, 16 Apr 2020 02:31:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8fa122291af9fd9c6f815c261a840f86e9a625513d7c111555a5abc7d61e85`  
		Last Modified: Thu, 16 Apr 2020 02:31:30 GMT  
		Size: 154.6 MB (154608295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996c74ff0ddb7610f734f6c35f4a06cfa91474047e9baba2c02098fb605a5a16`  
		Last Modified: Thu, 16 Apr 2020 02:31:05 GMT  
		Size: 4.4 KB (4387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.4.14-enterprise`

```console
$ docker pull neo4j@sha256:d90d2f2c84c147f5724f0ca5378775c075c9c933e641a3c84426fdeffc1c368b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.4.14-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:404189f9dfef394b6c66dfe021d4c5debaa1e3821b3b02cf5bd50576c1ed2831
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.3 MB (242328287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11059a0dc34c35da12e94b7b28d577599190591171f1e2cb917b4556bb681fb3`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:15:45 GMT
ENV NEO4J_SHA256=5ebd47769a7aa25343d0b1ea59c2e9f2c847c56ac344ce2644d1f60496a7386f NEO4J_TARBALL=neo4j-enterprise-3.4.14-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:15:46 GMT
ARG NEO4J_URI=http://dist.neo4j.org/neo4j-enterprise-3.4.14-unix.tar.gz
# Thu, 16 Apr 2020 02:15:47 GMT
# ARGS: NEO4J_URI=http://dist.neo4j.org/neo4j-enterprise-3.4.14-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:15:47 GMT
COPY file:696befc481f5ad55a590fa577c3d4ba04c9237326d85b95b729538f95702e110 in /tmp/ 
# Thu, 16 Apr 2020 02:15:59 GMT
# ARGS: NEO4J_URI=http://dist.neo4j.org/neo4j-enterprise-3.4.14-unix.tar.gz
RUN apt update     && apt install -y curl gosu     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs
# Thu, 16 Apr 2020 02:16:00 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:16:00 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:16:00 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:16:00 GMT
COPY file:a6df7d0365e68d6518a68c4e06867141cbce4a327fb803991d77cb4c971aed5d in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:16:00 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:16:01 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:16:01 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3808e5fc9b2cea4e67acf3356152f77b8f3018ec361bdfb406bb3019ce295823`  
		Last Modified: Thu, 16 Apr 2020 02:31:34 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cdb85b956363d9115c5c3a8902817f6bf9af67d1fec6c7279ce032310c71161`  
		Last Modified: Thu, 16 Apr 2020 02:31:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed61188dd8b5c1fee70ecf5e7a5dda9b6b940d44d159a62133f7b5f12aada1f5`  
		Last Modified: Thu, 16 Apr 2020 02:31:50 GMT  
		Size: 171.4 MB (171388447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03c89cd1472524cc8b2029f857f15c8129c41e00ce55a116e44b28a8f9bfae8`  
		Last Modified: Thu, 16 Apr 2020 02:31:34 GMT  
		Size: 4.4 KB (4387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.4.15`

```console
$ docker pull neo4j@sha256:51242e4f8146383e442d9f3f680f12faf4bb8fe1568a1be27398426ead574fe6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.4.15` - linux; amd64

```console
$ docker pull neo4j@sha256:9909276672bbbb7043dd12cafad23dfb87e877d1e775e9c9ef23314be0bc9abb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.2 MB (212158613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8337a900634bb4b7add4bcb5dc5555fedcb4b8424987f6f9eb24f9680d31957f`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:14:43 GMT
ENV NEO4J_SHA256=7e230753e2c53c912829f1ed2df963fbacc3892acd3501a84892118317fbccda NEO4J_TARBALL=neo4j-community-3.4.15-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:14:44 GMT
ARG NEO4J_URI=http://dist.neo4j.org/neo4j-community-3.4.15-unix.tar.gz
# Thu, 16 Apr 2020 02:14:45 GMT
# ARGS: NEO4J_URI=http://dist.neo4j.org/neo4j-community-3.4.15-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:14:45 GMT
COPY file:696befc481f5ad55a590fa577c3d4ba04c9237326d85b95b729538f95702e110 in /tmp/ 
# Thu, 16 Apr 2020 02:14:57 GMT
# ARGS: NEO4J_URI=http://dist.neo4j.org/neo4j-community-3.4.15-unix.tar.gz
RUN apt update     && apt install -y curl gosu     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:14:57 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:14:57 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:14:58 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:14:58 GMT
COPY file:e07128b8290e38440521f56bbf78b61bbce8be21a97b8b31668594bebdd2bf2b in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:14:58 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:14:58 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:14:58 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda9d7c3a29497f2a4780c8e81221d18a8dec7f4f7cdb709e823ff83916a061a`  
		Last Modified: Thu, 16 Apr 2020 02:30:31 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61edf3e709a397edc51ecaaad89d8d4ac1f1aa9b767ed7c5ab469b399ee3fd8a`  
		Last Modified: Thu, 16 Apr 2020 02:30:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1a16c52e0102f719db73626c4bb95e50888245a3d0ca3f5c04c2e6b60cd593`  
		Last Modified: Thu, 16 Apr 2020 02:30:42 GMT  
		Size: 141.2 MB (141218813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba8cd6428d3576ee4326f4a66e2a9b8820b5e45b7c83a98c3bd65232fad3a48`  
		Last Modified: Thu, 16 Apr 2020 02:30:31 GMT  
		Size: 4.3 KB (4348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.4.15-enterprise`

```console
$ docker pull neo4j@sha256:85dbca8d821f50c19b0a4609d1326cbeae9c15edc2d960bb771aa4b0226118ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.4.15-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:f4f0127038e192a5b535639991831e8d1a572540a667434a804402750846f5a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.9 MB (228941193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb6224a423ba4035f5aa1c3da564352cc73eb138e08e509a6fcc4415a49a2bca`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:15:02 GMT
ENV NEO4J_SHA256=d7d215dcdbb9e5d6bb426003d62a1be2ffe3cb20039bb3432be8f9eab9be9e56 NEO4J_TARBALL=neo4j-enterprise-3.4.15-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:15:03 GMT
ARG NEO4J_URI=http://dist.neo4j.org/neo4j-enterprise-3.4.15-unix.tar.gz
# Thu, 16 Apr 2020 02:15:04 GMT
# ARGS: NEO4J_URI=http://dist.neo4j.org/neo4j-enterprise-3.4.15-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:15:04 GMT
COPY file:696befc481f5ad55a590fa577c3d4ba04c9237326d85b95b729538f95702e110 in /tmp/ 
# Thu, 16 Apr 2020 02:15:16 GMT
# ARGS: NEO4J_URI=http://dist.neo4j.org/neo4j-enterprise-3.4.15-unix.tar.gz
RUN apt update     && apt install -y curl gosu     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:15:16 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:15:17 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:15:17 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:15:17 GMT
COPY file:e07128b8290e38440521f56bbf78b61bbce8be21a97b8b31668594bebdd2bf2b in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:15:17 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:15:18 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:15:18 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83bf79aa249e3e4a9f657b31854b59584771ae0c037ec345d1f9538e2274710b`  
		Last Modified: Thu, 16 Apr 2020 02:30:47 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2602a05175b94e6bb3b2ad3399852d3c13e3998aa3dd8f3c242c044fb5ff88ae`  
		Last Modified: Thu, 16 Apr 2020 02:30:47 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77649ed4220fc10b9e433a9efbe5864d9196c4296b032f7d53a08d9d7ad33405`  
		Last Modified: Thu, 16 Apr 2020 02:31:01 GMT  
		Size: 158.0 MB (158001392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16849bb92e095653147f827c82a08680477ee6708eaf6d494767198907a83f9c`  
		Last Modified: Thu, 16 Apr 2020 02:30:47 GMT  
		Size: 4.3 KB (4348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.4.16`

```console
$ docker pull neo4j@sha256:f9735a3ffae45ce96a4d92ace454279791762de7796a6859deb463535db1148c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.4.16` - linux; amd64

```console
$ docker pull neo4j@sha256:a505f82d3054b8002c7b588f649cebe410622298ec8af5bc8ee440dab008c4f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.6 MB (212621464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6478906ce72f09a037926ff257ebc19d0691f5adbbdf9808387a9840817861c7`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:14:00 GMT
ENV NEO4J_SHA256=8c42ebe3455d92deedb09417dc02bcd37f5e0f13eb3f3faa5f1a5b9d4a781c7b NEO4J_TARBALL=neo4j-community-3.4.16-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:14:00 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.4.16-unix.tar.gz
# Thu, 16 Apr 2020 02:14:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.4.16-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:14:02 GMT
COPY multi:70b59ed932367b04ea9c69354feb959e63e40f0dd9086b2097eaeba453964337 in /tmp/ 
# Thu, 16 Apr 2020 02:14:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.4.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:14:15 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:14:15 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:14:15 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:14:15 GMT
COPY file:d76df40f02e9ebf317a807eaee3b8b30c3997b4bca927f8a336e347e3901f7b6 in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:14:15 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:14:16 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:14:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a018dc81e61c552fd43f13d432b4a9902ce3488a21f57abbb590cc2e2f036cf0`  
		Last Modified: Thu, 16 Apr 2020 02:29:50 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8624637e0b984de8fc4adab62f7cb01b0120682726d939906356179c100b0e`  
		Last Modified: Thu, 16 Apr 2020 02:29:50 GMT  
		Size: 302.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7793f201dffe5cf02debeb0418306574b24655b2a7c25d5bb75459152dc36f7`  
		Last Modified: Thu, 16 Apr 2020 02:30:02 GMT  
		Size: 141.7 MB (141680536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbf4bcfe553040bcc6f4808f78a65cd0c8479c6750ff0c6dd7f35efed972811`  
		Last Modified: Thu, 16 Apr 2020 02:29:50 GMT  
		Size: 5.3 KB (5302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.4.16-enterprise`

```console
$ docker pull neo4j@sha256:c4a1b6e0732b3347e6ccd114d1fbc64f323477ec0c4a6149e843189afede181a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.4.16-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:b1278dfa544a347895c32ab8c928b292fa24c4f3a840202d6bc0bc66f93a59c4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.4 MB (229403210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:136ae3c58e77312ae626d934a18aedc9410e68fee55628f443a0638ef6507088`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:14:22 GMT
ENV NEO4J_SHA256=ba8cf11ba8eb689755fcb7aacedf74391c6b5ec9ff423e921948ace401db12b9 NEO4J_TARBALL=neo4j-enterprise-3.4.16-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:14:22 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.4.16-unix.tar.gz
# Thu, 16 Apr 2020 02:14:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.4.16-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:14:23 GMT
COPY multi:70b59ed932367b04ea9c69354feb959e63e40f0dd9086b2097eaeba453964337 in /tmp/ 
# Thu, 16 Apr 2020 02:14:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.4.16-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:14:38 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:14:38 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:14:38 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:14:39 GMT
COPY file:d76df40f02e9ebf317a807eaee3b8b30c3997b4bca927f8a336e347e3901f7b6 in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:14:39 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:14:39 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:14:39 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b992104d1fe89fe44277f2db3191e5c87835603321f05870170ae486e9424adc`  
		Last Modified: Thu, 16 Apr 2020 02:30:07 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3115bf4a872516db9bd588b5ee6477e24c76cf6a89d663dc26563f5ef7c005d3`  
		Last Modified: Thu, 16 Apr 2020 02:30:07 GMT  
		Size: 302.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c6c7bbc753a9a45531c79c6a980177f04bb01537e386f8b2fb8ad8d64f651`  
		Last Modified: Thu, 16 Apr 2020 02:30:23 GMT  
		Size: 158.5 MB (158462283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1810215795109f96e31b8e999025c41708682cba48bfc6bea8b3d2c3c126db3e`  
		Last Modified: Thu, 16 Apr 2020 02:30:06 GMT  
		Size: 5.3 KB (5302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.4.17`

```console
$ docker pull neo4j@sha256:f1026480c56b36bd5ebd615ff3112f71e2db312f7576a7237c7a6cd790d5f170
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.4.17` - linux; amd64

```console
$ docker pull neo4j@sha256:dd81be4704afbb9f6b7dc630dd87f50866a96830a9cfbf677da712f80bf6c95d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.0 MB (215023097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3495c9654754890f192a45705b28a1f7b68ea78ba48ae2c080ede47a4ad8bf16`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:13:10 GMT
ENV NEO4J_SHA256=fbb03e85a09e1e8a77c496ad61e8094ef94185268098634a4aaf1d1a01b841a6 NEO4J_TARBALL=neo4j-community-3.4.17-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:13:10 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.4.17-unix.tar.gz
# Thu, 16 Apr 2020 02:13:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.4.17-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:13:11 GMT
COPY multi:70b59ed932367b04ea9c69354feb959e63e40f0dd9086b2097eaeba453964337 in /tmp/ 
# Thu, 16 Apr 2020 02:13:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.4.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:13:25 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:13:25 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:13:25 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:13:25 GMT
COPY file:d76df40f02e9ebf317a807eaee3b8b30c3997b4bca927f8a336e347e3901f7b6 in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:13:26 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:13:26 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:13:26 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a2c4d18f0faf1a2df629c1cf527ec40040e7c91eae9394efaa617203fcd6da`  
		Last Modified: Thu, 16 Apr 2020 02:29:12 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d751d0ddc50da8548e44779c9dd7b3d339e7d2f40b938e63d7cdc938ee650b0`  
		Last Modified: Thu, 16 Apr 2020 02:29:12 GMT  
		Size: 302.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db18e23c9951df504610beafa95f064959e1fa405d408f200f67e72c9a7af997`  
		Last Modified: Thu, 16 Apr 2020 02:29:25 GMT  
		Size: 144.1 MB (144082170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41531daba68636097aeea65628c00cde4f355a5822451162bfec8e032a19c5d6`  
		Last Modified: Thu, 16 Apr 2020 02:29:12 GMT  
		Size: 5.3 KB (5302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.4.17-enterprise`

```console
$ docker pull neo4j@sha256:243fbdf3ccddc5bc3732429824928d0a019d5f66ed63553905566b0d42c47933
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.4.17-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:cf0242d6da87bb366714ec05532c9d6ee740078762be58184e0b951648202b1b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.8 MB (231806357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9064416d1cc046f89eb3d8d2d03983dfb680bf94fef3135bf00659517d872b0`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:13:31 GMT
ENV NEO4J_SHA256=7d8d689ddc605c66296fadedb0d6810b8159513cb596b68b730f2604ce8bb9df NEO4J_TARBALL=neo4j-enterprise-3.4.17-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:13:31 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.4.17-unix.tar.gz
# Thu, 16 Apr 2020 02:13:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.4.17-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:13:33 GMT
COPY multi:70b59ed932367b04ea9c69354feb959e63e40f0dd9086b2097eaeba453964337 in /tmp/ 
# Thu, 16 Apr 2020 02:13:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.4.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:13:52 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:13:53 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:13:53 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:13:53 GMT
COPY file:d76df40f02e9ebf317a807eaee3b8b30c3997b4bca927f8a336e347e3901f7b6 in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:13:53 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:13:54 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:13:54 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa3b184313110283972d9655ac938f0e646180baaad41050c42ac14b77d255d`  
		Last Modified: Thu, 16 Apr 2020 02:29:31 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6252628a121542de054ad438605b7ac1fc0923963d4a70c948dc8e811d8be28`  
		Last Modified: Thu, 16 Apr 2020 02:29:31 GMT  
		Size: 302.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547927c328838dc546e825dd58470a85aad7f3e15f1ef8e96d2689d2bcfbfabe`  
		Last Modified: Thu, 16 Apr 2020 02:29:45 GMT  
		Size: 160.9 MB (160865431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57fc7c40a466ed27f4b506bb1bb216b3d4b2fb94ea8210caf1aafbfaecd8c22b`  
		Last Modified: Thu, 16 Apr 2020 02:29:30 GMT  
		Size: 5.3 KB (5302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.4-enterprise`

```console
$ docker pull neo4j@sha256:243fbdf3ccddc5bc3732429824928d0a019d5f66ed63553905566b0d42c47933
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.4-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:cf0242d6da87bb366714ec05532c9d6ee740078762be58184e0b951648202b1b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.8 MB (231806357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9064416d1cc046f89eb3d8d2d03983dfb680bf94fef3135bf00659517d872b0`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:13:31 GMT
ENV NEO4J_SHA256=7d8d689ddc605c66296fadedb0d6810b8159513cb596b68b730f2604ce8bb9df NEO4J_TARBALL=neo4j-enterprise-3.4.17-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:13:31 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.4.17-unix.tar.gz
# Thu, 16 Apr 2020 02:13:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.4.17-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:13:33 GMT
COPY multi:70b59ed932367b04ea9c69354feb959e63e40f0dd9086b2097eaeba453964337 in /tmp/ 
# Thu, 16 Apr 2020 02:13:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.4.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:13:52 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:13:53 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:13:53 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:13:53 GMT
COPY file:d76df40f02e9ebf317a807eaee3b8b30c3997b4bca927f8a336e347e3901f7b6 in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:13:53 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:13:54 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:13:54 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa3b184313110283972d9655ac938f0e646180baaad41050c42ac14b77d255d`  
		Last Modified: Thu, 16 Apr 2020 02:29:31 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6252628a121542de054ad438605b7ac1fc0923963d4a70c948dc8e811d8be28`  
		Last Modified: Thu, 16 Apr 2020 02:29:31 GMT  
		Size: 302.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547927c328838dc546e825dd58470a85aad7f3e15f1ef8e96d2689d2bcfbfabe`  
		Last Modified: Thu, 16 Apr 2020 02:29:45 GMT  
		Size: 160.9 MB (160865431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57fc7c40a466ed27f4b506bb1bb216b3d4b2fb94ea8210caf1aafbfaecd8c22b`  
		Last Modified: Thu, 16 Apr 2020 02:29:30 GMT  
		Size: 5.3 KB (5302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.5`

```console
$ docker pull neo4j@sha256:a6ed5769bacc77022de6c2d52865717d89ffbe98e08ef4ca0f8af892de61d3f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.5` - linux; amd64

```console
$ docker pull neo4j@sha256:41cb0222e4768eb455711c88c36a25f346a50abe5fdf1e133cc26089532d2246
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.8 MB (206781212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ded1bd0b452b76c4be8ef887ec8fb1f9f011f9e1cc749c59fbf95053379865b`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:03:43 GMT
ENV NEO4J_SHA256=1c8b6ac0ffd346f0707fe1af713ef74f1c6ce1ea6feb5e9a0bd170e7a8a34a10 NEO4J_TARBALL=neo4j-community-3.5.17-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:03:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.17-unix.tar.gz
# Thu, 16 Apr 2020 02:03:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.17-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:03:44 GMT
COPY multi:5d2171ebdeb5752d080b96f9ac9e7cf87aeb5949ca626a75789d79e846b648b2 in /tmp/ 
# Thu, 16 Apr 2020 02:04:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.17-unix.tar.gz
RUN apt update      && apt install -y curl wget gosu jq      && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini      && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet      && chmod +x /sbin/tini      && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}      && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet      && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib      && mv /var/lib/neo4j-* "${NEO4J_HOME}"      && rm ${NEO4J_TARBALL}      && mv "${NEO4J_HOME}"/data /data      && mv "${NEO4J_HOME}"/logs /logs      && chown -R neo4j:neo4j /data      && chmod -R 777 /data      && chown -R neo4j:neo4j /logs      && chmod -R 777 /logs      && chown -R neo4j:neo4j "${NEO4J_HOME}"      && chmod -R 777 "${NEO4J_HOME}"      && ln -s /data "${NEO4J_HOME}"/data      && ln -s /logs "${NEO4J_HOME}"/logs      && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json      && rm -rf /tmp/*      && rm -rf /var/lib/apt/lists/*      && apt-get -y purge --auto-remove curl
# Thu, 16 Apr 2020 02:04:00 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:04:01 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:04:01 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:04:01 GMT
COPY file:cd969a3e3d21f58e9a9a346d321ec15de0b681e0976dc4b74a6a00cb6cd0f32c in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:04:01 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:04:01 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:04:02 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b67dfee6ee2225920639c3c30f590fbe5c25ea555e1297bbf2adb2b0e617775`  
		Last Modified: Thu, 16 Apr 2020 02:19:38 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6550692f2fe5bea9bac4d08a5a0648a687fe91d309cd31e0cd4583c489b92b`  
		Last Modified: Thu, 16 Apr 2020 02:19:38 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef744159b6db8eb1207df36e9fff32cab4c973df31258d3a986da28e1aa8d88`  
		Last Modified: Thu, 16 Apr 2020 02:20:07 GMT  
		Size: 135.8 MB (135839553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab73f13338f145e497be18dda41f129bd313bb009511608670e6b0f277ccdc64`  
		Last Modified: Thu, 16 Apr 2020 02:19:38 GMT  
		Size: 5.9 KB (5882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.5.11`

```console
$ docker pull neo4j@sha256:f01b2bd855e9f011423579019d4808344d6727c11e26cd9942c051ebc21cf709
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.5.11` - linux; amd64

```console
$ docker pull neo4j@sha256:043351b062728c302f4741421657530a1d330404eba5279688748b8ef492e001
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.1 MB (228134257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa8a53894c2f55a1abde4e52065447b7473a866d38f83fb564435d305642eb3a`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:09:28 GMT
ENV NEO4J_SHA256=4dd4f2b6c32e216b42ab8d2235f10c4d992d567d36927df93d2d9fb1763e6376 NEO4J_TARBALL=neo4j-community-3.5.11-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:09:28 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.11-unix.tar.gz
# Thu, 16 Apr 2020 02:09:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.11-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:09:31 GMT
COPY multi:7cf12d6a82ce8caa397305af40147113f0c2e3f75bed74dbe4e434adf3288487 in /tmp/ 
# Thu, 16 Apr 2020 02:09:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.11-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:09:50 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:09:50 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:09:50 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:09:51 GMT
COPY file:8d85ed1b091a881aa7d34786c77b3933cd5f54de55a2d3f2248786eef97d873d in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:09:51 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:09:51 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:09:51 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234b723cb929c2281cd9d6d278c1d9cc09b41053cf8667f301d11a5d2ea81966`  
		Last Modified: Thu, 16 Apr 2020 02:25:42 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698fd0943027fd5ea4ef0d71c5009155ab5e88fbb6e4f43315b8c6b21fce5988`  
		Last Modified: Thu, 16 Apr 2020 02:25:41 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c89564aa4b392d657384722370ae05ba3f97217be61864f7ddac8051c99b24`  
		Last Modified: Thu, 16 Apr 2020 02:26:00 GMT  
		Size: 157.2 MB (157193372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478a79085a1f73ef3732e56b2b89c6306a84e675a091d19b24314802cc1f0e93`  
		Last Modified: Thu, 16 Apr 2020 02:25:41 GMT  
		Size: 5.3 KB (5251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.5.11-enterprise`

```console
$ docker pull neo4j@sha256:18676e43d346379b484808f25891a91ca695ae6e66e6476ee296b25fb72822a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.5.11-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:654b8aa7d7f6ec3b4fb961f42bb0ba0d8d28e11629640333152f0d3bfa8959f7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263202643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0d3dc8070ad72231b665a56a45df41bb16142a5a626d381309de9767b939427`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:09:56 GMT
ENV NEO4J_SHA256=e706a6a008bebc5fa06d97f671dc6099d1d1871020373c053a28f695964f88b2 NEO4J_TARBALL=neo4j-enterprise-3.5.11-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:09:56 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.11-unix.tar.gz
# Thu, 16 Apr 2020 02:09:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.11-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:09:58 GMT
COPY multi:7cf12d6a82ce8caa397305af40147113f0c2e3f75bed74dbe4e434adf3288487 in /tmp/ 
# Thu, 16 Apr 2020 02:10:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.11-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:10:13 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:10:13 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:10:14 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:10:14 GMT
COPY file:8d85ed1b091a881aa7d34786c77b3933cd5f54de55a2d3f2248786eef97d873d in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:10:14 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:10:14 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:10:14 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38dc0fad8fd90afd200e14f06bd4460f3c9f58045b3e9966ba8097988bef8c52`  
		Last Modified: Thu, 16 Apr 2020 02:26:04 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49b47e75a82d2027d1de7231a1f30fbf2079867406e814499d911b26ab2676c`  
		Last Modified: Thu, 16 Apr 2020 02:26:04 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22cd8969f99770e3f960609cf6e8c573dbc4771131cb14e8dc2b9404ef48ef2a`  
		Last Modified: Thu, 16 Apr 2020 02:26:19 GMT  
		Size: 192.3 MB (192261763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043c12e22feae2d892fbb2c10b36f1013aa231bf4e1153430b12fc263f5c1eb3`  
		Last Modified: Thu, 16 Apr 2020 02:26:04 GMT  
		Size: 5.3 KB (5251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.5.12`

```console
$ docker pull neo4j@sha256:83a68e3b6ee3be5fad02995971ca4f4c2b95cfca60ed982c9022240e92e7b941
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.5.12` - linux; amd64

```console
$ docker pull neo4j@sha256:5daab270080e7f23cace7cea4b7c97fe8abfbb75f8733a573eced773b64683a4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.3 MB (228329683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95da811c3dffc54f24e1fcbf6e038e77a2e6b269bdf41c2a5c6a5dde07e782fa`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:08:28 GMT
ENV NEO4J_SHA256=3b82b72a211d1b628b64f18f4af9f10b12ed6e2fd0ad94910e11b7fef5d0d86c NEO4J_TARBALL=neo4j-community-3.5.12-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:08:28 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.12-unix.tar.gz
# Thu, 16 Apr 2020 02:08:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.12-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:08:30 GMT
COPY multi:70b59ed932367b04ea9c69354feb959e63e40f0dd9086b2097eaeba453964337 in /tmp/ 
# Thu, 16 Apr 2020 02:08:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.12-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:08:46 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:08:47 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:08:47 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:08:47 GMT
COPY file:8d85ed1b091a881aa7d34786c77b3933cd5f54de55a2d3f2248786eef97d873d in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:08:47 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:08:47 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:08:48 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993364021cff24074fd8aa6a7ed5c22a22aa3b53b31985145984909978d8ccd5`  
		Last Modified: Thu, 16 Apr 2020 02:24:45 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d705ee375ca64ec1103c16d45dee2177b2da881e1d3830b69f3c4423889bb1`  
		Last Modified: Thu, 16 Apr 2020 02:24:44 GMT  
		Size: 303.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04a2590b00c1cf22f5635d8473ee5cd316ccffa8edbc7062b7d81fbb6ae518b`  
		Last Modified: Thu, 16 Apr 2020 02:25:12 GMT  
		Size: 157.4 MB (157388807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f543a20d8c25fe23f9eca93c7c80482e13813ae70c08f96ab8e34cf1dd523eca`  
		Last Modified: Thu, 16 Apr 2020 02:24:45 GMT  
		Size: 5.3 KB (5251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.5.12-enterprise`

```console
$ docker pull neo4j@sha256:f03b00a3994cad88a2b8883097174622c2064cc1dca356cf8bc9336fa7791b34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.5.12-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:68484b9f2c817635cc41cc056cd95bf1c8fb3eb0ba6b044d4b21238d36df89d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.4 MB (263446610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:117fec18a285a01bf75e7a4b276f257f268162d4b0972e3813d7c7f9751e149b`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:08:53 GMT
ENV NEO4J_SHA256=bf23ff236aa5e4b15a840441d7e75d14ff3eb04de8e67edd291c23762be790cd NEO4J_TARBALL=neo4j-enterprise-3.5.12-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:08:53 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.12-unix.tar.gz
# Thu, 16 Apr 2020 02:08:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.12-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:08:55 GMT
COPY multi:70b59ed932367b04ea9c69354feb959e63e40f0dd9086b2097eaeba453964337 in /tmp/ 
# Thu, 16 Apr 2020 02:09:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.12-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:09:18 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:09:18 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:09:18 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:09:19 GMT
COPY file:8d85ed1b091a881aa7d34786c77b3933cd5f54de55a2d3f2248786eef97d873d in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:09:19 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:09:20 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:09:21 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9951de5401ad5ab977f8f8d65b49e5ef174985ec171cc4dafd55da10919c6bd5`  
		Last Modified: Thu, 16 Apr 2020 02:25:16 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec3dcbb3b36712fbdee9e0bddea25c35928b6e50c760e394390a590206b5b68`  
		Last Modified: Thu, 16 Apr 2020 02:25:16 GMT  
		Size: 303.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50089b934ee05f742101c6ff2cc103da3b3ccb521d23534e14405a4d6a5da37`  
		Last Modified: Thu, 16 Apr 2020 02:25:36 GMT  
		Size: 192.5 MB (192505733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49559ddf8a4a08c1e3f1f0322522891c6578b40739219fb6de3db0f9c6702b4`  
		Last Modified: Thu, 16 Apr 2020 02:25:16 GMT  
		Size: 5.3 KB (5251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.5.13`

```console
$ docker pull neo4j@sha256:754c92864d45d4da0cf929b7b438902cec99f914ad44249c47030061f58dd1f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.5.13` - linux; amd64

```console
$ docker pull neo4j@sha256:83adca0b0a6edc32b82084d7eb9b0cc840af7491cae9f1aceef49d6620eec568
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230546080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:855309734c99a6cd820cc77743082a2d63f03fdbff4d1f3d56610e437a2a1abf`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:07:23 GMT
ENV NEO4J_SHA256=2fdb29816bc72894b10f082b5d542fdaa0cf5d9cfdb899d9aac1e34bc2006250 NEO4J_TARBALL=neo4j-community-3.5.13-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:07:23 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.13-unix.tar.gz
# Thu, 16 Apr 2020 02:07:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.13-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:07:24 GMT
COPY multi:70b59ed932367b04ea9c69354feb959e63e40f0dd9086b2097eaeba453964337 in /tmp/ 
# Thu, 16 Apr 2020 02:07:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.13-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:07:41 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:07:42 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:07:42 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:07:42 GMT
COPY file:af001fe5ddb05cac858c69f075bc3cd9077701dfa2891fe6c5a518755a596997 in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:07:42 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:07:43 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:07:43 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89350d90d142f3cf7f122137462775a3a57ba205382dde725ccf5055a123f3b9`  
		Last Modified: Thu, 16 Apr 2020 02:24:02 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98dabbcb2ffc0882419c7adaba65204d1374ff02a2a8aa0d30e3e89e42d2379`  
		Last Modified: Thu, 16 Apr 2020 02:24:02 GMT  
		Size: 302.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f984420d895f79f2d8b9cd53ada583de8d4f422fae2ecc44ec4f50a0d42c90a1`  
		Last Modified: Thu, 16 Apr 2020 02:24:15 GMT  
		Size: 159.6 MB (159605197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09552b9150e09a563e5d0922145cfad477c41225d76f33e9dd6bddc767aeddc7`  
		Last Modified: Thu, 16 Apr 2020 02:24:02 GMT  
		Size: 5.3 KB (5252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.5.13-enterprise`

```console
$ docker pull neo4j@sha256:8853662294d9abddcb132baa64eb8bc4b0711c390e06c509bca2721b8d55f6f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.5.13-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:cbdbce0a72345125eee47dfea5028f63307bf384203b66050d00ed7336dacac6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.7 MB (265673480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfecf317e8dad8f2052a5aeb48ab9af428196accb4ee0a4bcff97337f806727d`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:07:49 GMT
ENV NEO4J_SHA256=e1f74ed3923dc65498f4bf8b17a41d4e05e505e093c23e65ab3e6c47d1ca61af NEO4J_TARBALL=neo4j-enterprise-3.5.13-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:07:50 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.13-unix.tar.gz
# Thu, 16 Apr 2020 02:07:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.13-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:07:53 GMT
COPY multi:70b59ed932367b04ea9c69354feb959e63e40f0dd9086b2097eaeba453964337 in /tmp/ 
# Thu, 16 Apr 2020 02:08:19 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.13-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:08:20 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:08:20 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:08:21 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:08:21 GMT
COPY file:af001fe5ddb05cac858c69f075bc3cd9077701dfa2891fe6c5a518755a596997 in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:08:21 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:08:22 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:08:22 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ccec82643d5014c98c3fbcf108ec80dacfc91867376417628c16670333d14c`  
		Last Modified: Thu, 16 Apr 2020 02:24:19 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f77edf6c5f2f2a9dbd49339d7a6062211b008ca2465fe1c2abe9021377ffd7`  
		Last Modified: Thu, 16 Apr 2020 02:24:19 GMT  
		Size: 302.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e3ff73eeac744bb23b24ef164f969457f0634c97a5013994472ab6f00b5059`  
		Last Modified: Thu, 16 Apr 2020 02:24:41 GMT  
		Size: 194.7 MB (194732603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6de79d85eed355ab6d5c52375d07ee10f03eadb11a6831ac41b6fbbf1e2d237`  
		Last Modified: Thu, 16 Apr 2020 02:24:20 GMT  
		Size: 5.3 KB (5252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.5.14`

```console
$ docker pull neo4j@sha256:f726d0bc0e57d5388f8350593d507a69c3ae8987e5fd1d972cca221d317d13d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.5.14` - linux; amd64

```console
$ docker pull neo4j@sha256:f2bf69077588473b554de312633f80073185df43791aef068ac86e9a59fb7728
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.5 MB (229461144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99fa81cee53614d6f936c67f27d640f4bf9aa82cd858d0980ed47bf60655e625`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:06:08 GMT
ENV NEO4J_SHA256=fb435b11494cde475f748f057a192bcbd8580c7445b380afe9ff52311f334bfe NEO4J_TARBALL=neo4j-community-3.5.14-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:06:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.14-unix.tar.gz
# Thu, 16 Apr 2020 02:06:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.14-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:06:10 GMT
COPY multi:70b59ed932367b04ea9c69354feb959e63e40f0dd9086b2097eaeba453964337 in /tmp/ 
# Thu, 16 Apr 2020 02:06:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.14-unix.tar.gz
RUN apt update      && apt install -y curl wget gosu jq      && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini      && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet      && chmod +x /sbin/tini      && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}      && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet      && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib      && mv /var/lib/neo4j-* "${NEO4J_HOME}"      && rm ${NEO4J_TARBALL}      && mv "${NEO4J_HOME}"/data /data      && mv "${NEO4J_HOME}"/logs /logs      && chown -R neo4j:neo4j /data      && chmod -R 777 /data      && chown -R neo4j:neo4j /logs      && chmod -R 777 /logs      && chown -R neo4j:neo4j "${NEO4J_HOME}"      && chmod -R 777 "${NEO4J_HOME}"      && ln -s /data "${NEO4J_HOME}"/data      && ln -s /logs "${NEO4J_HOME}"/logs      && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json      && rm -rf /tmp/*      && rm -rf /var/lib/apt/lists/*      && apt-get -y purge --auto-remove curl
# Thu, 16 Apr 2020 02:06:40 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:06:40 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:06:41 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:06:41 GMT
COPY file:7ffb493993f443c8153ccfe7de8510ab04c58686ca8ed69aed987a3e80542d26 in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:06:42 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:06:42 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:06:42 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5c2ccfe273e7b48b1432fe192e0ce940c5e77cbd7cec23d685729e996ff511`  
		Last Modified: Thu, 16 Apr 2020 02:23:14 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a846dcbaa89a737cd7126a6e842c97417fbbb9412859783ba0c94363185d324`  
		Last Modified: Thu, 16 Apr 2020 02:23:13 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9b1b6dd75c7a6e12590783c812a2ad8fcba845c0d4e4ed8d377445387854f5`  
		Last Modified: Thu, 16 Apr 2020 02:23:37 GMT  
		Size: 158.5 MB (158520106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bae2890f5a579317e5324308b0b53da6b9ecd68ad2580ffada317840e67f8f`  
		Last Modified: Thu, 16 Apr 2020 02:23:13 GMT  
		Size: 5.4 KB (5412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.5.14-enterprise`

```console
$ docker pull neo4j@sha256:9ea78016737476443efba29c8089ff92e3509ec78f2a4fc797bc65f6a258d756
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.5.14-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:dffbd283095ea17a2066bf56f39e936fa4a69970b197c9871711b7cf16df4998
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.6 MB (264579933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50e197a5f748fdf22e8cdc054df854441dc0446f7639baa7fb836e07a3a21348`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:06:49 GMT
ENV NEO4J_SHA256=8d02047f3196c23849f7b6dda605b98098dbdc694747f1708e119715af3d3e06 NEO4J_TARBALL=neo4j-enterprise-3.5.14-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:06:50 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.14-unix.tar.gz
# Thu, 16 Apr 2020 02:06:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.14-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:06:52 GMT
COPY multi:70b59ed932367b04ea9c69354feb959e63e40f0dd9086b2097eaeba453964337 in /tmp/ 
# Thu, 16 Apr 2020 02:07:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.14-unix.tar.gz
RUN apt update      && apt install -y curl wget gosu jq      && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini      && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet      && chmod +x /sbin/tini      && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}      && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet      && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib      && mv /var/lib/neo4j-* "${NEO4J_HOME}"      && rm ${NEO4J_TARBALL}      && mv "${NEO4J_HOME}"/data /data      && mv "${NEO4J_HOME}"/logs /logs      && chown -R neo4j:neo4j /data      && chmod -R 777 /data      && chown -R neo4j:neo4j /logs      && chmod -R 777 /logs      && chown -R neo4j:neo4j "${NEO4J_HOME}"      && chmod -R 777 "${NEO4J_HOME}"      && ln -s /data "${NEO4J_HOME}"/data      && ln -s /logs "${NEO4J_HOME}"/logs      && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json      && rm -rf /tmp/*      && rm -rf /var/lib/apt/lists/*      && apt-get -y purge --auto-remove curl
# Thu, 16 Apr 2020 02:07:16 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:07:16 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:07:16 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:07:16 GMT
COPY file:7ffb493993f443c8153ccfe7de8510ab04c58686ca8ed69aed987a3e80542d26 in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:07:17 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:07:17 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:07:17 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124654744d86bd2a3b00b6daf581dcdbe2606a1a890c98795d026252ea929a7a`  
		Last Modified: Thu, 16 Apr 2020 02:23:40 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff301ca3c79eb4b2ad483ffcdf2a42540c8138fef2fdb4e36f914219256b387`  
		Last Modified: Thu, 16 Apr 2020 02:23:40 GMT  
		Size: 302.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bdaa5e0e8fe00a9bde9eb012d2e08e5e6210c0430a831334d1ba9ac0c001af`  
		Last Modified: Thu, 16 Apr 2020 02:23:58 GMT  
		Size: 193.6 MB (193638896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7c730788c2fe4614e2660ead29de5f927a84a6867f0c4852e8eae5fa5059d0`  
		Last Modified: Thu, 16 Apr 2020 02:23:40 GMT  
		Size: 5.4 KB (5412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.5.15`

```console
$ docker pull neo4j@sha256:5c3b25fb62c7c6b78fb29f2d67f400ab2f550f95551589df79d3df8484fc43b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.5.15` - linux; amd64

```console
$ docker pull neo4j@sha256:5268457240c57bf4ad705477af7ea83530607d336f32d6c8cc8a90e28c7847fe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.7 MB (206727081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7573e8faba2d6b3bc27defbcac1e1c0c92491ad4a8f0be397b49f464d9082131`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:05:22 GMT
ENV NEO4J_SHA256=32ed30e81aed0fc32d7ca8245b4a25e7aa1c08b89770ea33da1f4b427f1f7664 NEO4J_TARBALL=neo4j-community-3.5.15-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:05:22 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.15-unix.tar.gz
# Thu, 16 Apr 2020 02:05:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.15-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:05:23 GMT
COPY multi:5d2171ebdeb5752d080b96f9ac9e7cf87aeb5949ca626a75789d79e846b648b2 in /tmp/ 
# Thu, 16 Apr 2020 02:05:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.15-unix.tar.gz
RUN apt update      && apt install -y curl wget gosu jq      && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini      && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet      && chmod +x /sbin/tini      && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}      && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet      && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib      && mv /var/lib/neo4j-* "${NEO4J_HOME}"      && rm ${NEO4J_TARBALL}      && mv "${NEO4J_HOME}"/data /data      && mv "${NEO4J_HOME}"/logs /logs      && chown -R neo4j:neo4j /data      && chmod -R 777 /data      && chown -R neo4j:neo4j /logs      && chmod -R 777 /logs      && chown -R neo4j:neo4j "${NEO4J_HOME}"      && chmod -R 777 "${NEO4J_HOME}"      && ln -s /data "${NEO4J_HOME}"/data      && ln -s /logs "${NEO4J_HOME}"/logs      && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json      && rm -rf /tmp/*      && rm -rf /var/lib/apt/lists/*      && apt-get -y purge --auto-remove curl
# Thu, 16 Apr 2020 02:05:38 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:05:38 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:05:38 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:05:39 GMT
COPY file:2302715b081c832649219f56c02e31f4562056b8ba8cd7c7dd5e1cf549d9e537 in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:05:39 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:05:39 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:05:39 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0f69b4a46a77e0a40317238d0ca7f75ae06bd83a134205cbf0516d4a23a5e4`  
		Last Modified: Thu, 16 Apr 2020 02:21:56 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c826bc4d39f3a8e819b5f8896c92aaa1eac5c140145c2b65a67f031644630f4`  
		Last Modified: Thu, 16 Apr 2020 02:21:56 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef3f8567a4108399a5a221ef7794ae01022b521f410da6d288aa9f4a97e0ae4`  
		Last Modified: Thu, 16 Apr 2020 02:22:23 GMT  
		Size: 135.8 MB (135785422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484597a6e4cc85575666bf7948d3cefe0ac6f978730f7edaff53a14dcd3dea2a`  
		Last Modified: Thu, 16 Apr 2020 02:21:56 GMT  
		Size: 5.9 KB (5880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.5.15-enterprise`

```console
$ docker pull neo4j@sha256:965be5208153730fce77fcc16fbdb36a94b5e88a3554bf33120e20c9a06e0b56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.5.15-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:b435d930ad3b410ea3886d626671450cfc5dece7c00b5b786f6e0cbc871c7ca6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.9 MB (241855300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:724c440788682137a9373cbc27241b28826fa7aab06eb58aa66d248dc0ff4d02`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:05:44 GMT
ENV NEO4J_SHA256=0d179b9e7f15c9d63a4b488976117012320b7ba6c8d9ccdca16342d392ea820a NEO4J_TARBALL=neo4j-enterprise-3.5.15-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:05:44 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.15-unix.tar.gz
# Thu, 16 Apr 2020 02:05:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.15-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:05:45 GMT
COPY multi:5d2171ebdeb5752d080b96f9ac9e7cf87aeb5949ca626a75789d79e846b648b2 in /tmp/ 
# Thu, 16 Apr 2020 02:06:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.15-unix.tar.gz
RUN apt update      && apt install -y curl wget gosu jq      && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini      && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet      && chmod +x /sbin/tini      && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}      && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet      && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib      && mv /var/lib/neo4j-* "${NEO4J_HOME}"      && rm ${NEO4J_TARBALL}      && mv "${NEO4J_HOME}"/data /data      && mv "${NEO4J_HOME}"/logs /logs      && chown -R neo4j:neo4j /data      && chmod -R 777 /data      && chown -R neo4j:neo4j /logs      && chmod -R 777 /logs      && chown -R neo4j:neo4j "${NEO4J_HOME}"      && chmod -R 777 "${NEO4J_HOME}"      && ln -s /data "${NEO4J_HOME}"/data      && ln -s /logs "${NEO4J_HOME}"/logs      && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json      && rm -rf /tmp/*      && rm -rf /var/lib/apt/lists/*      && apt-get -y purge --auto-remove curl
# Thu, 16 Apr 2020 02:06:01 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:06:01 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:06:01 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:06:02 GMT
COPY file:2302715b081c832649219f56c02e31f4562056b8ba8cd7c7dd5e1cf549d9e537 in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:06:02 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:06:02 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:06:02 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf9237730e52659c8528aa2b641cae7aab802363f311e7fa8295d42e0fcf7cc`  
		Last Modified: Thu, 16 Apr 2020 02:22:43 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a95ab9f98b720c1e1f1fc4a4eb2f9aa20069317c1bb9b7a9c20bb04dffe5ad`  
		Last Modified: Thu, 16 Apr 2020 02:22:43 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad17a892bd7f3cee63f6b2b510e6f6869fe5df1c7e5c234932d065ab91763f7`  
		Last Modified: Thu, 16 Apr 2020 02:23:09 GMT  
		Size: 170.9 MB (170913642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e2c25362df3691e7e8c7e72ad4047cf7010cb0e5e61dcc659dbf51ddbba7ef`  
		Last Modified: Thu, 16 Apr 2020 02:22:44 GMT  
		Size: 5.9 KB (5880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.5.16`

```console
$ docker pull neo4j@sha256:e8220c02fc1cc9ebc79c80081bd71c90475cfc92c1a816ad9607e29a2ea3a1ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.5.16` - linux; amd64

```console
$ docker pull neo4j@sha256:5bc204bbf28323faa8665159a59f7baa1dbd9fc6ac88ba26111494bbf8c2cf02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.7 MB (206733113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96bc6e18c7377f5460f60ccc283a7b9ad326c9d6bf7d47a1ccc993b9bebc5a1f`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:04:32 GMT
ENV NEO4J_SHA256=3eded9065de1ddd39d519b05845da2f572b5ddb4e6440b93555927f329eaf222 NEO4J_TARBALL=neo4j-community-3.5.16-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:04:33 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.16-unix.tar.gz
# Thu, 16 Apr 2020 02:04:34 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.16-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:04:34 GMT
COPY multi:5d2171ebdeb5752d080b96f9ac9e7cf87aeb5949ca626a75789d79e846b648b2 in /tmp/ 
# Thu, 16 Apr 2020 02:04:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.16-unix.tar.gz
RUN apt update      && apt install -y curl wget gosu jq      && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini      && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet      && chmod +x /sbin/tini      && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}      && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet      && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib      && mv /var/lib/neo4j-* "${NEO4J_HOME}"      && rm ${NEO4J_TARBALL}      && mv "${NEO4J_HOME}"/data /data      && mv "${NEO4J_HOME}"/logs /logs      && chown -R neo4j:neo4j /data      && chmod -R 777 /data      && chown -R neo4j:neo4j /logs      && chmod -R 777 /logs      && chown -R neo4j:neo4j "${NEO4J_HOME}"      && chmod -R 777 "${NEO4J_HOME}"      && ln -s /data "${NEO4J_HOME}"/data      && ln -s /logs "${NEO4J_HOME}"/logs      && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json      && rm -rf /tmp/*      && rm -rf /var/lib/apt/lists/*      && apt-get -y purge --auto-remove curl
# Thu, 16 Apr 2020 02:04:50 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:04:50 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:04:50 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:04:51 GMT
COPY file:2302715b081c832649219f56c02e31f4562056b8ba8cd7c7dd5e1cf549d9e537 in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:04:51 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:04:51 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:04:51 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d112bb0dcbf739fdcc8b0ddb4791ca95d5f3354f4980352db936211d6463be`  
		Last Modified: Thu, 16 Apr 2020 02:21:11 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cbfbbeff9f8015955db201484b8af63e275d0af730508085a632c0752f58521`  
		Last Modified: Thu, 16 Apr 2020 02:21:11 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e474efc4be59ea0297b3f4551d61c5dbb314a510c1cd09eac7a49221c30722`  
		Last Modified: Thu, 16 Apr 2020 02:21:31 GMT  
		Size: 135.8 MB (135791456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb25ce85000a2e8c12101bc309a15456f25a3aa77ab0504980de141993b78f8`  
		Last Modified: Thu, 16 Apr 2020 02:21:11 GMT  
		Size: 5.9 KB (5882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.5.16-enterprise`

```console
$ docker pull neo4j@sha256:5cdaa5053b7274e03777fb4404423b61f0504b5798153f2f3326154af180d7e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.5.16-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:636bbaacb6f582be9cb564f57e56dbeee424116f78efced0cdc1590890f08218
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.9 MB (241864032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a85212503c5df63b1dc6f2f8040e29f45f960e6c6f9e6aef8f13e59b60a6eabc`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:04:57 GMT
ENV NEO4J_SHA256=38dfbaa88b2b17eeb8ec7cf4362327b08f04dd2733374541ba6f233fba6560b2 NEO4J_TARBALL=neo4j-enterprise-3.5.16-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:04:57 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.16-unix.tar.gz
# Thu, 16 Apr 2020 02:04:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.16-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:04:59 GMT
COPY multi:5d2171ebdeb5752d080b96f9ac9e7cf87aeb5949ca626a75789d79e846b648b2 in /tmp/ 
# Thu, 16 Apr 2020 02:05:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.16-unix.tar.gz
RUN apt update      && apt install -y curl wget gosu jq      && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini      && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet      && chmod +x /sbin/tini      && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}      && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet      && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib      && mv /var/lib/neo4j-* "${NEO4J_HOME}"      && rm ${NEO4J_TARBALL}      && mv "${NEO4J_HOME}"/data /data      && mv "${NEO4J_HOME}"/logs /logs      && chown -R neo4j:neo4j /data      && chmod -R 777 /data      && chown -R neo4j:neo4j /logs      && chmod -R 777 /logs      && chown -R neo4j:neo4j "${NEO4J_HOME}"      && chmod -R 777 "${NEO4J_HOME}"      && ln -s /data "${NEO4J_HOME}"/data      && ln -s /logs "${NEO4J_HOME}"/logs      && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json      && rm -rf /tmp/*      && rm -rf /var/lib/apt/lists/*      && apt-get -y purge --auto-remove curl
# Thu, 16 Apr 2020 02:05:14 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:05:14 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:05:14 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:05:15 GMT
COPY file:2302715b081c832649219f56c02e31f4562056b8ba8cd7c7dd5e1cf549d9e537 in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:05:15 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:05:15 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:05:15 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ed92ed4a397575fc0fc0b23ec1d82f6a7b69028182073b8c73228a3cfa5705`  
		Last Modified: Thu, 16 Apr 2020 02:21:35 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7af5c05de4cb34776e4b3792f6e3869786d8c7cb0d96253b2c7665802c7e13`  
		Last Modified: Thu, 16 Apr 2020 02:21:36 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f77564ef625b151070bdd27df1786ba91c7b077999bf676e1f715f73561d40d`  
		Last Modified: Thu, 16 Apr 2020 02:21:52 GMT  
		Size: 170.9 MB (170922374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dc29df786c4d69cde6821213b722f6d3dc4effad069404defe818f8e17b80e`  
		Last Modified: Thu, 16 Apr 2020 02:21:35 GMT  
		Size: 5.9 KB (5882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.5.17`

```console
$ docker pull neo4j@sha256:a6ed5769bacc77022de6c2d52865717d89ffbe98e08ef4ca0f8af892de61d3f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.5.17` - linux; amd64

```console
$ docker pull neo4j@sha256:41cb0222e4768eb455711c88c36a25f346a50abe5fdf1e133cc26089532d2246
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.8 MB (206781212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ded1bd0b452b76c4be8ef887ec8fb1f9f011f9e1cc749c59fbf95053379865b`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:03:43 GMT
ENV NEO4J_SHA256=1c8b6ac0ffd346f0707fe1af713ef74f1c6ce1ea6feb5e9a0bd170e7a8a34a10 NEO4J_TARBALL=neo4j-community-3.5.17-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:03:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.17-unix.tar.gz
# Thu, 16 Apr 2020 02:03:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.17-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:03:44 GMT
COPY multi:5d2171ebdeb5752d080b96f9ac9e7cf87aeb5949ca626a75789d79e846b648b2 in /tmp/ 
# Thu, 16 Apr 2020 02:04:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-3.5.17-unix.tar.gz
RUN apt update      && apt install -y curl wget gosu jq      && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini      && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet      && chmod +x /sbin/tini      && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}      && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet      && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib      && mv /var/lib/neo4j-* "${NEO4J_HOME}"      && rm ${NEO4J_TARBALL}      && mv "${NEO4J_HOME}"/data /data      && mv "${NEO4J_HOME}"/logs /logs      && chown -R neo4j:neo4j /data      && chmod -R 777 /data      && chown -R neo4j:neo4j /logs      && chmod -R 777 /logs      && chown -R neo4j:neo4j "${NEO4J_HOME}"      && chmod -R 777 "${NEO4J_HOME}"      && ln -s /data "${NEO4J_HOME}"/data      && ln -s /logs "${NEO4J_HOME}"/logs      && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json      && rm -rf /tmp/*      && rm -rf /var/lib/apt/lists/*      && apt-get -y purge --auto-remove curl
# Thu, 16 Apr 2020 02:04:00 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:04:01 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:04:01 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:04:01 GMT
COPY file:cd969a3e3d21f58e9a9a346d321ec15de0b681e0976dc4b74a6a00cb6cd0f32c in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:04:01 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:04:01 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:04:02 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b67dfee6ee2225920639c3c30f590fbe5c25ea555e1297bbf2adb2b0e617775`  
		Last Modified: Thu, 16 Apr 2020 02:19:38 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6550692f2fe5bea9bac4d08a5a0648a687fe91d309cd31e0cd4583c489b92b`  
		Last Modified: Thu, 16 Apr 2020 02:19:38 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef744159b6db8eb1207df36e9fff32cab4c973df31258d3a986da28e1aa8d88`  
		Last Modified: Thu, 16 Apr 2020 02:20:07 GMT  
		Size: 135.8 MB (135839553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab73f13338f145e497be18dda41f129bd313bb009511608670e6b0f277ccdc64`  
		Last Modified: Thu, 16 Apr 2020 02:19:38 GMT  
		Size: 5.9 KB (5882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.5.17-enterprise`

```console
$ docker pull neo4j@sha256:96a5f656530a968fbe8452fc9db8b8fca17c1d9c8c2118c5b454ac540b82db8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.5.17-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:ab637cac291015d878dfe06f83fd4c88a944eabf7acaff2c0a5f6f0c0145865b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.9 MB (241912592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb4193fabe66b6f4d4cafdfb33ba6f4cd4f242867dcb425601a04c8e44860285`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:04:07 GMT
ENV NEO4J_SHA256=1f8c60e01e8bcdb5c6921341bd4a783c08a748cabb3348d4e4d2f104544232ca NEO4J_TARBALL=neo4j-enterprise-3.5.17-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:04:08 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.17-unix.tar.gz
# Thu, 16 Apr 2020 02:04:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.17-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:04:09 GMT
COPY multi:5d2171ebdeb5752d080b96f9ac9e7cf87aeb5949ca626a75789d79e846b648b2 in /tmp/ 
# Thu, 16 Apr 2020 02:04:28 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.17-unix.tar.gz
RUN apt update      && apt install -y curl wget gosu jq      && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini      && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet      && chmod +x /sbin/tini      && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}      && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet      && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib      && mv /var/lib/neo4j-* "${NEO4J_HOME}"      && rm ${NEO4J_TARBALL}      && mv "${NEO4J_HOME}"/data /data      && mv "${NEO4J_HOME}"/logs /logs      && chown -R neo4j:neo4j /data      && chmod -R 777 /data      && chown -R neo4j:neo4j /logs      && chmod -R 777 /logs      && chown -R neo4j:neo4j "${NEO4J_HOME}"      && chmod -R 777 "${NEO4J_HOME}"      && ln -s /data "${NEO4J_HOME}"/data      && ln -s /logs "${NEO4J_HOME}"/logs      && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json      && rm -rf /tmp/*      && rm -rf /var/lib/apt/lists/*      && apt-get -y purge --auto-remove curl
# Thu, 16 Apr 2020 02:04:28 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:04:28 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:04:28 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:04:28 GMT
COPY file:cd969a3e3d21f58e9a9a346d321ec15de0b681e0976dc4b74a6a00cb6cd0f32c in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:04:29 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:04:29 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:04:29 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853759afac23098365126554c7bc3639b80831480343f40162958c4b011f689c`  
		Last Modified: Thu, 16 Apr 2020 02:20:30 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba0a8b138c8cb1b72750542f9252a6035c762c1481b8a18afb1733944496ea2`  
		Last Modified: Thu, 16 Apr 2020 02:20:31 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff25b8480dbed949a22c3a62ae9280498403c53645b881f20c771ed93d5f7314`  
		Last Modified: Thu, 16 Apr 2020 02:21:06 GMT  
		Size: 171.0 MB (170970933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da4b1a2b309932072621b746f67b8beae09f6b7ae7ee5c0f9cacbd8f690f0c0`  
		Last Modified: Thu, 16 Apr 2020 02:20:30 GMT  
		Size: 5.9 KB (5882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.5.6`

```console
$ docker pull neo4j@sha256:a623b072a1ef476b6d4f02d3bd4d25f1931cd4be1881f65da24084de01082f59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.5.6` - linux; amd64

```console
$ docker pull neo4j@sha256:68eaa977764e20d1771b062b2fd57af2dd692ef5f817c680c499ae76555d79e9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.9 MB (240867944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7654176abd1c0d5908d196626cc9eaca2e52f7313221818bb31db71cfe608521`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:12:19 GMT
ENV NEO4J_SHA256=f536224565ce27b95947c91a37d52b9ba9e80247d8d3262075b24b8d47f8532a NEO4J_TARBALL=neo4j-community-3.5.6-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:12:19 GMT
ARG NEO4J_URI=http://dist.neo4j.org/neo4j-community-3.5.6-unix.tar.gz
# Thu, 16 Apr 2020 02:12:20 GMT
# ARGS: NEO4J_URI=http://dist.neo4j.org/neo4j-community-3.5.6-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:12:20 GMT
COPY file:696befc481f5ad55a590fa577c3d4ba04c9237326d85b95b729538f95702e110 in /tmp/ 
# Thu, 16 Apr 2020 02:12:37 GMT
# ARGS: NEO4J_URI=http://dist.neo4j.org/neo4j-community-3.5.6-unix.tar.gz
RUN apt update     && apt install -y curl gosu     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs
# Thu, 16 Apr 2020 02:12:37 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:12:38 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:12:38 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:12:39 GMT
COPY file:a6df7d0365e68d6518a68c4e06867141cbce4a327fb803991d77cb4c971aed5d in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:12:39 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:12:39 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:12:40 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277ba75c02df9095cb1ab5c6e4c066a66ae5cf79c5db72125ede5cda13f53a77`  
		Last Modified: Thu, 16 Apr 2020 02:28:11 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0fc70c0bbd2f64050802511e673fc46999cf07f797ee254dcbbfa3748bf6f6`  
		Last Modified: Thu, 16 Apr 2020 02:28:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cd6044aa7f0c7cf11b54053ede204bfae9bfdc7c3d786c3baa0a739deb5696`  
		Last Modified: Thu, 16 Apr 2020 02:28:30 GMT  
		Size: 169.9 MB (169928106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534b975d13b7c250c6ab85eba0b549e6cc8c756ab59334dd4838f1a6b57739e8`  
		Last Modified: Thu, 16 Apr 2020 02:28:12 GMT  
		Size: 4.4 KB (4387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.5.6-enterprise`

```console
$ docker pull neo4j@sha256:c413b3634c22bd7cc6bd2064d4cfdf023bc2f5fdaa274de8f4bd09db9cce1644
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.5.6-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:f1903fb40edec7ea06ae4ff4316e5136fb328c1e7a91811a1289aff055b31ce3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.0 MB (275965434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c83418c84ff9ebcf20897f15cff5f3e51e9d52c303daa299d87a351d83a86e0`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:12:45 GMT
ENV NEO4J_SHA256=0d738dd5bd04aaf15c672e27833480339de5bbe85a56cc932bd15aa27fb99509 NEO4J_TARBALL=neo4j-enterprise-3.5.6-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:12:45 GMT
ARG NEO4J_URI=http://dist.neo4j.org/neo4j-enterprise-3.5.6-unix.tar.gz
# Thu, 16 Apr 2020 02:12:47 GMT
# ARGS: NEO4J_URI=http://dist.neo4j.org/neo4j-enterprise-3.5.6-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:12:48 GMT
COPY file:696befc481f5ad55a590fa577c3d4ba04c9237326d85b95b729538f95702e110 in /tmp/ 
# Thu, 16 Apr 2020 02:13:03 GMT
# ARGS: NEO4J_URI=http://dist.neo4j.org/neo4j-enterprise-3.5.6-unix.tar.gz
RUN apt update     && apt install -y curl gosu     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs
# Thu, 16 Apr 2020 02:13:03 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:13:04 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:13:04 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:13:04 GMT
COPY file:a6df7d0365e68d6518a68c4e06867141cbce4a327fb803991d77cb4c971aed5d in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:13:04 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:13:04 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:13:05 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406338cddac82d6ed91418f4d33040477d3fd7a1fab3500280a5ee986fb903e1`  
		Last Modified: Thu, 16 Apr 2020 02:28:35 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddf80c084930b876ce63293002c57a3058901f4bd0a43a5f85399ca06ac4f36`  
		Last Modified: Thu, 16 Apr 2020 02:28:35 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392cf7edd0b797b17b96f05ee71b5625ba600accb14ebdd53c7e6c1d2b163837`  
		Last Modified: Thu, 16 Apr 2020 02:28:51 GMT  
		Size: 205.0 MB (205025589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c7b3f115ed9b788b655c04257539add98f9312c79786f9029c155810c8569a`  
		Last Modified: Thu, 16 Apr 2020 02:28:34 GMT  
		Size: 4.4 KB (4387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.5.7`

```console
$ docker pull neo4j@sha256:53afcdbdfa176ef81e4f622ab9e7d98b381f3db261205b2931a54e806a36cede
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.5.7` - linux; amd64

```console
$ docker pull neo4j@sha256:ca181d430a3588f804138b18613bf97a3d73032bd27f43015b6ac9780836386a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.9 MB (240932504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:397b302eb58b982ea179eb832fb0aa97c9430487234cea3818af29e753ba79fb`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:11:20 GMT
ENV NEO4J_SHA256=31c8f398df9342928502a7321f045eb8f2b96ec4ded26f9f057dc6f6fa10c60c NEO4J_TARBALL=neo4j-community-3.5.7-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:11:20 GMT
ARG NEO4J_URI=http://dist.neo4j.org/neo4j-community-3.5.7-unix.tar.gz
# Thu, 16 Apr 2020 02:11:21 GMT
# ARGS: NEO4J_URI=http://dist.neo4j.org/neo4j-community-3.5.7-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:11:22 GMT
COPY file:696befc481f5ad55a590fa577c3d4ba04c9237326d85b95b729538f95702e110 in /tmp/ 
# Thu, 16 Apr 2020 02:11:40 GMT
# ARGS: NEO4J_URI=http://dist.neo4j.org/neo4j-community-3.5.7-unix.tar.gz
RUN apt update     && apt install -y curl gosu     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs
# Thu, 16 Apr 2020 02:11:40 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:11:40 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:11:41 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:11:41 GMT
COPY file:a6df7d0365e68d6518a68c4e06867141cbce4a327fb803991d77cb4c971aed5d in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:11:42 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:11:42 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:11:42 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b125a837e7751383bc47ebcf27d73054ef921e73c5bcec2059c3308280603c8f`  
		Last Modified: Thu, 16 Apr 2020 02:27:24 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4d0cac9b5222341ce524b3b2a74a5ff7440c800372de7bd65ed12e990c3a1c`  
		Last Modified: Thu, 16 Apr 2020 02:27:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99cb09cb3410289baa0378cc2f6969434ecd94b83e3c120fc797edaa1b6ddd9`  
		Last Modified: Thu, 16 Apr 2020 02:27:46 GMT  
		Size: 170.0 MB (169992666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b92a4dce11a2d8ac5ad3222e4fe6d9da0587dbee9540370cbb1308fab6063a`  
		Last Modified: Thu, 16 Apr 2020 02:27:25 GMT  
		Size: 4.4 KB (4386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.5.7-enterprise`

```console
$ docker pull neo4j@sha256:cd76d47b69c77495f83cfcb044f9de090e70a68605d42f22d9020d7342cd766c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.5.7-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:956f09c39f3e52596f8e0241bd17a21b0dca04aa4a01174e1d8e20265d051470
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.1 MB (276060707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11e6a7a1f6f503d266dbc0366016db106e0f696b8583c8dedee6cc10908a87b6`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:11:50 GMT
ENV NEO4J_SHA256=f4585c82e43c52d06db3c4194a62766c20adea3566fcc9e9992e3f19d3311e14 NEO4J_TARBALL=neo4j-enterprise-3.5.7-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:11:51 GMT
ARG NEO4J_URI=http://dist.neo4j.org/neo4j-enterprise-3.5.7-unix.tar.gz
# Thu, 16 Apr 2020 02:11:52 GMT
# ARGS: NEO4J_URI=http://dist.neo4j.org/neo4j-enterprise-3.5.7-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:11:53 GMT
COPY file:696befc481f5ad55a590fa577c3d4ba04c9237326d85b95b729538f95702e110 in /tmp/ 
# Thu, 16 Apr 2020 02:12:11 GMT
# ARGS: NEO4J_URI=http://dist.neo4j.org/neo4j-enterprise-3.5.7-unix.tar.gz
RUN apt update     && apt install -y curl gosu     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs
# Thu, 16 Apr 2020 02:12:11 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:12:11 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:12:12 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:12:12 GMT
COPY file:a6df7d0365e68d6518a68c4e06867141cbce4a327fb803991d77cb4c971aed5d in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:12:12 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:12:12 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:12:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d0231b7ba45d045b69cf36c3b1123f129c6189095fe5c398cdd8e2de34fc6`  
		Last Modified: Thu, 16 Apr 2020 02:27:51 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05876da2999db2e07eb13df05ba83db81dc4e25da157ac61718b3ebc425f47bc`  
		Last Modified: Thu, 16 Apr 2020 02:27:51 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e179daa18f91449ce43072baca92e10facec8f4ed027a891dc4e4bbe0ade9bf`  
		Last Modified: Thu, 16 Apr 2020 02:28:07 GMT  
		Size: 205.1 MB (205120867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd6e2367c2b6dba81a469b95b4bcbde523e47aa4ada9050c97cd4bfd5a3d70e`  
		Last Modified: Thu, 16 Apr 2020 02:27:51 GMT  
		Size: 4.4 KB (4387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.5.8`

```console
$ docker pull neo4j@sha256:7bfcd138b928353b801815415d357ab291c26ad4c047375a58f27c79259e9188
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.5.8` - linux; amd64

```console
$ docker pull neo4j@sha256:22501c4840568298fd308005d310e62d8d2f307a1a1dce3b8389c1e911dd5700
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.6 MB (227555870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0a198d735e71844aea1c242319f4e721e6894253855ac95bb8e8a0d81703687`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:10:21 GMT
ENV NEO4J_SHA256=ef714d0e7067d437649e52b6727d258c46a144db2ce567dc4d13b62ee916494e NEO4J_TARBALL=neo4j-community-3.5.8-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:10:21 GMT
ARG NEO4J_URI=http://dist.neo4j.org/neo4j-community-3.5.8-unix.tar.gz
# Thu, 16 Apr 2020 02:10:22 GMT
# ARGS: NEO4J_URI=http://dist.neo4j.org/neo4j-community-3.5.8-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:10:22 GMT
COPY file:696befc481f5ad55a590fa577c3d4ba04c9237326d85b95b729538f95702e110 in /tmp/ 
# Thu, 16 Apr 2020 02:10:43 GMT
# ARGS: NEO4J_URI=http://dist.neo4j.org/neo4j-community-3.5.8-unix.tar.gz
RUN apt update     && apt install -y curl gosu     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:10:43 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:10:44 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:10:44 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:10:45 GMT
COPY file:e07128b8290e38440521f56bbf78b61bbce8be21a97b8b31668594bebdd2bf2b in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:10:45 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:10:47 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:10:47 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27f1799f4f0e5b0085a6fcd6222c0cabd6035d62dc8898aaa07e4ce7281add8`  
		Last Modified: Thu, 16 Apr 2020 02:26:23 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb4cdd73dfa447f4dcb6fd27c186269eefd03df228fb9a7f1704f9924f7f3f0`  
		Last Modified: Thu, 16 Apr 2020 02:26:23 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56118bb9c6d428dc8ec396c9a29aeee728793d0df443c180e7b12c6258a76694`  
		Last Modified: Thu, 16 Apr 2020 02:26:39 GMT  
		Size: 156.6 MB (156616070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778f84f21fbc9935213ef27799fb566ed49588f130808e391202c861f62d28a1`  
		Last Modified: Thu, 16 Apr 2020 02:26:22 GMT  
		Size: 4.3 KB (4347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.5.8-enterprise`

```console
$ docker pull neo4j@sha256:7d337f4e483687ad52e72b02046ecd6bbaf93cf12ca23bddf26a9c6918e207a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.5.8-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:1ec1367eab5e33b0db4fe32f0e6140a34e70e6787cc1949108d89cebb7735729
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.7 MB (262689677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67cfd0027507f9c64955d6f85e87bf011cd366f6fe3b3e90bd9fe018159d701d`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:10:56 GMT
ENV NEO4J_SHA256=29b854cc540b608d86236102417b7d3d06a027e28eb3d9be8fbf7931f713bca3 NEO4J_TARBALL=neo4j-enterprise-3.5.8-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:10:56 GMT
ARG NEO4J_URI=http://dist.neo4j.org/neo4j-enterprise-3.5.8-unix.tar.gz
# Thu, 16 Apr 2020 02:10:58 GMT
# ARGS: NEO4J_URI=http://dist.neo4j.org/neo4j-enterprise-3.5.8-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:10:58 GMT
COPY file:696befc481f5ad55a590fa577c3d4ba04c9237326d85b95b729538f95702e110 in /tmp/ 
# Thu, 16 Apr 2020 02:11:15 GMT
# ARGS: NEO4J_URI=http://dist.neo4j.org/neo4j-enterprise-3.5.8-unix.tar.gz
RUN apt update     && apt install -y curl gosu     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:11:15 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:11:15 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:11:16 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:11:16 GMT
COPY file:e07128b8290e38440521f56bbf78b61bbce8be21a97b8b31668594bebdd2bf2b in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:11:16 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:11:16 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:11:17 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e8397b64f119cc78ad63fffa08fb7b83083c2a129d212edec820b37c58f4c1`  
		Last Modified: Thu, 16 Apr 2020 02:26:47 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:021396b343eb6907bf88faeb6d995ab68343cc4fd4e3c440786f683ef6d87035`  
		Last Modified: Thu, 16 Apr 2020 02:26:47 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd82e26b37ee73ff769d6261c8b07f5ae47d0414c3bac7c32bc67de92b9b98fd`  
		Last Modified: Thu, 16 Apr 2020 02:27:20 GMT  
		Size: 191.7 MB (191749876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355b8fb7e59455e2d4114b8b8ad4747a5d42198d43442da958b1ceb1afbbe20f`  
		Last Modified: Thu, 16 Apr 2020 02:26:47 GMT  
		Size: 4.3 KB (4348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:3.5-enterprise`

```console
$ docker pull neo4j@sha256:96a5f656530a968fbe8452fc9db8b8fca17c1d9c8c2118c5b454ac540b82db8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:3.5-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:ab637cac291015d878dfe06f83fd4c88a944eabf7acaff2c0a5f6f0c0145865b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.9 MB (241912592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb4193fabe66b6f4d4cafdfb33ba6f4cd4f242867dcb425601a04c8e44860285`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 31 Mar 2020 01:34:08 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:34:09 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:29:40 GMT
ENV JAVA_VERSION=8u252
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Thu, 16 Apr 2020 00:30:08 GMT
ENV JAVA_URL_VERSION=8u252b09
# Thu, 16 Apr 2020 00:30:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 16 Apr 2020 02:04:07 GMT
ENV NEO4J_SHA256=1f8c60e01e8bcdb5c6921341bd4a783c08a748cabb3348d4e4d2f104544232ca NEO4J_TARBALL=neo4j-enterprise-3.5.17-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:04:08 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.17-unix.tar.gz
# Thu, 16 Apr 2020 02:04:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.17-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:04:09 GMT
COPY multi:5d2171ebdeb5752d080b96f9ac9e7cf87aeb5949ca626a75789d79e846b648b2 in /tmp/ 
# Thu, 16 Apr 2020 02:04:28 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-3.5.17-unix.tar.gz
RUN apt update      && apt install -y curl wget gosu jq      && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini      && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet      && chmod +x /sbin/tini      && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}      && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet      && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib      && mv /var/lib/neo4j-* "${NEO4J_HOME}"      && rm ${NEO4J_TARBALL}      && mv "${NEO4J_HOME}"/data /data      && mv "${NEO4J_HOME}"/logs /logs      && chown -R neo4j:neo4j /data      && chmod -R 777 /data      && chown -R neo4j:neo4j /logs      && chmod -R 777 /logs      && chown -R neo4j:neo4j "${NEO4J_HOME}"      && chmod -R 777 "${NEO4J_HOME}"      && ln -s /data "${NEO4J_HOME}"/data      && ln -s /logs "${NEO4J_HOME}"/logs      && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json      && rm -rf /tmp/*      && rm -rf /var/lib/apt/lists/*      && apt-get -y purge --auto-remove curl
# Thu, 16 Apr 2020 02:04:28 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:04:28 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:04:28 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:04:28 GMT
COPY file:cd969a3e3d21f58e9a9a346d321ec15de0b681e0976dc4b74a6a00cb6cd0f32c in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:04:29 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:04:29 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:04:29 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d82fb9640b4c941a26ff89bc30bd267489171d25397878e454ca34d3ea8726`  
		Last Modified: Tue, 31 Mar 2020 01:37:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5592c3225b44ab9640bdb6d7478ee80e7811f08938eee2db03b72a3508463e`  
		Last Modified: Thu, 16 Apr 2020 00:34:14 GMT  
		Size: 40.6 MB (40592797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853759afac23098365126554c7bc3639b80831480343f40162958c4b011f689c`  
		Last Modified: Thu, 16 Apr 2020 02:20:30 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba0a8b138c8cb1b72750542f9252a6035c762c1481b8a18afb1733944496ea2`  
		Last Modified: Thu, 16 Apr 2020 02:20:31 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff25b8480dbed949a22c3a62ae9280498403c53645b881f20c771ed93d5f7314`  
		Last Modified: Thu, 16 Apr 2020 02:21:06 GMT  
		Size: 171.0 MB (170970933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da4b1a2b309932072621b746f67b8beae09f6b7ae7ee5c0f9cacbd8f690f0c0`  
		Last Modified: Thu, 16 Apr 2020 02:20:30 GMT  
		Size: 5.9 KB (5882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.0`

```console
$ docker pull neo4j@sha256:5f508da2071f8924d85007f3e9d4c978bcf763d3f631f8bab55213137a2e641d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:4.0` - linux; amd64

```console
$ docker pull neo4j@sha256:ae0dbfa6b5bd8b3706f63033cfb0a378d185774a887f5760f05ac50128d36181
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.7 MB (333738104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f228b6985eae8f6830e250e769cb20104bf1d89c0d269217617775ccc2cf793a`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:33:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 31 Mar 2020 01:33:15 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:33:15 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:28:35 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jdk_
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 00:28:53 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac --version; 	java --version
# Thu, 16 Apr 2020 00:28:53 GMT
CMD ["jshell"]
# Thu, 16 Apr 2020 02:00:04 GMT
ENV NEO4J_SHA256=34db8c51899eced35ca5b9ba764649419f160b944b81abc52ed3587492c07085 NEO4J_TARBALL=neo4j-community-4.0.3-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:00:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.0.3-unix.tar.gz
# Thu, 16 Apr 2020 02:00:05 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.0.3-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:00:06 GMT
COPY multi:5d2171ebdeb5752d080b96f9ac9e7cf87aeb5949ca626a75789d79e846b648b2 in /tmp/ 
# Thu, 16 Apr 2020 02:00:20 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.0.3-unix.tar.gz
RUN apt update     && apt install -y curl wget gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*     && apt-get -y purge --auto-remove curl
# Thu, 16 Apr 2020 02:00:20 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:00:21 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:00:21 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:00:21 GMT
COPY file:2ee670821c25faddd6488b3c5db5184559d53b25bcb108162fb216e902abb8bc in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:00:21 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:00:21 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:00:21 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f5150f7beb631588d1fd1dc420e1529f2db039f6c330d8cad4d7fc17fe51e5`  
		Last Modified: Tue, 31 Mar 2020 01:36:33 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493e3ada4f9660331aa17dee326ff1ef7a8c1b2cb21c79e56198f043e7f98b5d`  
		Last Modified: Thu, 16 Apr 2020 00:32:21 GMT  
		Size: 196.5 MB (196475256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81f58ec492b2c1d59660342c3c53a0439ab65ea84564832099fd9412de833a5`  
		Last Modified: Thu, 16 Apr 2020 02:16:23 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0069cdf9c96072d4c65527727dbbd8442633559454466790acd678377e54e542`  
		Last Modified: Thu, 16 Apr 2020 02:16:22 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7193620b86414659d4efadbe6c236ccff8141733225ec3733451a7ecdef47019`  
		Last Modified: Thu, 16 Apr 2020 02:16:31 GMT  
		Size: 106.9 MB (106914032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047982078c585f3a34320d5565af67793483a19f6eaac0e188930da09ac08842`  
		Last Modified: Thu, 16 Apr 2020 02:16:23 GMT  
		Size: 5.8 KB (5837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.0.0`

```console
$ docker pull neo4j@sha256:26bf65d22094e7d2a2f5dff51b00214d98b284e72f278d78ad5c13f6c60b972b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:4.0.0` - linux; amd64

```console
$ docker pull neo4j@sha256:0e8e379a9e6defe7b5a09d8d75617bf09c3c946cf6b551a829272369f6ba4fcd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.9 MB (357903566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27f761901efce90d21c8483fe5be260c6693e698f8e41540ceb2f904b8a95150`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:33:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 31 Mar 2020 01:33:15 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:33:15 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:28:35 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jdk_
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 00:28:53 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac --version; 	java --version
# Thu, 16 Apr 2020 00:28:53 GMT
CMD ["jshell"]
# Thu, 16 Apr 2020 02:02:38 GMT
ENV NEO4J_SHA256=63c85ee709916f9f5fa2fac7274f1a55bdd44d6ab353cbdd05f050aed9532e82 NEO4J_TARBALL=neo4j-community-4.0.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:02:38 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.0.0-unix.tar.gz
# Thu, 16 Apr 2020 02:02:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.0.0-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:02:39 GMT
COPY multi:1bd8b938243645019f0ce38b6c9eeda97edd652b6f36f34befd360fa818b53e9 in /tmp/ 
# Thu, 16 Apr 2020 02:02:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.0.0-unix.tar.gz
RUN apt update     && apt install -y curl wget gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*     && apt-get -y purge --auto-remove curl
# Thu, 16 Apr 2020 02:02:55 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:02:55 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:02:56 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:02:56 GMT
COPY file:c841ea3ded595df832d5ef9cc6bd4500806b0225676ea4550413353a0f0b82a5 in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:02:56 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:02:56 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:02:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f5150f7beb631588d1fd1dc420e1529f2db039f6c330d8cad4d7fc17fe51e5`  
		Last Modified: Tue, 31 Mar 2020 01:36:33 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493e3ada4f9660331aa17dee326ff1ef7a8c1b2cb21c79e56198f043e7f98b5d`  
		Last Modified: Thu, 16 Apr 2020 00:32:21 GMT  
		Size: 196.5 MB (196475256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00446c167ce19cc2ca2fcbbe9deda1a9e1e11605692b30b0dbd36f47d1d8e1e3`  
		Last Modified: Thu, 16 Apr 2020 02:18:36 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f23a110761128dce6559eab432e9e5c60f6b0d38b9907394da5ebd93374dcc`  
		Last Modified: Thu, 16 Apr 2020 02:18:37 GMT  
		Size: 424.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890cf446fc3752d17751694450147274641359ca3c862a7773c24471a25211bf`  
		Last Modified: Thu, 16 Apr 2020 02:18:58 GMT  
		Size: 131.1 MB (131079287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51f59b102c72a1c04693ac6c6d6400d3a319cd8dea30feedf56a1a4ce189700`  
		Last Modified: Thu, 16 Apr 2020 02:18:36 GMT  
		Size: 6.1 KB (6076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.0.0-enterprise`

```console
$ docker pull neo4j@sha256:f3e3d706b12dd9730164d745e5d0ffcff6dd1ec8142454819b592d2645a336f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:4.0.0-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:e7482114f9bbd22a60bf8dd5926d70fe46789a72a6d1c2e83b9fe5ff7cea3051
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **388.1 MB (388143434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:365a7c3be87554f63aef5c58483e0d16da2e550bc72e6ed9f8c5dcf1c1274b8d`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:33:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 31 Mar 2020 01:33:15 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:33:15 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:28:35 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jdk_
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 00:28:53 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac --version; 	java --version
# Thu, 16 Apr 2020 00:28:53 GMT
CMD ["jshell"]
# Thu, 16 Apr 2020 02:03:03 GMT
ENV NEO4J_SHA256=97060ce09086fa089516a2a3581b3db0d3d0dc4d2dd60daa470fa9ba090a7184 NEO4J_TARBALL=neo4j-enterprise-4.0.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:03:03 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.0.0-unix.tar.gz
# Thu, 16 Apr 2020 02:03:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.0.0-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:03:04 GMT
COPY multi:1bd8b938243645019f0ce38b6c9eeda97edd652b6f36f34befd360fa818b53e9 in /tmp/ 
# Thu, 16 Apr 2020 02:03:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.0.0-unix.tar.gz
RUN apt update     && apt install -y curl wget gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*     && apt-get -y purge --auto-remove curl
# Thu, 16 Apr 2020 02:03:33 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:03:33 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:03:34 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:03:34 GMT
COPY file:c841ea3ded595df832d5ef9cc6bd4500806b0225676ea4550413353a0f0b82a5 in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:03:34 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:03:34 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:03:34 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f5150f7beb631588d1fd1dc420e1529f2db039f6c330d8cad4d7fc17fe51e5`  
		Last Modified: Tue, 31 Mar 2020 01:36:33 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493e3ada4f9660331aa17dee326ff1ef7a8c1b2cb21c79e56198f043e7f98b5d`  
		Last Modified: Thu, 16 Apr 2020 00:32:21 GMT  
		Size: 196.5 MB (196475256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df4fa84dbff94d2b882803c5b6bb26f46717b3d0af2d61d75b0a14dbde63937`  
		Last Modified: Thu, 16 Apr 2020 02:19:03 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcd40ab7ec9de459a9ec6ec938e919d8c07b3084f4e827de7d849ae8553fe22`  
		Last Modified: Thu, 16 Apr 2020 02:19:02 GMT  
		Size: 425.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c765bb7a1fbd052dfe07e0d998a3d77dbe870105a5bdbf5907247e8256d490`  
		Last Modified: Thu, 16 Apr 2020 02:19:33 GMT  
		Size: 161.3 MB (161319152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbdab7dae85d8d4c213803a1c1f088f416c5be003d3aefbb76ca93a1d1acaa55`  
		Last Modified: Thu, 16 Apr 2020 02:19:02 GMT  
		Size: 6.1 KB (6076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.0.1`

```console
$ docker pull neo4j@sha256:7f71ffb1f57379582108c493f0a87e07b99f6df119210d45b295188c442de8ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:4.0.1` - linux; amd64

```console
$ docker pull neo4j@sha256:0b16fa74236e6b67f5988194be0e7fbda04b9a0e120e6b91ccc9b4e533c76b07
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.6 MB (333643149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a8826cdc71e1ce6df08670f3348b626063af95d9590edd7727be588a9d52b7d`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:33:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 31 Mar 2020 01:33:15 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:33:15 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:28:35 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jdk_
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 00:28:53 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac --version; 	java --version
# Thu, 16 Apr 2020 00:28:53 GMT
CMD ["jshell"]
# Thu, 16 Apr 2020 02:01:37 GMT
ENV NEO4J_SHA256=623c807ec23ed5c5e8db665a36bcdcb03a11ca2179ce24b61b220ecac60ace90 NEO4J_TARBALL=neo4j-community-4.0.1-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:01:37 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.0.1-unix.tar.gz
# Thu, 16 Apr 2020 02:01:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.0.1-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:01:39 GMT
COPY multi:5d2171ebdeb5752d080b96f9ac9e7cf87aeb5949ca626a75789d79e846b648b2 in /tmp/ 
# Thu, 16 Apr 2020 02:01:53 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.0.1-unix.tar.gz
RUN apt update     && apt install -y curl wget gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*     && apt-get -y purge --auto-remove curl
# Thu, 16 Apr 2020 02:01:53 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:01:53 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:01:54 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:01:54 GMT
COPY file:180882cf912cbd895c07318211915dd64e94178cf2bd8093fdaf8e8c1b4692f3 in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:01:54 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:01:54 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:01:54 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f5150f7beb631588d1fd1dc420e1529f2db039f6c330d8cad4d7fc17fe51e5`  
		Last Modified: Tue, 31 Mar 2020 01:36:33 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493e3ada4f9660331aa17dee326ff1ef7a8c1b2cb21c79e56198f043e7f98b5d`  
		Last Modified: Thu, 16 Apr 2020 00:32:21 GMT  
		Size: 196.5 MB (196475256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb9f43007a161b5bba8d2ac93d2842cbdad97d64ac0f5cbda7ca51b2763ba15`  
		Last Modified: Thu, 16 Apr 2020 02:18:04 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de308aeddad9edb2757996eb18225840d2bb8b6440d406f407b36992a27277f`  
		Last Modified: Thu, 16 Apr 2020 02:18:04 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74de20981c546c5ce15681a5e6e7dcbdbcb939c411efc508e674a50b464d75cf`  
		Last Modified: Thu, 16 Apr 2020 02:18:15 GMT  
		Size: 106.8 MB (106818828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8a64c9d8105a9452f9a399b3e4fae4f24f19daf641b37cd577d1e6bd8f4ac2`  
		Last Modified: Thu, 16 Apr 2020 02:18:04 GMT  
		Size: 6.1 KB (6085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.0.1-enterprise`

```console
$ docker pull neo4j@sha256:f9b02c90fad6f0f8a2ba83561a05bfcec8c4345d0f1397ae23ff8b2607b19439
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:4.0.1-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:1644de1833e2a77ce2fba5846dd4e70f5d1c6bd6ae893e9ccfc4cb7f2bb72db6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.9 MB (363920396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb75ab5a6fcbaedfa0f9975219ea366ad4d11d83016a7001d01d1829f33bd9e8`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:33:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 31 Mar 2020 01:33:15 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:33:15 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:28:35 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jdk_
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 00:28:53 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac --version; 	java --version
# Thu, 16 Apr 2020 00:28:53 GMT
CMD ["jshell"]
# Thu, 16 Apr 2020 02:01:58 GMT
ENV NEO4J_SHA256=8c6aed4f05246a494ca5ec282f8fd7b4d8342c55adfd3dfa474b4e474f19fe09 NEO4J_TARBALL=neo4j-enterprise-4.0.1-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:01:59 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.0.1-unix.tar.gz
# Thu, 16 Apr 2020 02:02:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.0.1-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:02:00 GMT
COPY multi:5d2171ebdeb5752d080b96f9ac9e7cf87aeb5949ca626a75789d79e846b648b2 in /tmp/ 
# Thu, 16 Apr 2020 02:02:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.0.1-unix.tar.gz
RUN apt update     && apt install -y curl wget gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*     && apt-get -y purge --auto-remove curl
# Thu, 16 Apr 2020 02:02:30 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:02:30 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:02:30 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:02:30 GMT
COPY file:180882cf912cbd895c07318211915dd64e94178cf2bd8093fdaf8e8c1b4692f3 in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:02:30 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:02:30 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:02:31 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f5150f7beb631588d1fd1dc420e1529f2db039f6c330d8cad4d7fc17fe51e5`  
		Last Modified: Tue, 31 Mar 2020 01:36:33 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493e3ada4f9660331aa17dee326ff1ef7a8c1b2cb21c79e56198f043e7f98b5d`  
		Last Modified: Thu, 16 Apr 2020 00:32:21 GMT  
		Size: 196.5 MB (196475256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0f096ba635757f65089d1b386868e4b72b87a5ca22d43538304a80bf7d5720`  
		Last Modified: Thu, 16 Apr 2020 02:18:21 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dded5474f50c19c0d23462eeab22dd10ec4bdc2faa373e61030176c12e1bd8bd`  
		Last Modified: Thu, 16 Apr 2020 02:18:20 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45a105e45dba6b8cb09ba45a573b437ae6ef4f0055fac5814c4b320630360a4`  
		Last Modified: Thu, 16 Apr 2020 02:18:33 GMT  
		Size: 137.1 MB (137096076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42a52a72739cad812dfa8a5d0dd2c2b4f46ca82284a1055466be7228a9d415e`  
		Last Modified: Thu, 16 Apr 2020 02:18:21 GMT  
		Size: 6.1 KB (6085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.0.2`

```console
$ docker pull neo4j@sha256:bc97fe200bd6ebeabf1be46f7cd8e911da4740f2a2bf81f8c0afec2eee305847
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:4.0.2` - linux; amd64

```console
$ docker pull neo4j@sha256:682ced7caffe206213cca600399cdb2dc50bf33c8bdcc6d25d4f4045218d8eb7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.7 MB (333688200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:074d9aef4c9e76069a86799ad8a6a74b0e7852b950ca247ebbc86f133c63e189`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:33:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 31 Mar 2020 01:33:15 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:33:15 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:28:35 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jdk_
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 00:28:53 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac --version; 	java --version
# Thu, 16 Apr 2020 00:28:53 GMT
CMD ["jshell"]
# Thu, 16 Apr 2020 02:00:51 GMT
ENV NEO4J_SHA256=e189f557a41835170fae42ee8d2dea9a94a3c790cfc73f0d9eb28be21b806830 NEO4J_TARBALL=neo4j-community-4.0.2-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:00:51 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.0.2-unix.tar.gz
# Thu, 16 Apr 2020 02:00:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.0.2-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:00:52 GMT
COPY multi:5d2171ebdeb5752d080b96f9ac9e7cf87aeb5949ca626a75789d79e846b648b2 in /tmp/ 
# Thu, 16 Apr 2020 02:01:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.0.2-unix.tar.gz
RUN apt update     && apt install -y curl wget gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*     && apt-get -y purge --auto-remove curl
# Thu, 16 Apr 2020 02:01:06 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:01:06 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:01:07 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:01:07 GMT
COPY file:2ee670821c25faddd6488b3c5db5184559d53b25bcb108162fb216e902abb8bc in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:01:07 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:01:07 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:01:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f5150f7beb631588d1fd1dc420e1529f2db039f6c330d8cad4d7fc17fe51e5`  
		Last Modified: Tue, 31 Mar 2020 01:36:33 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493e3ada4f9660331aa17dee326ff1ef7a8c1b2cb21c79e56198f043e7f98b5d`  
		Last Modified: Thu, 16 Apr 2020 00:32:21 GMT  
		Size: 196.5 MB (196475256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18e87dd2850b5302874ab6efdccf33e54e706036e1f61cd0f02d48ee2ba850e`  
		Last Modified: Thu, 16 Apr 2020 02:17:10 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f708f04b03bc2810331ff8a2f34beae984d425c40403602817a54ed2ddb02f8`  
		Last Modified: Thu, 16 Apr 2020 02:17:10 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d455804fcc9117e1e57f93e1051ad14568b20064a0006d524e32e34ce70a4a`  
		Last Modified: Thu, 16 Apr 2020 02:17:28 GMT  
		Size: 106.9 MB (106864129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e116dd87ac1282c8ac24f1b2ae49f712890ec78e3f161ad6ddfc429ec1b1fa`  
		Last Modified: Thu, 16 Apr 2020 02:17:10 GMT  
		Size: 5.8 KB (5837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.0.2-enterprise`

```console
$ docker pull neo4j@sha256:34092cfa1d1f74de499d075d3745974627fc6c519807a8554fc6302cda5f2182
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:4.0.2-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:c2ff6ee29d5cda252089202833cce0ea0732190566e7afc1d41a7bd62a7dec22
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.0 MB (363986983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef44c91c03ec7cf9d864246c40de5abf5889792036adf4e83091fec0f2dd3da5`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:33:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 31 Mar 2020 01:33:15 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:33:15 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:28:35 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jdk_
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 00:28:53 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac --version; 	java --version
# Thu, 16 Apr 2020 00:28:53 GMT
CMD ["jshell"]
# Thu, 16 Apr 2020 02:01:12 GMT
ENV NEO4J_SHA256=a39791336692e0cabb06f725b9f76dda43c80ef0d8073d696fea8feb5ee502f4 NEO4J_TARBALL=neo4j-enterprise-4.0.2-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:01:12 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.0.2-unix.tar.gz
# Thu, 16 Apr 2020 02:01:13 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.0.2-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:01:13 GMT
COPY multi:5d2171ebdeb5752d080b96f9ac9e7cf87aeb5949ca626a75789d79e846b648b2 in /tmp/ 
# Thu, 16 Apr 2020 02:01:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.0.2-unix.tar.gz
RUN apt update     && apt install -y curl wget gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*     && apt-get -y purge --auto-remove curl
# Thu, 16 Apr 2020 02:01:30 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:01:31 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:01:31 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:01:31 GMT
COPY file:2ee670821c25faddd6488b3c5db5184559d53b25bcb108162fb216e902abb8bc in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:01:31 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:01:31 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:01:32 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f5150f7beb631588d1fd1dc420e1529f2db039f6c330d8cad4d7fc17fe51e5`  
		Last Modified: Tue, 31 Mar 2020 01:36:33 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493e3ada4f9660331aa17dee326ff1ef7a8c1b2cb21c79e56198f043e7f98b5d`  
		Last Modified: Thu, 16 Apr 2020 00:32:21 GMT  
		Size: 196.5 MB (196475256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4db5bc62e5981f48691e244da24cbfe99179906e686a2873ffd173c34f73a0e`  
		Last Modified: Thu, 16 Apr 2020 02:17:32 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc48fc9b1586aa05a4ddbe180b65ee8d664aa8c32e17df671aba843bc444060`  
		Last Modified: Thu, 16 Apr 2020 02:17:32 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a726fb9ce9188cd8f5effc868f010cb9634d758ea22d722f72fb7c759e9c9e14`  
		Last Modified: Thu, 16 Apr 2020 02:17:56 GMT  
		Size: 137.2 MB (137162913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617d3e08e9e83b6718455597e7a83a591c1251b1ba61483e578d20a9c5fcdd53`  
		Last Modified: Thu, 16 Apr 2020 02:17:32 GMT  
		Size: 5.8 KB (5837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.0.3`

```console
$ docker pull neo4j@sha256:5f508da2071f8924d85007f3e9d4c978bcf763d3f631f8bab55213137a2e641d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:4.0.3` - linux; amd64

```console
$ docker pull neo4j@sha256:ae0dbfa6b5bd8b3706f63033cfb0a378d185774a887f5760f05ac50128d36181
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.7 MB (333738104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f228b6985eae8f6830e250e769cb20104bf1d89c0d269217617775ccc2cf793a`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:33:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 31 Mar 2020 01:33:15 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:33:15 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:28:35 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jdk_
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 00:28:53 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac --version; 	java --version
# Thu, 16 Apr 2020 00:28:53 GMT
CMD ["jshell"]
# Thu, 16 Apr 2020 02:00:04 GMT
ENV NEO4J_SHA256=34db8c51899eced35ca5b9ba764649419f160b944b81abc52ed3587492c07085 NEO4J_TARBALL=neo4j-community-4.0.3-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:00:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.0.3-unix.tar.gz
# Thu, 16 Apr 2020 02:00:05 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.0.3-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:00:06 GMT
COPY multi:5d2171ebdeb5752d080b96f9ac9e7cf87aeb5949ca626a75789d79e846b648b2 in /tmp/ 
# Thu, 16 Apr 2020 02:00:20 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.0.3-unix.tar.gz
RUN apt update     && apt install -y curl wget gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*     && apt-get -y purge --auto-remove curl
# Thu, 16 Apr 2020 02:00:20 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:00:21 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:00:21 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:00:21 GMT
COPY file:2ee670821c25faddd6488b3c5db5184559d53b25bcb108162fb216e902abb8bc in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:00:21 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:00:21 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:00:21 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f5150f7beb631588d1fd1dc420e1529f2db039f6c330d8cad4d7fc17fe51e5`  
		Last Modified: Tue, 31 Mar 2020 01:36:33 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493e3ada4f9660331aa17dee326ff1ef7a8c1b2cb21c79e56198f043e7f98b5d`  
		Last Modified: Thu, 16 Apr 2020 00:32:21 GMT  
		Size: 196.5 MB (196475256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81f58ec492b2c1d59660342c3c53a0439ab65ea84564832099fd9412de833a5`  
		Last Modified: Thu, 16 Apr 2020 02:16:23 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0069cdf9c96072d4c65527727dbbd8442633559454466790acd678377e54e542`  
		Last Modified: Thu, 16 Apr 2020 02:16:22 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7193620b86414659d4efadbe6c236ccff8141733225ec3733451a7ecdef47019`  
		Last Modified: Thu, 16 Apr 2020 02:16:31 GMT  
		Size: 106.9 MB (106914032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047982078c585f3a34320d5565af67793483a19f6eaac0e188930da09ac08842`  
		Last Modified: Thu, 16 Apr 2020 02:16:23 GMT  
		Size: 5.8 KB (5837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.0.3-enterprise`

```console
$ docker pull neo4j@sha256:11deffeefe27986ec1319cdb2432b787754857aa4ab3aaa321c449a47aadb67d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:4.0.3-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:2360eae705a2d052fc91241d844f8c2700534114a4b5e3f7ace174f9c5d9f21e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.0 MB (364039192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c3acd9c267620b0cd022cf153c9bfc921694122e0a946cced1486f2f2262adf`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:33:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 31 Mar 2020 01:33:15 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:33:15 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:28:35 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jdk_
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 00:28:53 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac --version; 	java --version
# Thu, 16 Apr 2020 00:28:53 GMT
CMD ["jshell"]
# Thu, 16 Apr 2020 02:00:26 GMT
ENV NEO4J_SHA256=f70ea236b75d4210a49ff4e009388cc99577d50a38eb25ac73fce16eee783aa0 NEO4J_TARBALL=neo4j-enterprise-4.0.3-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:00:26 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.0.3-unix.tar.gz
# Thu, 16 Apr 2020 02:00:27 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.0.3-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:00:27 GMT
COPY multi:5d2171ebdeb5752d080b96f9ac9e7cf87aeb5949ca626a75789d79e846b648b2 in /tmp/ 
# Thu, 16 Apr 2020 02:00:43 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.0.3-unix.tar.gz
RUN apt update     && apt install -y curl wget gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*     && apt-get -y purge --auto-remove curl
# Thu, 16 Apr 2020 02:00:43 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:00:43 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:00:43 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:00:43 GMT
COPY file:2ee670821c25faddd6488b3c5db5184559d53b25bcb108162fb216e902abb8bc in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:00:44 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:00:44 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:00:44 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f5150f7beb631588d1fd1dc420e1529f2db039f6c330d8cad4d7fc17fe51e5`  
		Last Modified: Tue, 31 Mar 2020 01:36:33 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493e3ada4f9660331aa17dee326ff1ef7a8c1b2cb21c79e56198f043e7f98b5d`  
		Last Modified: Thu, 16 Apr 2020 00:32:21 GMT  
		Size: 196.5 MB (196475256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68eafec47d96d5bef369b1dffcf51c0a409c5b396fce6bba4e5b69b9b7b2907`  
		Last Modified: Thu, 16 Apr 2020 02:16:37 GMT  
		Size: 1.4 KB (1368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef797f1cdc41e602dca00286dafde26a32810b1a5c27da72f76ab5f7e3ee51e1`  
		Last Modified: Thu, 16 Apr 2020 02:16:37 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985cc5aef834e25161c5a7fb443472ff301312a46cac082ba3f990320cd48474`  
		Last Modified: Thu, 16 Apr 2020 02:17:03 GMT  
		Size: 137.2 MB (137215117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3990e64a9dcd5ca29f5a9fdf761cc596bbfd94cb37e7d53a56fb72e36a7fd7`  
		Last Modified: Thu, 16 Apr 2020 02:16:37 GMT  
		Size: 5.8 KB (5837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.0-enterprise`

```console
$ docker pull neo4j@sha256:11deffeefe27986ec1319cdb2432b787754857aa4ab3aaa321c449a47aadb67d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:4.0-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:2360eae705a2d052fc91241d844f8c2700534114a4b5e3f7ace174f9c5d9f21e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.0 MB (364039192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c3acd9c267620b0cd022cf153c9bfc921694122e0a946cced1486f2f2262adf`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:33:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 31 Mar 2020 01:33:15 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:33:15 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:28:35 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jdk_
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 00:28:53 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac --version; 	java --version
# Thu, 16 Apr 2020 00:28:53 GMT
CMD ["jshell"]
# Thu, 16 Apr 2020 02:00:26 GMT
ENV NEO4J_SHA256=f70ea236b75d4210a49ff4e009388cc99577d50a38eb25ac73fce16eee783aa0 NEO4J_TARBALL=neo4j-enterprise-4.0.3-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:00:26 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.0.3-unix.tar.gz
# Thu, 16 Apr 2020 02:00:27 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.0.3-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:00:27 GMT
COPY multi:5d2171ebdeb5752d080b96f9ac9e7cf87aeb5949ca626a75789d79e846b648b2 in /tmp/ 
# Thu, 16 Apr 2020 02:00:43 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.0.3-unix.tar.gz
RUN apt update     && apt install -y curl wget gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*     && apt-get -y purge --auto-remove curl
# Thu, 16 Apr 2020 02:00:43 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:00:43 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:00:43 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:00:43 GMT
COPY file:2ee670821c25faddd6488b3c5db5184559d53b25bcb108162fb216e902abb8bc in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:00:44 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:00:44 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:00:44 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f5150f7beb631588d1fd1dc420e1529f2db039f6c330d8cad4d7fc17fe51e5`  
		Last Modified: Tue, 31 Mar 2020 01:36:33 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493e3ada4f9660331aa17dee326ff1ef7a8c1b2cb21c79e56198f043e7f98b5d`  
		Last Modified: Thu, 16 Apr 2020 00:32:21 GMT  
		Size: 196.5 MB (196475256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68eafec47d96d5bef369b1dffcf51c0a409c5b396fce6bba4e5b69b9b7b2907`  
		Last Modified: Thu, 16 Apr 2020 02:16:37 GMT  
		Size: 1.4 KB (1368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef797f1cdc41e602dca00286dafde26a32810b1a5c27da72f76ab5f7e3ee51e1`  
		Last Modified: Thu, 16 Apr 2020 02:16:37 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985cc5aef834e25161c5a7fb443472ff301312a46cac082ba3f990320cd48474`  
		Last Modified: Thu, 16 Apr 2020 02:17:03 GMT  
		Size: 137.2 MB (137215117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3990e64a9dcd5ca29f5a9fdf761cc596bbfd94cb37e7d53a56fb72e36a7fd7`  
		Last Modified: Thu, 16 Apr 2020 02:16:37 GMT  
		Size: 5.8 KB (5837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise`

```console
$ docker pull neo4j@sha256:11deffeefe27986ec1319cdb2432b787754857aa4ab3aaa321c449a47aadb67d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:2360eae705a2d052fc91241d844f8c2700534114a4b5e3f7ace174f9c5d9f21e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.0 MB (364039192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c3acd9c267620b0cd022cf153c9bfc921694122e0a946cced1486f2f2262adf`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:33:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 31 Mar 2020 01:33:15 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:33:15 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:28:35 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jdk_
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 00:28:53 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac --version; 	java --version
# Thu, 16 Apr 2020 00:28:53 GMT
CMD ["jshell"]
# Thu, 16 Apr 2020 02:00:26 GMT
ENV NEO4J_SHA256=f70ea236b75d4210a49ff4e009388cc99577d50a38eb25ac73fce16eee783aa0 NEO4J_TARBALL=neo4j-enterprise-4.0.3-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:00:26 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.0.3-unix.tar.gz
# Thu, 16 Apr 2020 02:00:27 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.0.3-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:00:27 GMT
COPY multi:5d2171ebdeb5752d080b96f9ac9e7cf87aeb5949ca626a75789d79e846b648b2 in /tmp/ 
# Thu, 16 Apr 2020 02:00:43 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.0.3-unix.tar.gz
RUN apt update     && apt install -y curl wget gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*     && apt-get -y purge --auto-remove curl
# Thu, 16 Apr 2020 02:00:43 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:00:43 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:00:43 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:00:43 GMT
COPY file:2ee670821c25faddd6488b3c5db5184559d53b25bcb108162fb216e902abb8bc in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:00:44 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:00:44 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:00:44 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f5150f7beb631588d1fd1dc420e1529f2db039f6c330d8cad4d7fc17fe51e5`  
		Last Modified: Tue, 31 Mar 2020 01:36:33 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493e3ada4f9660331aa17dee326ff1ef7a8c1b2cb21c79e56198f043e7f98b5d`  
		Last Modified: Thu, 16 Apr 2020 00:32:21 GMT  
		Size: 196.5 MB (196475256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68eafec47d96d5bef369b1dffcf51c0a409c5b396fce6bba4e5b69b9b7b2907`  
		Last Modified: Thu, 16 Apr 2020 02:16:37 GMT  
		Size: 1.4 KB (1368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef797f1cdc41e602dca00286dafde26a32810b1a5c27da72f76ab5f7e3ee51e1`  
		Last Modified: Thu, 16 Apr 2020 02:16:37 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985cc5aef834e25161c5a7fb443472ff301312a46cac082ba3f990320cd48474`  
		Last Modified: Thu, 16 Apr 2020 02:17:03 GMT  
		Size: 137.2 MB (137215117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3990e64a9dcd5ca29f5a9fdf761cc596bbfd94cb37e7d53a56fb72e36a7fd7`  
		Last Modified: Thu, 16 Apr 2020 02:16:37 GMT  
		Size: 5.8 KB (5837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:latest`

```console
$ docker pull neo4j@sha256:5f508da2071f8924d85007f3e9d4c978bcf763d3f631f8bab55213137a2e641d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neo4j:latest` - linux; amd64

```console
$ docker pull neo4j@sha256:ae0dbfa6b5bd8b3706f63033cfb0a378d185774a887f5760f05ac50128d36181
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.7 MB (333738104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f228b6985eae8f6830e250e769cb20104bf1d89c0d269217617775ccc2cf793a`
-	Entrypoint: `["\/sbin\/tini","-g","--","\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:31:09 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 01:33:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 31 Mar 2020 01:33:15 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:33:15 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 00:28:35 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jdk_
# Thu, 16 Apr 2020 00:28:36 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 00:28:53 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac --version; 	java --version
# Thu, 16 Apr 2020 00:28:53 GMT
CMD ["jshell"]
# Thu, 16 Apr 2020 02:00:04 GMT
ENV NEO4J_SHA256=34db8c51899eced35ca5b9ba764649419f160b944b81abc52ed3587492c07085 NEO4J_TARBALL=neo4j-community-4.0.3-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j TINI_VERSION=v0.18.0 TINI_SHA256=12d20136605531b09a2c2dac02ccee85e1b874eb322ef6baf7561cd93f93c855
# Thu, 16 Apr 2020 02:00:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.0.3-unix.tar.gz
# Thu, 16 Apr 2020 02:00:05 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.0.3-unix.tar.gz
RUN addgroup --system neo4j && adduser --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Apr 2020 02:00:06 GMT
COPY multi:5d2171ebdeb5752d080b96f9ac9e7cf87aeb5949ca626a75789d79e846b648b2 in /tmp/ 
# Thu, 16 Apr 2020 02:00:20 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.0.3-unix.tar.gz
RUN apt update     && apt install -y curl wget gosu jq     && curl -L --fail --silent --show-error "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini" > /sbin/tini     && echo "${TINI_SHA256}  /sbin/tini" | sha256sum -c --strict --quiet     && chmod +x /sbin/tini     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /tmp/neo4jlabs-plugins.json /neo4jlabs-plugins.json     && rm -rf /tmp/*     && rm -rf /var/lib/apt/lists/*     && apt-get -y purge --auto-remove curl
# Thu, 16 Apr 2020 02:00:20 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 02:00:21 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Apr 2020 02:00:21 GMT
VOLUME [/data /logs]
# Thu, 16 Apr 2020 02:00:21 GMT
COPY file:2ee670821c25faddd6488b3c5db5184559d53b25bcb108162fb216e902abb8bc in /docker-entrypoint.sh 
# Thu, 16 Apr 2020 02:00:21 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Apr 2020 02:00:21 GMT
ENTRYPOINT ["/sbin/tini" "-g" "--" "/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:00:21 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e36ba391601ebce2c22f34982f56ce9236ca9cfdef13b2bc60457881d84e8`  
		Last Modified: Tue, 31 Mar 2020 01:35:26 GMT  
		Size: 3.2 MB (3249089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f5150f7beb631588d1fd1dc420e1529f2db039f6c330d8cad4d7fc17fe51e5`  
		Last Modified: Tue, 31 Mar 2020 01:36:33 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493e3ada4f9660331aa17dee326ff1ef7a8c1b2cb21c79e56198f043e7f98b5d`  
		Last Modified: Thu, 16 Apr 2020 00:32:21 GMT  
		Size: 196.5 MB (196475256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81f58ec492b2c1d59660342c3c53a0439ab65ea84564832099fd9412de833a5`  
		Last Modified: Thu, 16 Apr 2020 02:16:23 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0069cdf9c96072d4c65527727dbbd8442633559454466790acd678377e54e542`  
		Last Modified: Thu, 16 Apr 2020 02:16:22 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7193620b86414659d4efadbe6c236ccff8141733225ec3733451a7ecdef47019`  
		Last Modified: Thu, 16 Apr 2020 02:16:31 GMT  
		Size: 106.9 MB (106914032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047982078c585f3a34320d5565af67793483a19f6eaac0e188930da09ac08842`  
		Last Modified: Thu, 16 Apr 2020 02:16:23 GMT  
		Size: 5.8 KB (5837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
