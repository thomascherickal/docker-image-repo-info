## `openjdk:19-ea-slim-buster`

```console
$ docker pull openjdk@sha256:4a817bf1e687567ea507c395d8fb9a588783ef1c0eec3a9dfed94c152a876ab0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-ea-slim-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:2a2262fb1db0bd236ac7fe51792116069ee0e7b87e7d9517247a735146218461
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.0 MB (226959648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7891ae9884f563f2a380f2ebf9d311e593f58b9487701bb4b6e6548a7e5fa0fc`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:24 GMT
ADD file:81dbfe4f9df4d280f7580380c0c5c93ba71fedba17b3072d2b7b4bce127f88a9 in / 
# Tue, 02 Aug 2022 01:20:24 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:48:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:50:04 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Tue, 02 Aug 2022 05:50:04 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 05:50:04 GMT
ENV LANG=C.UTF-8
# Tue, 02 Aug 2022 05:50:04 GMT
ENV JAVA_VERSION=19-ea+33
# Tue, 02 Aug 2022 05:50:18 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/33/GPL/openjdk-19-ea+33_linux-x64_bin.tar.gz'; 			downloadSha256='31aa1cf0a266dfc90d9e85d688379a2b2b9b1888bb7df326a4434dc92fdc105f'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/33/GPL/openjdk-19-ea+33_linux-aarch64_bin.tar.gz'; 			downloadSha256='8e758bdc4cd496f29c85a53ce1eb155b7ee8f945c11517cc4a766492349c52e2'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 02 Aug 2022 05:50:19 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:751ef25978b2971e15496369695ba51ed5b1b9aaca7e37b18a173d754d1ca820`  
		Last Modified: Tue, 02 Aug 2022 01:25:00 GMT  
		Size: 27.1 MB (27140083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140e22108c7d39a72fc1f5f3ba4ffdd55836614e9c53175f5d43ada8b6bbaacc`  
		Last Modified: Tue, 02 Aug 2022 06:02:41 GMT  
		Size: 3.3 MB (3273367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7048431f0bfdb4473842583fa6800d4a0baba68b994325b2d0e2c622f20af1a`  
		Last Modified: Tue, 02 Aug 2022 06:05:39 GMT  
		Size: 196.5 MB (196546198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-ea-slim-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:53aef53aaccc736fb1bbbee9f5c3b019ca2f0cc37dedcf23c29998a077a3c0db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.2 MB (224227792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:135f3b2cc0a1bfb65b5fc708827020d29ac3efd8bbccfa9b2aa1f38ca581fce8`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:03 GMT
ADD file:d973e057fdca9166fb9f39e73d7d5d4ca8ac2af6a55813580bf14a13cef4c159 in / 
# Tue, 02 Aug 2022 00:41:04 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:42:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:44:53 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Tue, 02 Aug 2022 04:44:54 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 04:44:55 GMT
ENV LANG=C.UTF-8
# Tue, 02 Aug 2022 04:44:56 GMT
ENV JAVA_VERSION=19-ea+33
# Tue, 02 Aug 2022 04:45:10 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/33/GPL/openjdk-19-ea+33_linux-x64_bin.tar.gz'; 			downloadSha256='31aa1cf0a266dfc90d9e85d688379a2b2b9b1888bb7df326a4434dc92fdc105f'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/33/GPL/openjdk-19-ea+33_linux-aarch64_bin.tar.gz'; 			downloadSha256='8e758bdc4cd496f29c85a53ce1eb155b7ee8f945c11517cc4a766492349c52e2'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 02 Aug 2022 04:45:11 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6d588874b4737b02fc84169cf7d3d1d70f20c7f5dbd1ddfe27de4aff25e23314`  
		Last Modified: Tue, 02 Aug 2022 00:46:56 GMT  
		Size: 25.9 MB (25914363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c6f3c25c4deaf78673b1fd4ca615f7a3d33a177d1d101f83a1700e34bc27f1`  
		Last Modified: Tue, 02 Aug 2022 05:05:08 GMT  
		Size: 3.1 MB (3126019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6362ff3f7a5eef178fb9010aa7295dd44eb81ce5cbaa590ae933b1049e1f8939`  
		Last Modified: Tue, 02 Aug 2022 05:08:42 GMT  
		Size: 195.2 MB (195187410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
