## `openjdk:22-ea-jdk-bookworm`

```console
$ docker pull openjdk@sha256:86fadf05d7bc6c9a05d545e8396f7c635d1f4cc4a609548dc0e4ca8119daf487
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:22-ea-jdk-bookworm` - linux; amd64

```console
$ docker pull openjdk@sha256:f04cdff34b2838c10dd9e10ee211a527a7ceb428ebb15a00710ae8c7b0201ec8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.6 MB (359553798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e697237ade9a72c0dad0a81421a2347b7cf752d47cbc28eb71858d439a7e953e`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:29 GMT
ADD file:cc1376ecb3d9e93e4160573c110da753ffeb2efe2223351f1fbf483d89f1a756 in / 
# Thu, 27 Jul 2023 23:24:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:01:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:08:29 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Fri, 28 Jul 2023 04:08:29 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 04:08:30 GMT
ENV LANG=C.UTF-8
# Sat, 12 Aug 2023 00:02:55 GMT
ENV JAVA_VERSION=22-ea+10
# Sat, 12 Aug 2023 00:03:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/10/GPL/openjdk-22-ea+10_linux-x64_bin.tar.gz'; 			downloadSha256='aa3e45c81e7269d389411b52c17721916d2acb7d3e7ab6367c62138063f5052b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/10/GPL/openjdk-22-ea+10_linux-aarch64_bin.tar.gz'; 			downloadSha256='e143f6323650bd4747e4304ef07ba80ade1510a71325bc36a7c4f51939cfe423'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Aug 2023 00:03:06 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:785ef8b9b236a5f027f33cae77513051704c0538bff455ff5548105c954c3b1c`  
		Last Modified: Thu, 27 Jul 2023 23:29:02 GMT  
		Size: 49.6 MB (49557354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6dad8f55ae6c733e986316bd08205c8b2c41640bf8d08ff6e9bbcb6884304f`  
		Last Modified: Fri, 28 Jul 2023 03:07:18 GMT  
		Size: 24.0 MB (24030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd36c7bfe5f4bdffcc0bbb74b0fb38feb35c286ea58b5992617fb38b0c933603`  
		Last Modified: Fri, 28 Jul 2023 03:07:36 GMT  
		Size: 64.1 MB (64112293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23081abc6d37ce8cde709fa970343e4a97f93dc71c081510386ac63a6804ae7f`  
		Last Modified: Fri, 28 Jul 2023 04:12:13 GMT  
		Size: 16.9 MB (16947358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14ec8d804acc48bb9accf0f6dc73541c1977ffb7262439af92dff225e4bfef2`  
		Last Modified: Sat, 12 Aug 2023 00:08:04 GMT  
		Size: 204.9 MB (204906254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-ea-jdk-bookworm` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:ca10dfca3a2bb4772d55e577a66e12ebe354d5fb6c04a4897126aa6970f88f6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.1 MB (358123275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4a220f1bebb9371897a833fdb15615c6e2b6ceb7f0ea8c7ecd53149c180a58c`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:49 GMT
ADD file:ca43018e3d97d44b49e60fe002bb20834a74cc1163d7e95ad50d549f072de158 in / 
# Tue, 15 Aug 2023 23:39:49 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:21:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:21:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:11:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:11:27 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Wed, 16 Aug 2023 04:11:27 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 04:11:27 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 04:11:27 GMT
ENV JAVA_VERSION=22-ea+10
# Wed, 16 Aug 2023 04:11:56 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/10/GPL/openjdk-22-ea+10_linux-x64_bin.tar.gz'; 			downloadSha256='aa3e45c81e7269d389411b52c17721916d2acb7d3e7ab6367c62138063f5052b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/10/GPL/openjdk-22-ea+10_linux-aarch64_bin.tar.gz'; 			downloadSha256='e143f6323650bd4747e4304ef07ba80ade1510a71325bc36a7c4f51939cfe423'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 16 Aug 2023 04:11:57 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a014e5e7d08c37cf1703b97e701ccdc850e4a18d0ee679f03aa875dcd520aa85`  
		Last Modified: Tue, 15 Aug 2023 23:42:59 GMT  
		Size: 49.6 MB (49591310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715cea74ecbb15cb82efef1e77dd60c31d90b01d1286d6f39b4562afaebe75f3`  
		Last Modified: Wed, 16 Aug 2023 01:38:30 GMT  
		Size: 23.6 MB (23570046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003f1109a21287fa17dc866e87e8c6685113960cbb0379fee8f42b83de63c647`  
		Last Modified: Wed, 16 Aug 2023 01:38:47 GMT  
		Size: 64.0 MB (63988473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e1d2ce07002848455170902f2b6ea91a492e5b318bc6ae2fb7691c51b7e9ed`  
		Last Modified: Wed, 16 Aug 2023 04:16:10 GMT  
		Size: 17.7 MB (17729096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74f9b37cd525c2bbc6d7e569fb6e71c3a19d803390985b57eeab1cb5fe5911a`  
		Last Modified: Wed, 16 Aug 2023 04:16:21 GMT  
		Size: 203.2 MB (203244350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
