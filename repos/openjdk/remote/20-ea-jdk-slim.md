## `openjdk:20-ea-jdk-slim`

```console
$ docker pull openjdk@sha256:4da85bd5850786ac2535e3ebd9bf118dea813834e5a60771cce59cd1c2008eb8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-jdk-slim` - linux; amd64

```console
$ docker pull openjdk@sha256:e7213bc05820ca834ce799c48543ab3fe5a7d806dcee622ae2404b801cb15d1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.2 MB (230224668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee643966a10cfeeaed41d5f73e037c2529d7e68b93283a7ddc6ebbdb1cecd49a`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 07:01:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 07:01:59 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 13 Sep 2022 07:01:59 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Sep 2022 07:01:59 GMT
ENV LANG=C.UTF-8
# Wed, 21 Sep 2022 00:01:00 GMT
ENV JAVA_VERSION=20-ea+15
# Wed, 21 Sep 2022 00:01:14 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/15/GPL/openjdk-20-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='2ee417bc5d9f36c634a5e004c201967b70b6b3a5382147d74406cc9b015eac97'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/15/GPL/openjdk-20-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='6ec219647905af892891d6fd018538043bf19cfae2a40df439b9fde070476681'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 21 Sep 2022 00:01:15 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e69b53e7b682e7dd85bc12ebde7a4734ebd6cf1c24c9932ed6d0f5ad309612`  
		Last Modified: Tue, 13 Sep 2022 07:09:16 GMT  
		Size: 1.6 MB (1582302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b0a1563dc68e3130b2df20bc755f3a418ba00510cdd654838234ef2be7ed25`  
		Last Modified: Wed, 21 Sep 2022 00:06:27 GMT  
		Size: 197.2 MB (197238245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-jdk-slim` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:c970ebe098a299169705beeac1daf569006432ede7c657eb3e73943feb2eb7a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.2 MB (227171963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:573b89cf2f6cee21bf7b83dfd2b533c09233a718f2db5541156a2dc759d73bea`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 14:38:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 14:38:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 13 Sep 2022 14:38:03 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Sep 2022 14:38:04 GMT
ENV LANG=C.UTF-8
# Wed, 21 Sep 2022 00:34:35 GMT
ENV JAVA_VERSION=20-ea+15
# Wed, 21 Sep 2022 00:34:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/15/GPL/openjdk-20-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='2ee417bc5d9f36c634a5e004c201967b70b6b3a5382147d74406cc9b015eac97'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/15/GPL/openjdk-20-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='6ec219647905af892891d6fd018538043bf19cfae2a40df439b9fde070476681'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 21 Sep 2022 00:34:50 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dff4c2315c7ba5819fcc75c0bf4e213049019660b96d9d0fa49d7361693e85`  
		Last Modified: Tue, 13 Sep 2022 14:50:08 GMT  
		Size: 1.6 MB (1565978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1877dec275ae0349457b089cef847a78516e87998ef282d57d54b816e39f292`  
		Last Modified: Wed, 21 Sep 2022 00:43:03 GMT  
		Size: 195.6 MB (195551746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
