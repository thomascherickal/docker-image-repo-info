## `openjdk:22-jdk-slim-bookworm`

```console
$ docker pull openjdk@sha256:b49ee92c9dfb003032856cb1df6e028b5a08aab8018f3aab3b37d39686039fe7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:22-jdk-slim-bookworm` - linux; amd64

```console
$ docker pull openjdk@sha256:de5c34e0f657a801fb1d053a5c8909d01d170c25a7c1394480480d6d320e626e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.2 MB (238193758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a84206b9f3f2e53cd15ad5f41adc06ac8574985dbc0d0d35464f214055430b3f`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:52:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 01:52:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Tue, 04 Jul 2023 01:52:41 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 01:52:41 GMT
ENV LANG=C.UTF-8
# Fri, 14 Jul 2023 00:33:46 GMT
ENV JAVA_VERSION=22-ea+6
# Fri, 14 Jul 2023 00:34:00 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/6/GPL/openjdk-22-ea+6_linux-x64_bin.tar.gz'; 			downloadSha256='c0f9b77f4e63ceed956850811dd605aab708ed3251fdcb20bc4b34e46e98142d'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/6/GPL/openjdk-22-ea+6_linux-aarch64_bin.tar.gz'; 			downloadSha256='d42979ec7c71a40dcadb323c40a19068416045a32b0b8d950d7bfc96ae75197e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 14 Jul 2023 00:34:00 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:faef57eae888cbe4a5613eca6741b5e48d768b83f6088858aee9a5a2834f8151`  
		Last Modified: Tue, 04 Jul 2023 01:25:03 GMT  
		Size: 29.1 MB (29124829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbdb27ec859f702c52e07508d08c6644cdff01fc5028ae06b5440b5e48d2937`  
		Last Modified: Tue, 04 Jul 2023 01:57:48 GMT  
		Size: 4.0 MB (4008037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e5e3d3bfff8f8737a5bb643d039ac55d835ef5d5d39a1717d7ae8ccc483d55`  
		Last Modified: Fri, 14 Jul 2023 00:39:15 GMT  
		Size: 205.1 MB (205060892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-jdk-slim-bookworm` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:2fae3bab9bbd639a8b78f1408380eedcc3d5f686d843da29b1b2e298aa06693b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.4 MB (236357918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28222bbb9b0c90d1fec4383e11938e92a17cb912b11db28862c3a0865d0a979c`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 13:26:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 13:26:51 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Tue, 04 Jul 2023 13:26:51 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 13:26:51 GMT
ENV LANG=C.UTF-8
# Fri, 14 Jul 2023 00:45:14 GMT
ENV JAVA_VERSION=22-ea+6
# Fri, 14 Jul 2023 00:45:27 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/6/GPL/openjdk-22-ea+6_linux-x64_bin.tar.gz'; 			downloadSha256='c0f9b77f4e63ceed956850811dd605aab708ed3251fdcb20bc4b34e46e98142d'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/6/GPL/openjdk-22-ea+6_linux-aarch64_bin.tar.gz'; 			downloadSha256='d42979ec7c71a40dcadb323c40a19068416045a32b0b8d950d7bfc96ae75197e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 14 Jul 2023 00:45:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160b152e2d87fa10c40e3d8ffcd0828fc336c0c9bfed0a0f293fedd4e70afdd0`  
		Last Modified: Tue, 04 Jul 2023 13:30:53 GMT  
		Size: 3.8 MB (3817545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b1795cc7b350c14da5eb74a2f42e2e8f815f898d0faf3406517d490b379c6c`  
		Last Modified: Fri, 14 Jul 2023 00:50:25 GMT  
		Size: 203.4 MB (203387915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
