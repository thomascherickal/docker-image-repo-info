## `openjdk:19-ea-34-jdk-slim`

```console
$ docker pull openjdk@sha256:2ec3f7ed85de11754d0ef375efc426041ba7dae2a8e65ff1fbb91c7c6fff9738
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-ea-34-jdk-slim` - linux; amd64

```console
$ docker pull openjdk@sha256:975427385339213ab71e872ec025168b3c1c3f48c7d7cb2056f26f2c45b21b4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.5 MB (229496992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e46a2581479efafdf97653188a95613255d2604a8f33da8d6e6902828f662627`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:04 GMT
ADD file:0eae0dca665c7044bf242cb1fc92cb8ea744f5af2dd376a558c90bc47349aefe in / 
# Tue, 02 Aug 2022 01:20:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:48:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:49:32 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Tue, 02 Aug 2022 05:49:32 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 05:49:32 GMT
ENV LANG=C.UTF-8
# Mon, 08 Aug 2022 22:53:52 GMT
ENV JAVA_VERSION=19-ea+34
# Mon, 08 Aug 2022 22:54:06 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_linux-x64_bin.tar.gz'; 			downloadSha256='719889f7aaf988e7ec5c6edd0c3bd03342294f329a36dd6591af2e64f6aefae7'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_linux-aarch64_bin.tar.gz'; 			downloadSha256='8d5d5327b1a7d35ae2c16ba69701cb58cb5b5df58f5ace295c08fe77d96a688b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 08 Aug 2022 22:54:07 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1efc276f4ff952c055dea726cfc96ec6a4fdb8b62d9eed816bd2b788f2860ad7`  
		Last Modified: Tue, 02 Aug 2022 01:24:13 GMT  
		Size: 31.4 MB (31366757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f2f93da48276873890ac821b3c991d53a7e864791aaf82c39b7863c908b93b`  
		Last Modified: Tue, 02 Aug 2022 06:01:18 GMT  
		Size: 1.6 MB (1582262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31667857ff8d98329e7ef3658c28a077f93154190e090a4e5c91d3c33fbd7dc8`  
		Last Modified: Mon, 08 Aug 2022 23:06:04 GMT  
		Size: 196.5 MB (196547973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-ea-34-jdk-slim` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:865e6980b8faca37dbe2b82ae37048f89bd0f9ceb2e91536a3b3122c7eac65e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226810377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7120cd808cdd48c9e3bdeda3361f965d8e75857910f8410a4f2bd6b88399a5db`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:41:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:44:03 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Tue, 02 Aug 2022 04:44:04 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 04:44:05 GMT
ENV LANG=C.UTF-8
# Mon, 08 Aug 2022 23:33:34 GMT
ENV JAVA_VERSION=19-ea+34
# Mon, 08 Aug 2022 23:33:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_linux-x64_bin.tar.gz'; 			downloadSha256='719889f7aaf988e7ec5c6edd0c3bd03342294f329a36dd6591af2e64f6aefae7'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_linux-aarch64_bin.tar.gz'; 			downloadSha256='8d5d5327b1a7d35ae2c16ba69701cb58cb5b5df58f5ace295c08fe77d96a688b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 08 Aug 2022 23:33:59 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4015b6e8cc8db11af172df5c0369552bc2a74cd69094b0756d21fc6b0b2a5393`  
		Last Modified: Tue, 02 Aug 2022 05:03:25 GMT  
		Size: 1.6 MB (1565954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fd63e1e2c90e1731c4cb7377b6011bed7e6e7c524fb222794a1889a4b8c7b4`  
		Last Modified: Mon, 08 Aug 2022 23:52:42 GMT  
		Size: 195.2 MB (195190119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
