## `openjdk:22-jdk-slim`

```console
$ docker pull openjdk@sha256:d2c483ae602cceee8b58c923b7191b6eb04a83e560337abe79e61754f6cb7aad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:22-jdk-slim` - linux; amd64

```console
$ docker pull openjdk@sha256:f28f4255b082053bf5a3c922a8fd8c466d0ae8bd4f2a0ed93ed3e528f2773bd8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.1 MB (239055634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1338ca9bd32e3eddac89630fd83ac7698cb386ae36cf20b8331e1c11940c1aa3`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 02:48:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 02:48:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Thu, 12 Oct 2023 02:48:48 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 02:48:48 GMT
ENV LANG=C.UTF-8
# Sat, 28 Oct 2023 00:37:43 GMT
ENV JAVA_VERSION=22-ea+21
# Sat, 28 Oct 2023 00:37:57 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/21/GPL/openjdk-22-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='cefe6f9697801dd2a7abebdbd5b7bd36ad489794589e838562da46bde434ae5e'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/21/GPL/openjdk-22-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='b77e7f170973c91690aa64a028f2e991828fde5092eabc29b602e26824216797'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 28 Oct 2023 00:37:58 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6b4e2c8e80e7a261b67542c6655d67269b5dad6ffbef15b5e49e5589289b82`  
		Last Modified: Thu, 12 Oct 2023 02:50:10 GMT  
		Size: 4.0 MB (4017876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618caab73a45ea5cc9841438a7f6723b47c2f7d6a193bfcd79edd154275c5188`  
		Last Modified: Sat, 28 Oct 2023 00:41:07 GMT  
		Size: 205.9 MB (205887884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-jdk-slim` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:0f4ab4f1fc59c7aa163fa9c1c7843639f5f16e9a6e62d4ad1c7803a9c13db98a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.1 MB (237102364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22fb56222176fae8205fecf401fdcf5abb7ad58c15f265d3a8da4ccbf89d5c8e`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:51 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Wed, 11 Oct 2023 18:24:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:50:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:50:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Wed, 11 Oct 2023 22:50:09 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 22:50:09 GMT
ENV LANG=C.UTF-8
# Sat, 28 Oct 2023 00:37:42 GMT
ENV JAVA_VERSION=22-ea+21
# Sat, 28 Oct 2023 00:37:55 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/21/GPL/openjdk-22-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='cefe6f9697801dd2a7abebdbd5b7bd36ad489794589e838562da46bde434ae5e'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/21/GPL/openjdk-22-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='b77e7f170973c91690aa64a028f2e991828fde5092eabc29b602e26824216797'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 28 Oct 2023 00:37:57 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1addc1e1c2c75c85302c72986bed4391fe81acea06679d6de790ea18001eb6`  
		Last Modified: Wed, 11 Oct 2023 22:52:19 GMT  
		Size: 3.8 MB (3825526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c4256e814b2ca4c3814d699c6a5eb1655fde8d7ba82f39a009c3006b87d8a9`  
		Last Modified: Sat, 28 Oct 2023 00:41:03 GMT  
		Size: 204.1 MB (204097554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
