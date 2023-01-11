## `openjdk:20-ea-30-jdk-slim-buster`

```console
$ docker pull openjdk@sha256:195593486ff2b965b6f8fc1bc87ba3ae4d471226d015b3d2b1f43646a4729506
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-30-jdk-slim-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:23a82c16580a566b36c206f0fa67e08275a7ec327a6a9cb3d2d5a15d51ccec92
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.9 MB (228934664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffe265fb5f104816b0347cdc63de39d4c28ebbe623eb4e1866199badce8d093d`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 11 Jan 2023 02:35:07 GMT
ADD file:67ceb946e54c26c505b5f9f393d77befbd5e9b3b5c069ca301e314ecc74456b0 in / 
# Wed, 11 Jan 2023 02:35:07 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 07:04:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 07:06:17 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Wed, 11 Jan 2023 07:06:17 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 07:06:17 GMT
ENV LANG=C.UTF-8
# Wed, 11 Jan 2023 07:06:17 GMT
ENV JAVA_VERSION=20-ea+30
# Wed, 11 Jan 2023 07:06:31 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/30/GPL/openjdk-20-ea+30_linux-x64_bin.tar.gz'; 			downloadSha256='07b5d85ab1263aa1204c5c03ba27c2184cba75c80fb966ff361640f451d8c1c2'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/30/GPL/openjdk-20-ea+30_linux-aarch64_bin.tar.gz'; 			downloadSha256='18f7e42c0779deda7e49d001254fa146c123a0016d2a7b938540d4802df92b5a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 11 Jan 2023 07:06:32 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:548fcab5fe888f589dd092c68b813bfd65359878bd1950d6b753f749e82ebd7c`  
		Last Modified: Wed, 11 Jan 2023 02:39:48 GMT  
		Size: 27.1 MB (27140352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828545e8b79db162ad5abac22f03044bd33fdec65ab2de0eab43a39483567a11`  
		Last Modified: Wed, 11 Jan 2023 07:12:21 GMT  
		Size: 3.3 MB (3275922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7b7a4eb91c072e1490d74dae9c696648003736f1463668d45dfc4b9a313b7d`  
		Last Modified: Wed, 11 Jan 2023 07:15:01 GMT  
		Size: 198.5 MB (198518390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-30-jdk-slim-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:1e737c0498c63c25570571f0c36ca9d70b967590173b0a4fd15efb66f8a26c31
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.1 MB (226054045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9185dd1e89f784c2dea73a81c902b8e5d1cd03e7537559f7d35e3a7b442b6d6e`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:52 GMT
ADD file:08addf73dde8bf5ac64e0d9bdd1997ce5f406976c19da431616783c14fdb36ac in / 
# Wed, 11 Jan 2023 02:57:52 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 13:33:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 13:34:43 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Wed, 11 Jan 2023 13:34:43 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 13:34:43 GMT
ENV LANG=C.UTF-8
# Wed, 11 Jan 2023 13:34:43 GMT
ENV JAVA_VERSION=20-ea+30
# Wed, 11 Jan 2023 13:34:54 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/30/GPL/openjdk-20-ea+30_linux-x64_bin.tar.gz'; 			downloadSha256='07b5d85ab1263aa1204c5c03ba27c2184cba75c80fb966ff361640f451d8c1c2'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/30/GPL/openjdk-20-ea+30_linux-aarch64_bin.tar.gz'; 			downloadSha256='18f7e42c0779deda7e49d001254fa146c123a0016d2a7b938540d4802df92b5a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 11 Jan 2023 13:34:56 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7fac02f4cd2bcf681b9e156a67009cf4609f45447818b52327d93553bfeb2965`  
		Last Modified: Wed, 11 Jan 2023 03:01:58 GMT  
		Size: 25.9 MB (25914925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c3b6f956b3fce7c340f2d003d19d58e27ae60d033838d462212b60d5e10443`  
		Last Modified: Wed, 11 Jan 2023 13:40:37 GMT  
		Size: 3.1 MB (3129360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729e96da5481de74e877914ddd77c3f5f1a43873c58898bc4f6212487c6e753a`  
		Last Modified: Wed, 11 Jan 2023 13:43:07 GMT  
		Size: 197.0 MB (197009760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
