## `openjdk:18-ea-5-jdk-slim`

```console
$ docker pull openjdk@sha256:2ec6912a8c18f67ea9045d8e48d25c106a332b46274c50eb215d651d1ec2c537
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-ea-5-jdk-slim` - linux; amd64

```console
$ docker pull openjdk@sha256:bdb5ec1aa321c9726d28c4cb458f47ae8f441d712d9cde3e7c06a63b24370ab6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.7 MB (218665668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c461e50442baa7878d446077bf13cb41f7487c04555623999932868f43229f7`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 08:00:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 08:00:09 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Wed, 23 Jun 2021 08:00:10 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 08:00:10 GMT
ENV LANG=C.UTF-8
# Mon, 12 Jul 2021 23:33:52 GMT
ENV JAVA_VERSION=18-ea+5
# Mon, 12 Jul 2021 23:34:06 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/5/GPL/openjdk-18-ea+5_linux-x64_bin.tar.gz'; 			downloadSha256='a50d2f7309f987ee33cfdfdfbd22c18ea8e6dc8a3bb21b582cd67fb97c906a82'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/5/GPL/openjdk-18-ea+5_linux-aarch64_bin.tar.gz'; 			downloadSha256='28e3b50e98e75ae64d200ddcf87ba0664229e0659ccba3cd8ee2e25cbe6de24f'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 12 Jul 2021 23:34:06 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee45ae9730633057cf9bd12924f9a1bf2b590631d3d085b14c96f4466557794`  
		Last Modified: Wed, 23 Jun 2021 08:12:04 GMT  
		Size: 3.3 MB (3268886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0ff24080a4bade61e69e9d3e4dccdc7e5b60f1ad91f20c52ee28bb56653baa`  
		Last Modified: Mon, 12 Jul 2021 23:43:52 GMT  
		Size: 188.3 MB (188250931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-5-jdk-slim` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:c39e40a5e7c9157934a2aa514222571818fd094001d1efb363ed2dd45402522d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.0 MB (215985858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c766fd8023a2964f5b392db00d3f593756b28bac50fffd56206ec483447561f6`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 04:56:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 04:56:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Wed, 23 Jun 2021 04:56:08 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 04:56:08 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jul 2021 00:13:56 GMT
ENV JAVA_VERSION=18-ea+5
# Tue, 13 Jul 2021 00:14:09 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/5/GPL/openjdk-18-ea+5_linux-x64_bin.tar.gz'; 			downloadSha256='a50d2f7309f987ee33cfdfdfbd22c18ea8e6dc8a3bb21b582cd67fb97c906a82'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/5/GPL/openjdk-18-ea+5_linux-aarch64_bin.tar.gz'; 			downloadSha256='28e3b50e98e75ae64d200ddcf87ba0664229e0659ccba3cd8ee2e25cbe6de24f'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 13 Jul 2021 00:14:10 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb5c013aa648ff2c30dafc35db9efb2faa7f9fa6f1c98a2f31c1b5fee0334dc`  
		Last Modified: Wed, 23 Jun 2021 05:11:10 GMT  
		Size: 3.1 MB (3118894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dddafc95c3580a23f1296a6be3bfec53fac8699eaed91182bbc14414f77b4414`  
		Last Modified: Tue, 13 Jul 2021 00:29:20 GMT  
		Size: 187.0 MB (186951971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
