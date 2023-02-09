## `openjdk:20-ea-34-slim`

```console
$ docker pull openjdk@sha256:ba6b53b50ebbe241782ada7de17e79e47ef8561c030ad1d231d6ce2a222f2d66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-34-slim` - linux; amd64

```console
$ docker pull openjdk@sha256:c112959e59fa4622890bdcc8d5e97da6c184f17d6aab3743d5510f0b4f241183
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231499214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c301c41bc3d72dee0e22ff99e07bf7e2006673c0929043b8f146c1c38dc75ec`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:47:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:48:58 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Thu, 09 Feb 2023 10:48:58 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 10:48:58 GMT
ENV LANG=C.UTF-8
# Thu, 09 Feb 2023 10:48:58 GMT
ENV JAVA_VERSION=20-ea+34
# Thu, 09 Feb 2023 10:49:12 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/34/GPL/openjdk-20-ea+34_linux-x64_bin.tar.gz'; 			downloadSha256='1c8e4809d7444903dfde02ef45821c1206a5d98c241c04280434ef9b5aca15ad'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/34/GPL/openjdk-20-ea+34_linux-aarch64_bin.tar.gz'; 			downloadSha256='6e43b2f39d2b6359755a6cd26c01057b1b6d53c84d944fc3396500b2f21a15be'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 09 Feb 2023 10:49:13 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10286f48c71be2a630e155ceb33e8e5132e861088b8d5db5ae0b2589912a958d`  
		Last Modified: Thu, 09 Feb 2023 10:54:07 GMT  
		Size: 1.6 MB (1582324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d12ea9914b91f82fa15f038a652a3af36250622e4cef118dd207428b5f31d7e`  
		Last Modified: Thu, 09 Feb 2023 10:56:47 GMT  
		Size: 198.5 MB (198505080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-34-slim` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:f09685bd514c47a73e67e8e1782295aad19208f086894ea32f20974787da6f9c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.6 MB (228636705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3d808464fd9a2a62f53bba3eea2e239c3d0ff7f8555e4dec2576a9a21b37e72`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:07:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:09:20 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Thu, 09 Feb 2023 10:09:20 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 10:09:21 GMT
ENV LANG=C.UTF-8
# Thu, 09 Feb 2023 10:09:21 GMT
ENV JAVA_VERSION=20-ea+34
# Thu, 09 Feb 2023 10:09:33 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/34/GPL/openjdk-20-ea+34_linux-x64_bin.tar.gz'; 			downloadSha256='1c8e4809d7444903dfde02ef45821c1206a5d98c241c04280434ef9b5aca15ad'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/34/GPL/openjdk-20-ea+34_linux-aarch64_bin.tar.gz'; 			downloadSha256='6e43b2f39d2b6359755a6cd26c01057b1b6d53c84d944fc3396500b2f21a15be'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 09 Feb 2023 10:09:35 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12ec23d1569af13aa4b739730163609a2c012fc5a8c00a55e2c980462802868`  
		Last Modified: Thu, 09 Feb 2023 10:14:41 GMT  
		Size: 1.6 MB (1566302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:682f8bba53ac51d3fdb1a5f667a0889acb22088150e939fd3dd8d8c6144cf7b6`  
		Last Modified: Thu, 09 Feb 2023 10:17:15 GMT  
		Size: 197.0 MB (197007894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
