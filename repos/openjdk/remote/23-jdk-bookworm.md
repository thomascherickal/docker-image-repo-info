## `openjdk:23-jdk-bookworm`

```console
$ docker pull openjdk@sha256:5f69a7020f66168d55767c3e60217eb9f22575da135a5711e81cc0afb4c39272
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `openjdk:23-jdk-bookworm` - linux; amd64

```console
$ docker pull openjdk@sha256:d0da87842831bff1a1be25d90853dda7edd29ce726b6131208650a40787b3216
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.6 MB (357627326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c3d7ad5a5d31048298cf76e7da5f50aaedb4dc9611eec77ae4fb64f149c32ae`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:24 GMT
ADD file:39d17d28c5de0bd629e5b7c8190228e5a445d61d668e189b7523e90e68f78244 in / 
# Tue, 21 Nov 2023 05:21:25 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:52:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:53:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 18:45:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 09 Dec 2023 18:45:21 GMT
ENV JAVA_HOME=/usr/local/openjdk-23
# Sat, 09 Dec 2023 18:45:21 GMT
ENV PATH=/usr/local/openjdk-23/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 09 Dec 2023 18:45:21 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 18:45:21 GMT
ENV JAVA_VERSION=23-ea+1
# Sat, 09 Dec 2023 18:45:21 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/1/GPL/openjdk-23-ea+1_linux-x64_bin.tar.gz'; 			downloadSha256='740a84253d35402b9213bf187ee4f058817c614f8cc47cb3414e02760f05099f'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/1/GPL/openjdk-23-ea+1_linux-aarch64_bin.tar.gz'; 			downloadSha256='74fe7c8e67c5b80f868ec20daecb112fc090fb91c58bf4ce5297cf77c9935fa5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Sat, 09 Dec 2023 18:45:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:90e5e7d8b87a34877f61c2b86d053db1c4f440b9054cf49573e3be5d6a674a47`  
		Last Modified: Tue, 21 Nov 2023 05:25:34 GMT  
		Size: 49.6 MB (49582225 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:27e1a8ca91d35598fbae8dee7f1c211f0f93cec529f6804a60e9301c53a604d0`  
		Last Modified: Tue, 21 Nov 2023 10:01:22 GMT  
		Size: 24.0 MB (24049172 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d3a767d1d12e57724b9f254794e359f3b04d4d5ad966006e5b5cda78cc382762`  
		Last Modified: Tue, 21 Nov 2023 10:01:41 GMT  
		Size: 64.1 MB (64130771 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c1a93371d85c6e94598965f26e9284a3e428bdf3c6c77fff296347ed379fbe40`  
		Last Modified: Fri, 15 Dec 2023 22:05:51 GMT  
		Size: 16.9 MB (16949287 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:27d53b4de97cc9e8f78da55f4eba9dd9f441c8756785782033d8fea7cc2ad155`  
		Last Modified: Fri, 15 Dec 2023 22:05:55 GMT  
		Size: 202.9 MB (202915871 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:23-jdk-bookworm` - unknown; unknown

```console
$ docker pull openjdk@sha256:8ad778a86eeaf2679addc9dfc9d8a3e6dd82a4949f288b1067c6f7140a731ca5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7135093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4c7b209f3502b3df188cd454355c154ed2d3b2d5c790d1040da3a72aabec305`

```dockerfile
```

-	Layers:
	-	`sha256:ac3a6d238327795a4f0a96d1e87b26717ceaadb3f2c2a6210ab51f1b0cd02fbd`  
		Last Modified: Fri, 15 Dec 2023 22:05:50 GMT  
		Size: 7.1 MB (7116204 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:19c6cbb248ed53298c2317d7e85852a95c575dd82df46ce72a0fa304904e6cd2`  
		Last Modified: Fri, 15 Dec 2023 22:05:49 GMT  
		Size: 18.9 KB (18889 bytes)  
		MIME: application/vnd.in-toto+json

### `openjdk:23-jdk-bookworm` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:e80ddf98b530e0253c4a8d89bb375e4756b41bbe86e3666dfb27de0fe31e2f8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.9 MB (355889489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30a2f5e28ffeaf131819a4b394481ef78b0f46220a89f2d3ee90bc2321fd6003`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 21 Nov 2023 06:26:54 GMT
ADD file:6550a7c17e64067114283d098e85f9a74d4707f2879b53c2e4cae99f329c9025 in / 
# Tue, 21 Nov 2023 06:26:55 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:57:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:57:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 18:45:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 09 Dec 2023 18:45:21 GMT
ENV JAVA_HOME=/usr/local/openjdk-23
# Sat, 09 Dec 2023 18:45:21 GMT
ENV PATH=/usr/local/openjdk-23/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 09 Dec 2023 18:45:21 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 18:45:21 GMT
ENV JAVA_VERSION=23-ea+1
# Sat, 09 Dec 2023 18:45:21 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/1/GPL/openjdk-23-ea+1_linux-x64_bin.tar.gz'; 			downloadSha256='740a84253d35402b9213bf187ee4f058817c614f8cc47cb3414e02760f05099f'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/1/GPL/openjdk-23-ea+1_linux-aarch64_bin.tar.gz'; 			downloadSha256='74fe7c8e67c5b80f868ec20daecb112fc090fb91c58bf4ce5297cf77c9935fa5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Sat, 09 Dec 2023 18:45:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:df2021ddb7d686bdbb125598b2a6163d63035f080356b3014595f354ea0b40d6`  
		Last Modified: Tue, 21 Nov 2023 06:30:07 GMT  
		Size: 49.6 MB (49612650 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8d647f1dd7e741209a8a75083ccc889e39cb3e94c17f45441eae96e1a679d971`  
		Last Modified: Tue, 21 Nov 2023 08:06:01 GMT  
		Size: 23.6 MB (23584876 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5cdd9a70365f741a6b9f7a4e32cdb7d4aa29ac73da0b78ca0a83e937f285fdd5`  
		Last Modified: Tue, 21 Nov 2023 08:06:19 GMT  
		Size: 64.0 MB (63994275 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7cc6ea26c20f1b5bc02a72a1735a76f0ae863509017fa522e313126696dc52cb`  
		Last Modified: Fri, 15 Dec 2023 23:22:25 GMT  
		Size: 17.7 MB (17732314 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8bf9cf9e004e4dfa0d53087b09c6b16750e65e3acadb8433a2be0585305b2300`  
		Last Modified: Fri, 15 Dec 2023 23:22:30 GMT  
		Size: 201.0 MB (200965374 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:23-jdk-bookworm` - unknown; unknown

```console
$ docker pull openjdk@sha256:597559a468db392e4c8c424fe2991319dd5afb0a18813e5d88a768898056ea2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7253943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9808a40c47794069a47907f252ed7a189d34ba5a0bf7dad998eb9c537ace5bea`

```dockerfile
```

-	Layers:
	-	`sha256:f936c2ab9c35c4e4fe8c4525e17f0eaa873bd762bff8eebcfcfb2900f50e8556`  
		Last Modified: Fri, 15 Dec 2023 23:22:25 GMT  
		Size: 7.2 MB (7235039 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:030a515380d97ed02410971d3669f66afa41fa23ee487205db61f097fa35e401`  
		Last Modified: Fri, 15 Dec 2023 23:22:24 GMT  
		Size: 18.9 KB (18904 bytes)  
		MIME: application/vnd.in-toto+json
