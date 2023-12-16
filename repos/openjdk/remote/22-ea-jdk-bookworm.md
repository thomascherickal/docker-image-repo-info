## `openjdk:22-ea-jdk-bookworm`

```console
$ docker pull openjdk@sha256:b4d3bf3aabc80f3badc342e149e2341cc25779f99e88e558ee6a516f17b15e86
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `openjdk:22-ea-jdk-bookworm` - linux; amd64

```console
$ docker pull openjdk@sha256:f96fc97dd37a9a7e05485e86dec8e133c2819e4e3c3cd7f95d3f394d2eb713e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.6 MB (357556820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5b166b19d85a42e82171d6ebf153b59aefb168288838e4e3914dbf4fad51756`
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
# Fri, 08 Dec 2023 19:48:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 08 Dec 2023 19:48:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Fri, 08 Dec 2023 19:48:25 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Dec 2023 19:48:25 GMT
ENV LANG=C.UTF-8
# Fri, 08 Dec 2023 19:48:25 GMT
ENV JAVA_VERSION=22-ea+27
# Fri, 08 Dec 2023 19:48:25 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='102a2e0fa1174ba6e67f79685a98122609d7f3106f3745f7418a5224e55e8643'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='39341b5dba8789f64a9f1dd7310ede993d890a44ecde059955992c3260e82b78'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Fri, 08 Dec 2023 19:48:25 GMT
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
	-	`sha256:8cd1b6222bff07f7eade03df1445b5ca4636fca2b21960c0b1a357e0d3cd585c`  
		Last Modified: Fri, 15 Dec 2023 22:05:54 GMT  
		Size: 16.9 MB (16949223 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e4f2b69d417852085e46100c637ef886f360ee0b8c4f2d84d5fc9a6a15b33826`  
		Last Modified: Fri, 15 Dec 2023 22:05:58 GMT  
		Size: 202.8 MB (202845429 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:22-ea-jdk-bookworm` - unknown; unknown

```console
$ docker pull openjdk@sha256:91e47b34807c35f07614a322640caf1cc9f6390425dc9f5d71f44775faa59638
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7135121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a38e82de8f55a1516d12cc74db92c6b0e8918414accc19497f3e35df2942ac5`

```dockerfile
```

-	Layers:
	-	`sha256:90743e3bb13a5233eaa516b972c2d281a2d40b2889ed447ef8ee3265c7ae7168`  
		Last Modified: Fri, 15 Dec 2023 22:05:54 GMT  
		Size: 7.1 MB (7116216 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:550b47ebe55bc7cb458451fd1f37994afa4981a2ce43e9ff1cde06a8f4201378`  
		Last Modified: Fri, 15 Dec 2023 22:05:53 GMT  
		Size: 18.9 KB (18905 bytes)  
		MIME: application/vnd.in-toto+json

### `openjdk:22-ea-jdk-bookworm` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:02288028e820f259b6e1f1f225d5d80eb8166d74f85e01e5852801fa19eb0741
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.8 MB (355821155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de614c354aa61a6206b8db2c980f1e8fc18a275dbef17305859bb51cc0d221c0`
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
# Fri, 08 Dec 2023 19:48:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 08 Dec 2023 19:48:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Fri, 08 Dec 2023 19:48:25 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Dec 2023 19:48:25 GMT
ENV LANG=C.UTF-8
# Fri, 08 Dec 2023 19:48:25 GMT
ENV JAVA_VERSION=22-ea+27
# Fri, 08 Dec 2023 19:48:25 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='102a2e0fa1174ba6e67f79685a98122609d7f3106f3745f7418a5224e55e8643'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='39341b5dba8789f64a9f1dd7310ede993d890a44ecde059955992c3260e82b78'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Fri, 08 Dec 2023 19:48:25 GMT
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
	-	`sha256:4a792695977e2aacb8742098a0db93188ed9009e1fb99647aa87e73abb96131f`  
		Last Modified: Fri, 15 Dec 2023 23:29:04 GMT  
		Size: 200.9 MB (200897040 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:22-ea-jdk-bookworm` - unknown; unknown

```console
$ docker pull openjdk@sha256:cf973a02d912c756cb490686b4b42c9f8887216c6150358a8ecc3fbf610669e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7253467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4489454729cd175fd7f835849c7d837c6301595fd5130396f6819e0770d437e7`

```dockerfile
```

-	Layers:
	-	`sha256:af26e710ebbe861e43e5725d25210657b2ff01b8e07b9c11a05b28e13c2de18d`  
		Last Modified: Fri, 15 Dec 2023 23:28:59 GMT  
		Size: 7.2 MB (7235043 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c60b63fd58e2aea9dea26ebd36c44f6885fb60561b7ca4b9aef92a97dfd565c1`  
		Last Modified: Fri, 15 Dec 2023 23:28:58 GMT  
		Size: 18.4 KB (18424 bytes)  
		MIME: application/vnd.in-toto+json
