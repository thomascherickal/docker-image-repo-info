## `openjdk:20-ea-2-slim`

```console
$ docker pull openjdk@sha256:66444510e408af549327be5de824d9eb1707f2067e087fd19066e0cbaaf5870f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-2-slim` - linux; amd64

```console
$ docker pull openjdk@sha256:b2f73fbdd3fe96c5a07959541cd06d82c133ac8fecc6f467368d125b22d5a416
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230491852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cf02c98c9150d3efc6a9818955167486bbaa74d6bc4b404c6099c10ee524c3d`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:16:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Jun 2022 01:22:35 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Thu, 16 Jun 2022 01:22:35 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Jun 2022 01:22:35 GMT
ENV LANG=C.UTF-8
# Wed, 22 Jun 2022 01:20:44 GMT
ENV JAVA_VERSION=20-ea+2
# Wed, 22 Jun 2022 01:20:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/2/GPL/openjdk-20-ea+2_linux-x64_bin.tar.gz'; 			downloadSha256='21ff68a0fba20bd62c33f66b6215e4dbb6a4ccc40ee4c63aefd5a69ded443812'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/2/GPL/openjdk-20-ea+2_linux-aarch64_bin.tar.gz'; 			downloadSha256='23ec06e04606ac8ccd9f304bc06527f78c6a196b796b8b7581de2153a3097bff'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 22 Jun 2022 01:20:58 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b062e78fd7c8f9370711c8b47595bc59fea38f7e04e22d887fbd3256f2324c`  
		Last Modified: Sat, 28 May 2022 02:27:46 GMT  
		Size: 1.6 MB (1582290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46096e0b37819f74779afed974042a5275a0c4f7e0a97d1bf602a3f56cb36f9`  
		Last Modified: Wed, 22 Jun 2022 01:31:33 GMT  
		Size: 197.5 MB (197530286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-2-slim` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:27604414469575c61b678f1959e493b6238cf5bae46b41b50d91ce2cfa5df4f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.6 MB (227578964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a9d06622ab49cd95aecbfd6e90a84240f8269bc6720202a846a7b67883ecedf`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:37:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Jun 2022 00:50:18 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Thu, 16 Jun 2022 00:50:19 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Jun 2022 00:50:20 GMT
ENV LANG=C.UTF-8
# Wed, 22 Jun 2022 02:14:04 GMT
ENV JAVA_VERSION=20-ea+2
# Wed, 22 Jun 2022 02:14:17 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/2/GPL/openjdk-20-ea+2_linux-x64_bin.tar.gz'; 			downloadSha256='21ff68a0fba20bd62c33f66b6215e4dbb6a4ccc40ee4c63aefd5a69ded443812'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/2/GPL/openjdk-20-ea+2_linux-aarch64_bin.tar.gz'; 			downloadSha256='23ec06e04606ac8ccd9f304bc06527f78c6a196b796b8b7581de2153a3097bff'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 22 Jun 2022 02:14:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c8727eedfb1755681add8fcb3c2c35d3b41f8231849edcec84588c6404f3b3`  
		Last Modified: Sat, 28 May 2022 01:54:41 GMT  
		Size: 1.4 MB (1361240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d100fd387ab07d3803a54ec0bec788f48cb30a3f99814c37feaa45124d700f97`  
		Last Modified: Wed, 22 Jun 2022 02:31:49 GMT  
		Size: 196.2 MB (196151996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
