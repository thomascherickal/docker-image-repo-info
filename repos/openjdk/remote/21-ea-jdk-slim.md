## `openjdk:21-ea-jdk-slim`

```console
$ docker pull openjdk@sha256:36253bbcdd24d247eadcd88ec46d2046651badfa8b35de51f81e9ba9af51fb63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-jdk-slim` - linux; amd64

```console
$ docker pull openjdk@sha256:78adb16c919db9d105caafc6be14d07568de6f1fd38db5e4dd102934945c6352
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.6 MB (232600024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc113da9e1efcc9c5323ebcbb895dc373c5d85b2787d05c894f6ff64fbf48e37`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 07:04:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 07:04:10 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Wed, 11 Jan 2023 07:04:10 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 07:04:10 GMT
ENV LANG=C.UTF-8
# Thu, 02 Feb 2023 23:32:17 GMT
ENV JAVA_VERSION=21-ea+8
# Thu, 02 Feb 2023 23:32:31 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/8/GPL/openjdk-21-ea+8_linux-x64_bin.tar.gz'; 			downloadSha256='ce77e229b2dc811e1231ab1197f851d3234e56cb9e9a26e9f1d7c0294eb09af8'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/8/GPL/openjdk-21-ea+8_linux-aarch64_bin.tar.gz'; 			downloadSha256='c52c76023ce2b7202744161d92772f5bc21c6ada643b926c92d5a56b0d1c4664'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 02 Feb 2023 23:32:32 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec49d0093a3b27f87b047abc2b89aef94d6db65ce71e6660520e4b01f9ceae25`  
		Last Modified: Wed, 11 Jan 2023 07:11:03 GMT  
		Size: 1.6 MB (1582290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55de0bb37e005d63e5972e4d3fcad13e3a908f93b7ea2a30d3e810c056afb8f6`  
		Last Modified: Thu, 02 Feb 2023 23:39:56 GMT  
		Size: 199.6 MB (199620762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-jdk-slim` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:4f3879ac2f454849ba1415c68d76e832f717d45891d099692fae82743be3fa68
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.7 MB (229694930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8732a7d164b80b52a2424674de1ee5e797c72b996629e116ba3cf2f4104ee32e`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 09:13:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 09:13:05 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Sat, 04 Feb 2023 09:13:05 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 09:13:06 GMT
ENV LANG=C.UTF-8
# Sat, 04 Feb 2023 09:13:06 GMT
ENV JAVA_VERSION=21-ea+8
# Sat, 04 Feb 2023 09:13:17 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/8/GPL/openjdk-21-ea+8_linux-x64_bin.tar.gz'; 			downloadSha256='ce77e229b2dc811e1231ab1197f851d3234e56cb9e9a26e9f1d7c0294eb09af8'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/8/GPL/openjdk-21-ea+8_linux-aarch64_bin.tar.gz'; 			downloadSha256='c52c76023ce2b7202744161d92772f5bc21c6ada643b926c92d5a56b0d1c4664'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 04 Feb 2023 09:13:19 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001ee2e58ebf78c483b4dba276ed5ef2fd462c4471bf7dfef4daffe6b2595c09`  
		Last Modified: Sat, 04 Feb 2023 09:20:28 GMT  
		Size: 1.6 MB (1566232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507541258b3a7338138b6d9f2aadce6408692513e60d7e964d794fbccd7db923`  
		Last Modified: Sat, 04 Feb 2023 09:20:40 GMT  
		Size: 198.1 MB (198083906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
