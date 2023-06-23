## `openjdk:22-ea-3-slim`

```console
$ docker pull openjdk@sha256:5f0433b72659a8a7aa0f1f3972942d719e11fee14c8f3d396cf6d19e54ded775
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `openjdk:22-ea-3-slim` - linux; amd64

```console
$ docker pull openjdk@sha256:73a243f484702ad3a05e2eb169493752e33029ec56f0eb11270bf75ea2dde9d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.1 MB (238139607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e27b4973dbb99d5b1d136b7baf2e91bc9afa9352ec15d2a1df9e244ecc0375`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:42 GMT
ADD file:ba1250b6ecd5dd09d4914189d72741c2817988994e7da514bf62be439a34bdb5 in / 
# Mon, 12 Jun 2023 23:20:42 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 18:42:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:42:40 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Tue, 13 Jun 2023 18:42:40 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 18:42:40 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jun 2023 00:26:30 GMT
ENV JAVA_VERSION=22-ea+3
# Fri, 23 Jun 2023 00:26:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/3/GPL/openjdk-22-ea+3_linux-x64_bin.tar.gz'; 			downloadSha256='6541c5f5f08ec100af327c36768e302185851f548f6c33d1fe26250133998d5a'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/3/GPL/openjdk-22-ea+3_linux-aarch64_bin.tar.gz'; 			downloadSha256='e94529988d1c61d552981cc44896e13a1c49f3720567b2a92ad103f24291a167'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 23 Jun 2023 00:26:45 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5b5fe70539cd6989aa19f25826309f9715a9489cf1c057982d6a84c1ad8975c7`  
		Last Modified: Mon, 12 Jun 2023 23:25:49 GMT  
		Size: 29.1 MB (29124744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3811e3d95202c7b7a774cb28118272b61b9a762e2b037aa469fd2c653d628bd6`  
		Last Modified: Tue, 13 Jun 2023 18:45:05 GMT  
		Size: 4.0 MB (4007955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba070bd57331f7e8949c395cb55075d3fc76d49c445bed959d187e0be6bfa60`  
		Last Modified: Fri, 23 Jun 2023 00:31:49 GMT  
		Size: 205.0 MB (205006908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
