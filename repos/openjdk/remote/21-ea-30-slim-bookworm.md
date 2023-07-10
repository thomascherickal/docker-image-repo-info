## `openjdk:21-ea-30-slim-bookworm`

```console
$ docker pull openjdk@sha256:9559e150c4ad010fa746497193a0092453514229cca09acf38db22abdc6cfa75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-30-slim-bookworm` - linux; amd64

```console
$ docker pull openjdk@sha256:b924e02204f406ac7a717a517f80325528ecf8a95042a098c0b64f1b163f35df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.4 MB (237371016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8080c1c3fe8006463c99648bd979c0edb24dd546ea3bcf34ad35a3a1e5e12bc`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:52:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 01:54:22 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Tue, 04 Jul 2023 01:54:22 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 01:54:22 GMT
ENV LANG=C.UTF-8
# Mon, 10 Jul 2023 20:48:59 GMT
ENV JAVA_VERSION=21-ea+30
# Mon, 10 Jul 2023 20:49:12 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/30/GPL/openjdk-21-ea+30_linux-x64_bin.tar.gz'; 			downloadSha256='c35a1f2906d502e9f75a975165f4c86e29167ca8cc2d9d25b5351b46d90d4ab7'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/30/GPL/openjdk-21-ea+30_linux-aarch64_bin.tar.gz'; 			downloadSha256='ae690af5ffa639feba3bc04fc804480cdbc40b4099890c9d28dceac8f58f0426'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 10 Jul 2023 20:49:13 GMT
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
	-	`sha256:e72cfe534dda11eaa6824f3ac0d0bc2f5fb80ff9fae5c16defb1e38078268551`  
		Last Modified: Mon, 10 Jul 2023 20:56:21 GMT  
		Size: 204.2 MB (204238150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-30-slim-bookworm` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:c846ea39bd2bc8071c3f7c7c327dde7a360c4a937d549a57395a669eba3a23ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.6 MB (235553939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d498ca5853245d4eeebb8ea4c6f8a4459339c8d95c3954abfcbc2e2238382f1a`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 13:26:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 13:28:34 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Tue, 04 Jul 2023 13:28:34 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 13:28:34 GMT
ENV LANG=C.UTF-8
# Mon, 10 Jul 2023 21:35:25 GMT
ENV JAVA_VERSION=21-ea+30
# Mon, 10 Jul 2023 21:35:37 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/30/GPL/openjdk-21-ea+30_linux-x64_bin.tar.gz'; 			downloadSha256='c35a1f2906d502e9f75a975165f4c86e29167ca8cc2d9d25b5351b46d90d4ab7'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/30/GPL/openjdk-21-ea+30_linux-aarch64_bin.tar.gz'; 			downloadSha256='ae690af5ffa639feba3bc04fc804480cdbc40b4099890c9d28dceac8f58f0426'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 10 Jul 2023 21:35:39 GMT
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
	-	`sha256:e07b8f4b58b8c2b78b9a0f284412a765e956431e845b635d12af1b156b012450`  
		Last Modified: Mon, 10 Jul 2023 21:42:02 GMT  
		Size: 202.6 MB (202583936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
