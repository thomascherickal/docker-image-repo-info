## `openjdk:21-ea-slim-buster`

```console
$ docker pull openjdk@sha256:81f4d31bedaba7f08cfbb23f2f57c6b9c1a90628435087876390bbaee3e89672
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-slim-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:242dfa90e09795c292ccb61d4c3e648397f34e8a3934e96e5f924187d335d240
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.7 MB (232656197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c931a9ffe1821c903d61c2b46151e1402a6527248c48435a9394ee6f2973dea`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 02 May 2023 23:47:16 GMT
ADD file:00bc0eda6d2eb0f8ad4abc654f762ffb9ec7e8d1c95d0cc0e7d0cba176d33e27 in / 
# Tue, 02 May 2023 23:47:17 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:20:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:20:16 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Wed, 03 May 2023 18:20:16 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 18:20:16 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 23:37:45 GMT
ENV JAVA_VERSION=21-ea+21
# Thu, 04 May 2023 23:38:00 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/21/GPL/openjdk-21-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='218aa2d9ef829851d8eafe470922cefd372aa31b68cdab3aa0691c0492e6adde'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/21/GPL/openjdk-21-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='449a26a88e27c331c9565a95892533f33792094f23f28a71b880a60588ddf0c2'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 04 May 2023 23:38:00 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:25ff99d195814e98b7ef4708519299d9f177def504f9b718c61eb82c7f0b34be`  
		Last Modified: Tue, 02 May 2023 23:51:01 GMT  
		Size: 27.1 MB (27138959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5572f0fb7b53dfd62a51ebc6aea399bb961104546222935c7fc356213a2108`  
		Last Modified: Wed, 03 May 2023 18:22:41 GMT  
		Size: 3.3 MB (3278806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77b421213ab63f3e46365c6cdfe74777cca6052f5fd2af3ad2863aa97c1d685`  
		Last Modified: Thu, 04 May 2023 23:41:30 GMT  
		Size: 202.2 MB (202238432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-slim-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:df4a8dd62f9d45c273738200e6b9f82676cb69be6be8c9de6db3ba3c8bf55b88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.7 MB (229661921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a92015d9d297041e426d44310d12eea02ad8093b46037da6c41272a5c0427738`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 03 May 2023 00:23:05 GMT
ADD file:1d8cf95f550bb4b86ad82b22e7195179335fa3b327fd1f1ba1e6c8357ee15c94 in / 
# Wed, 03 May 2023 00:23:05 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:05:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 17:05:27 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Wed, 03 May 2023 17:05:27 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 17:05:27 GMT
ENV LANG=C.UTF-8
# Fri, 05 May 2023 00:03:25 GMT
ENV JAVA_VERSION=21-ea+21
# Fri, 05 May 2023 00:03:41 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/21/GPL/openjdk-21-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='218aa2d9ef829851d8eafe470922cefd372aa31b68cdab3aa0691c0492e6adde'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/21/GPL/openjdk-21-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='449a26a88e27c331c9565a95892533f33792094f23f28a71b880a60588ddf0c2'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 05 May 2023 00:03:43 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5627aec4010af613408c2ee78d5d32b9ecac22cb396d702906fb1160721f0011`  
		Last Modified: Wed, 03 May 2023 00:26:29 GMT  
		Size: 25.9 MB (25922039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9563e8b04d7a9913e093d138a52956da4d7e040127df5ba21381fc762e84eab`  
		Last Modified: Wed, 03 May 2023 17:07:53 GMT  
		Size: 3.1 MB (3131737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fda53726ff9354d56d43251fb0b7561866df3131f8f6c0fb4b83af4d8748c35`  
		Last Modified: Fri, 05 May 2023 00:07:09 GMT  
		Size: 200.6 MB (200608145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
