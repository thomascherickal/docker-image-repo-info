## `openjdk:20-ea-slim`

```console
$ docker pull openjdk@sha256:7c5c56740fdd0182f5625fee4491c74632936ea4bfefa62d5b91a4f0a94f1aca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-slim` - linux; amd64

```console
$ docker pull openjdk@sha256:1d9b021555c37daa3d5985e693c67bb309b6b274772bbd81a520175f7def5761
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231484362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:462fe9e55b6915f2208ffcb65165903da6b95f8d33e4450111888cdc36716944`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 07:04:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 07:05:38 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Wed, 11 Jan 2023 07:05:38 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 07:05:38 GMT
ENV LANG=C.UTF-8
# Thu, 02 Feb 2023 23:34:05 GMT
ENV JAVA_VERSION=20-ea+34
# Thu, 02 Feb 2023 23:34:18 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/34/GPL/openjdk-20-ea+34_linux-x64_bin.tar.gz'; 			downloadSha256='1c8e4809d7444903dfde02ef45821c1206a5d98c241c04280434ef9b5aca15ad'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/34/GPL/openjdk-20-ea+34_linux-aarch64_bin.tar.gz'; 			downloadSha256='6e43b2f39d2b6359755a6cd26c01057b1b6d53c84d944fc3396500b2f21a15be'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 02 Feb 2023 23:34:19 GMT
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
	-	`sha256:fba7638aa8b21ba3cce7f66b035a44f9d3125197d7c29d41b0d4ee431ab9b54a`  
		Last Modified: Thu, 02 Feb 2023 23:43:36 GMT  
		Size: 198.5 MB (198505100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-slim` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:c6d715a700f3605cf95ca222cb06e08ba6b5fd97d3480ac971975feb428f4ff6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.6 MB (228618988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d872d553ab5693cf21cbc9a253d6c8bc1c0a87e0806846a71b9904abdeb5997`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 09:13:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 09:14:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Sat, 04 Feb 2023 09:14:45 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 09:14:45 GMT
ENV LANG=C.UTF-8
# Sat, 04 Feb 2023 09:14:45 GMT
ENV JAVA_VERSION=20-ea+34
# Sat, 04 Feb 2023 09:14:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/34/GPL/openjdk-20-ea+34_linux-x64_bin.tar.gz'; 			downloadSha256='1c8e4809d7444903dfde02ef45821c1206a5d98c241c04280434ef9b5aca15ad'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/34/GPL/openjdk-20-ea+34_linux-aarch64_bin.tar.gz'; 			downloadSha256='6e43b2f39d2b6359755a6cd26c01057b1b6d53c84d944fc3396500b2f21a15be'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 04 Feb 2023 09:15:00 GMT
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
	-	`sha256:ec87d2314586b0ac150a235bc46dbcb5f9d9e8b78905aad443cafeb46cadee50`  
		Last Modified: Sat, 04 Feb 2023 09:22:56 GMT  
		Size: 197.0 MB (197007964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
