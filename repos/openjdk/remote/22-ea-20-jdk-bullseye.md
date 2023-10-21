## `openjdk:22-ea-20-jdk-bullseye`

```console
$ docker pull openjdk@sha256:bf17ff39268daa84b234221b4386ef835a7b41197ee41598890b589567dcedb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `openjdk:22-ea-20-jdk-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:d3b13ca7a34e73ffc3b103e4089c099d474df367c659d244f18f2e7cc1576b76
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.3 MB (343275890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb9b0266ed69fc7ec5733829148c7f42b7f86019b5ef6e11c5423dc5fc49f002`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:58 GMT
ADD file:e1a6c6c976e5e7c53eb2a7343a7a763b46e56828588535f4c79e63d6ec08198d in / 
# Wed, 11 Oct 2023 18:24:58 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:46:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:46:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:50:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:50:35 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Wed, 11 Oct 2023 22:50:35 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 22:50:35 GMT
ENV LANG=C.UTF-8
# Fri, 20 Oct 2023 23:59:32 GMT
ENV JAVA_VERSION=22-ea+20
# Fri, 20 Oct 2023 23:59:41 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/20/GPL/openjdk-22-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='5f1627efa81951307900954bbf7b2e49d8c5303615cf116959c273e9707b0496'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/20/GPL/openjdk-22-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='8fa022a3b05cc606bccbb014baea9e821954a789ba40b6fd39b40cd4453fb9f5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 20 Oct 2023 23:59:43 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:dd0dc10f921f4b3b65b17f20d367374079e6cb4e26531624ee64caaaf4adcc28`  
		Last Modified: Wed, 11 Oct 2023 18:28:45 GMT  
		Size: 53.7 MB (53707810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7a630df11a812111dd2b7f5b819a692f2350ad055fab0cd3e60b322c2eead5`  
		Last Modified: Wed, 11 Oct 2023 19:54:57 GMT  
		Size: 15.7 MB (15749899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c8e3bce435b9fb78d2fd6a8f0ce18ddecff51902c10074a9da4287cb35963b`  
		Last Modified: Wed, 11 Oct 2023 19:55:14 GMT  
		Size: 54.7 MB (54700074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce69653b6ca4f5b8af5395fb51702430f4939c431d3783d57c5d63306413bde`  
		Last Modified: Wed, 11 Oct 2023 22:53:03 GMT  
		Size: 15.5 MB (15529844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a158a9ff3744e26ff2c409fac0fe6a18f8bb4a689d5eda8e576b3e53e38964ce`  
		Last Modified: Sat, 21 Oct 2023 00:06:18 GMT  
		Size: 203.6 MB (203588263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
