## `openjdk:20-ea-jdk-slim`

```console
$ docker pull openjdk@sha256:63f023d73c75f488a72f897dbd0b56a07410a0f2fe4f27b6451b340d996e379c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `openjdk:20-ea-jdk-slim` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:f4bf2202ab416bc49140fecb2695f44c3ec89636b500df0e75e05c4f2a422c3a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.5 MB (227539027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5232eaf57456dcf24fe1976a329631cd203cfe8c95a617cf1146ac213912ab68`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:37:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Jun 2022 00:50:18 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Thu, 16 Jun 2022 00:50:19 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Jun 2022 00:50:20 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jun 2022 00:50:21 GMT
ENV JAVA_VERSION=20-ea+1
# Thu, 16 Jun 2022 00:50:37 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/1/GPL/openjdk-20-ea+1_linux-x64_bin.tar.gz'; 			downloadSha256='0abed92a0e13e5d0f0d02463a90b21a040db83ea57617f5c61c5547862152766'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/1/GPL/openjdk-20-ea+1_linux-aarch64_bin.tar.gz'; 			downloadSha256='898a2f8ca4e530d154e94ca685ef4f03341cd78f3514661a03c8f87bfbdd2371'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 16 Jun 2022 00:50:38 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c8727eedfb1755681add8fcb3c2c35d3b41f8231849edcec84588c6404f3b3`  
		Last Modified: Sat, 28 May 2022 01:54:41 GMT  
		Size: 1.4 MB (1361240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f838126c01f53b92c193533b42d7d46e82b496fc6ccd3d596ca5401c518b0c`  
		Last Modified: Thu, 16 Jun 2022 01:06:29 GMT  
		Size: 196.1 MB (196112059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
