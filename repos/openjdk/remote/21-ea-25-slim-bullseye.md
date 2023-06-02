## `openjdk:21-ea-25-slim-bullseye`

```console
$ docker pull openjdk@sha256:4f2ed99cbf2bb0951af5d15b10bfa23a815d7d163c8b6f713118dc702f2350c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-25-slim-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:12e08fe0b25430016ff35e58688052d4652338a69298bf7c254eb2705c457e8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.9 MB (236934903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6fed5a68ddf7fbb0da4987ae5df29fb830876059388fb53fe311c742d2b5684`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 07:48:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 07:48:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Tue, 23 May 2023 07:48:25 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 07:48:25 GMT
ENV LANG=C.UTF-8
# Thu, 01 Jun 2023 23:26:32 GMT
ENV JAVA_VERSION=21-ea+25
# Thu, 01 Jun 2023 23:26:47 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/25/GPL/openjdk-21-ea+25_linux-x64_bin.tar.gz'; 			downloadSha256='26d0ae26838de257ddb7dc06e11eee28038678adf85c494686c6592ff027a0b4'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/25/GPL/openjdk-21-ea+25_linux-aarch64_bin.tar.gz'; 			downloadSha256='44d36b86be342723ab29831812a4ccd8dfe9b964ef1b12b0fee053b76f97438e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 01 Jun 2023 23:26:47 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72173670925a3c8ba13478bbdf18b2e895b12815a5672faa2685b09d6ed1143d`  
		Last Modified: Tue, 23 May 2023 07:50:29 GMT  
		Size: 1.6 MB (1582459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101a678f1846f34aeb1f0051cbeecd72c2a9537d2a30e0e7a3e0ef19a671c48c`  
		Last Modified: Thu, 01 Jun 2023 23:29:44 GMT  
		Size: 203.9 MB (203948858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-25-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:36ebb1804b1fcf9874c784bec6323babb0b06bfb842d6360795ea20e356e5309
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.9 MB (233896159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da5cc03326f7e44a1154d306de2efd08f0a7e95c712326a948662587cc1027a5`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:45:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:45:24 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Tue, 23 May 2023 02:45:24 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:45:24 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 02:53:05 GMT
ENV JAVA_VERSION=21-ea+25
# Fri, 02 Jun 2023 02:53:16 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/25/GPL/openjdk-21-ea+25_linux-x64_bin.tar.gz'; 			downloadSha256='26d0ae26838de257ddb7dc06e11eee28038678adf85c494686c6592ff027a0b4'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/25/GPL/openjdk-21-ea+25_linux-aarch64_bin.tar.gz'; 			downloadSha256='44d36b86be342723ab29831812a4ccd8dfe9b964ef1b12b0fee053b76f97438e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 02 Jun 2023 02:53:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c2720cbf9c47906a0307f15640e572385cf4a861c09321177843a6399e647c`  
		Last Modified: Tue, 23 May 2023 02:47:18 GMT  
		Size: 1.6 MB (1566444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3adbc26df1aec4d7cdc74964719538170e97aab35b043bf9c4a6dcb96b64eb12`  
		Last Modified: Fri, 02 Jun 2023 02:56:03 GMT  
		Size: 202.3 MB (202276968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
