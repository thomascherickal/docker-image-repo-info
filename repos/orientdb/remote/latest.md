## `orientdb:latest`

```console
$ docker pull orientdb@sha256:38dbe314b8eedf3976a4a5d7f8e981187456462c3600179d46d6ef3928190353
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `orientdb:latest` - linux; amd64

```console
$ docker pull orientdb@sha256:da3bd7d689629eef577f5ddeec54b3adad403d49598ecacde75fee27737c6b1c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.0 MB (212956647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ae605e4930ba8d407497f5ea430cd1de039dd596e1f2e9493913fb6b5104166`
-	Default Command: `["server.sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:52:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 00:57:17 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 29 Mar 2022 00:57:17 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 29 Mar 2022 00:57:17 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 00:57:18 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 00:57:18 GMT
ENV JAVA_VERSION=8u322
# Tue, 29 Mar 2022 00:57:38 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 30 Mar 2022 03:52:33 GMT
MAINTAINER OrientDB LTD (info@orientdb.com)
# Wed, 30 Mar 2022 03:52:33 GMT
ARG ORIENTDB_DOWNLOAD_SERVER
# Wed, 30 Mar 2022 03:52:33 GMT
ENV ORIENTDB_VERSION=3.2.5
# Wed, 30 Mar 2022 03:52:33 GMT
ENV ORIENTDB_DOWNLOAD_MD5=76c3e185d26c0bbc2de194f063b0c2c0
# Wed, 30 Mar 2022 03:52:33 GMT
ENV ORIENTDB_DOWNLOAD_SHA1=f444c92aa00cabba18874b9a3c003eda68296f5e
# Wed, 30 Mar 2022 03:52:33 GMT
ENV ORIENTDB_DOWNLOAD_URL=https://repo1.maven.org/maven2/com/orientechnologies/orientdb-community/3.2.5/orientdb-community-3.2.5.tar.gz
# Wed, 30 Mar 2022 03:52:38 GMT
RUN apt update     && apt install -y curl wget     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 03:52:41 GMT
RUN mkdir /orientdb &&   wget  $ORIENTDB_DOWNLOAD_URL   && echo "$ORIENTDB_DOWNLOAD_MD5 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | md5sum -c -   && echo "$ORIENTDB_DOWNLOAD_SHA1 *orientdb-community-$ORIENTDB_VERSION.tar.gz" | sha1sum -c -   && tar -xvzf orientdb-community-$ORIENTDB_VERSION.tar.gz -C /orientdb --strip-components=1   && rm orientdb-community-$ORIENTDB_VERSION.tar.gz   && rm -rf /orientdb/databases/*
# Wed, 30 Mar 2022 03:52:41 GMT
ENV PATH=/orientdb/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 03:52:42 GMT
VOLUME [/orientdb/backup /orientdb/databases /orientdb/config]
# Wed, 30 Mar 2022 03:52:42 GMT
WORKDIR /orientdb
# Wed, 30 Mar 2022 03:52:42 GMT
EXPOSE 2424
# Wed, 30 Mar 2022 03:52:42 GMT
EXPOSE 2480
# Wed, 30 Mar 2022 03:52:42 GMT
CMD ["server.sh"]
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1dc05f270bad654ee17f1143c48586c188a72929a128d61fd8ae15905d7b00`  
		Last Modified: Tue, 29 Mar 2022 01:04:32 GMT  
		Size: 1.6 MB (1582122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e68111de204b0c46a897b6ac5dd87c1e8aafae5aca100c679358a7a00513a8`  
		Last Modified: Tue, 29 Mar 2022 01:13:37 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e471efaa2016146a5e0876d311ea5cb43c98063f897d841810fb30bb2c29ac`  
		Last Modified: Tue, 29 Mar 2022 01:13:46 GMT  
		Size: 106.3 MB (106344248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ddac555735ddddfda36da2d3024e6d9300ade97014dd87e4af4c40b624a82e`  
		Last Modified: Wed, 30 Mar 2022 03:54:48 GMT  
		Size: 2.1 MB (2105594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:401579a3ee124897427fe479d7b93b65d6e652e0b1275591c804c7b821322ea1`  
		Last Modified: Wed, 30 Mar 2022 03:54:52 GMT  
		Size: 71.5 MB (71546016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
