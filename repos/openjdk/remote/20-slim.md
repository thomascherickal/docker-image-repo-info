## `openjdk:20-slim`

```console
$ docker pull openjdk@sha256:6501250d25840406d6ccc799c77bc61361c3ac9940f4054f001a4471d2cd31c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-slim` - linux; amd64

```console
$ docker pull openjdk@sha256:08bbf7b60756102c56db922bfec7ce48bc1e95c93a4d6ae2c752892883c8ec8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230528919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f421b50c805c0ebaaec1aaeef7c2544121cce87d5c7d8004aa4671408d4e5fd`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:29:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:29:36 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 23 Aug 2022 04:29:36 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 04:29:36 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 04:29:36 GMT
ENV JAVA_VERSION=20-ea+11
# Tue, 23 Aug 2022 04:29:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/11/GPL/openjdk-20-ea+11_linux-x64_bin.tar.gz'; 			downloadSha256='9a0afe9f1c3ef50968060fe8d70d7b27d93b5515479846193de809127f0d427f'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/11/GPL/openjdk-20-ea+11_linux-aarch64_bin.tar.gz'; 			downloadSha256='d7e80f5000f66440c34073bdb0e443b941ef11209ca30f0e698f07a3fce08118'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 23 Aug 2022 04:29:50 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b1c853f5d1e2529f16cddde75874e53c112a9bee4b0954afb1bb8a2a29044b`  
		Last Modified: Tue, 23 Aug 2022 04:36:30 GMT  
		Size: 1.6 MB (1582289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48a8a35f532c2f63b4b4b72e896cab1acca4532d337a736ea41752afadbb63b`  
		Last Modified: Tue, 23 Aug 2022 04:36:44 GMT  
		Size: 197.6 MB (197565145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-slim` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:359283c41fec4d174940d0a0d8abfb3f9b1a3d87aea4acc0bee5508fe1bfa386
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.3 MB (227308668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef2491df07670ceb7ea323ee107aca70b39e7b3059066e11c60db8b1c5a3cc99`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 05:16:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 05:16:05 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 23 Aug 2022 05:16:06 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 05:16:07 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 05:16:08 GMT
ENV JAVA_VERSION=20-ea+11
# Tue, 23 Aug 2022 05:16:45 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/11/GPL/openjdk-20-ea+11_linux-x64_bin.tar.gz'; 			downloadSha256='9a0afe9f1c3ef50968060fe8d70d7b27d93b5515479846193de809127f0d427f'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/11/GPL/openjdk-20-ea+11_linux-aarch64_bin.tar.gz'; 			downloadSha256='d7e80f5000f66440c34073bdb0e443b941ef11209ca30f0e698f07a3fce08118'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 23 Aug 2022 05:16:46 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a336c8a0edb35428a570e25d2023ce4e03a37c1c31638892cc2c38fca7cf3c91`  
		Last Modified: Tue, 23 Aug 2022 05:27:39 GMT  
		Size: 1.4 MB (1361214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905b5ced44b85f9224f61ba153e7aab5d934ba953e8765099b58b541b7694940`  
		Last Modified: Tue, 23 Aug 2022 05:27:56 GMT  
		Size: 195.9 MB (195883666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
