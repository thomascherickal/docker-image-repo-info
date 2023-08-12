## `openjdk:22-ea-jdk-slim`

```console
$ docker pull openjdk@sha256:93c3a8afa18a0fc5379c48c35cbd7f5b2c6db887eb828fbe96383bd7bcdbbc19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:22-ea-jdk-slim` - linux; amd64

```console
$ docker pull openjdk@sha256:bf30bdc3de3ec725194f4008d3c0670de9f2b9dbeba03d0ea9a29acde0a59325
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.3 MB (238294834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55199a9661c489e159a1e260cb4963b00fec63e64b47b8f8e98b4d9b951af28c`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:44 GMT
ADD file:209589a8bdb5a3788ee42ecdbccbbb561835dab96b0d8286bb5a2229d2f41be7 in / 
# Thu, 27 Jul 2023 23:24:45 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 04:08:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:08:55 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Fri, 28 Jul 2023 04:08:55 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 04:08:55 GMT
ENV LANG=C.UTF-8
# Sat, 12 Aug 2023 00:03:10 GMT
ENV JAVA_VERSION=22-ea+10
# Sat, 12 Aug 2023 00:03:23 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/10/GPL/openjdk-22-ea+10_linux-x64_bin.tar.gz'; 			downloadSha256='aa3e45c81e7269d389411b52c17721916d2acb7d3e7ab6367c62138063f5052b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/10/GPL/openjdk-22-ea+10_linux-aarch64_bin.tar.gz'; 			downloadSha256='e143f6323650bd4747e4304ef07ba80ade1510a71325bc36a7c4f51939cfe423'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Aug 2023 00:03:24 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:648e0aadf75ac2ef63c5390adc6dc14fde37a5ad88c2870ea604df0a9c0eb4e5`  
		Last Modified: Thu, 27 Jul 2023 23:29:26 GMT  
		Size: 29.1 MB (29124532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0240addcdc3176ff8e69de0608d99fa8e2e530a860fb05c187d7e292b3f119b8`  
		Last Modified: Fri, 28 Jul 2023 04:12:44 GMT  
		Size: 4.0 MB (4007998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3daacd6ce4276efafba045db83cab673e285016c18d1fd5291ceccfc333494d8`  
		Last Modified: Sat, 12 Aug 2023 00:08:38 GMT  
		Size: 205.2 MB (205162304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-ea-jdk-slim` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:bb716615e1ba293d86a6c6583ed9810a9dd3eb587c734e81dd4700f24ef7e17b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.5 MB (236525791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:138f797ba3b7ad7d0450c08540e12f72a986647d43c39df2d610681e060cba33`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:00 GMT
ADD file:1de2ba0dc88aa343332814e19adc6b850d08e62c31589fe902b8eb2cb465934e in / 
# Thu, 27 Jul 2023 23:43:00 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 10:40:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 10:40:44 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Fri, 28 Jul 2023 10:40:45 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 10:40:45 GMT
ENV LANG=C.UTF-8
# Fri, 04 Aug 2023 00:58:20 GMT
ENV JAVA_VERSION=22-ea+9
# Fri, 04 Aug 2023 00:58:33 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/9/GPL/openjdk-22-ea+9_linux-x64_bin.tar.gz'; 			downloadSha256='dd11f0f96ed6992b56452eee0683b50f1b550f74c31fb39e1eb1ff8a232caf68'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/9/GPL/openjdk-22-ea+9_linux-aarch64_bin.tar.gz'; 			downloadSha256='47ab1fb3cbe8174c21e10880e5de0c60d754cf5ba6d5cdfbe1a1d91b53b193bc'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 04 Aug 2023 00:58:35 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:90524f7dc01b4ce9b387992acc6cbdbcc2a9ee8c6addfd632429ca06ea18751e`  
		Last Modified: Thu, 27 Jul 2023 23:46:17 GMT  
		Size: 29.2 MB (29157226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4010ee17df6d7205932abb7128f52402f584cf7fb6dd4c00ed64745bd944dec`  
		Last Modified: Fri, 28 Jul 2023 10:44:45 GMT  
		Size: 3.8 MB (3817603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb53728594550d79ac46d182344a1ce9ab12c7e26c87a4eb9a3b2b52bafced0`  
		Last Modified: Fri, 04 Aug 2023 01:03:53 GMT  
		Size: 203.6 MB (203550962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
