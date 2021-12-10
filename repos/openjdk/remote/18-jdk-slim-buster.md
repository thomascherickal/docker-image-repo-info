## `openjdk:18-jdk-slim-buster`

```console
$ docker pull openjdk@sha256:225ea6c4854ca58d883180103be36cca65035973ad87df8b6bd6a930ec70034c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-jdk-slim-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:a9690247f537bee08d0012043043c3c68835829e26e15bec2ea23bb2c1f29375
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.4 MB (219384001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e6e9a42c96e094cf8e6801432b4f26a10c9fa22561875cbf15e9644376de397`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 11:30:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:30:51 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Thu, 02 Dec 2021 11:30:51 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 11:30:51 GMT
ENV LANG=C.UTF-8
# Fri, 10 Dec 2021 21:21:25 GMT
ENV JAVA_VERSION=18-ea+27
# Fri, 10 Dec 2021 21:21:41 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/27/GPL/openjdk-18-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='625301c146fd49d5f45dae30876079fe01ee959d84573a056426362fd6699f1f'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/27/GPL/openjdk-18-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='ad926dc5db48de8dce170eb97ed1539d03829b3f23cf4a2a654e0f8f296be8e7'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 10 Dec 2021 21:21:42 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169731f46e61fb8aef8f7ed809068db98d3feb2466197e9680dbbdbb80d8ed90`  
		Last Modified: Thu, 02 Dec 2021 11:48:59 GMT  
		Size: 3.3 MB (3269625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468a3a429e6318710a0d2fe1348e7bf50a73640fb34eaeed7a24eeda8480df79`  
		Last Modified: Fri, 10 Dec 2021 21:30:06 GMT  
		Size: 189.0 MB (188960647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-jdk-slim-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:63bfdea0a38e9fb431b987da586c26554439c6ab992d58e57ff1dcdc535b7f15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.7 MB (216708844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a479e092f175fb0be631a4006bdc86297b891e736e65b5b6a1847db3919b8b35`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 11:03:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:03:23 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Thu, 02 Dec 2021 11:03:24 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 11:03:25 GMT
ENV LANG=C.UTF-8
# Fri, 10 Dec 2021 21:53:51 GMT
ENV JAVA_VERSION=18-ea+27
# Fri, 10 Dec 2021 21:54:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/27/GPL/openjdk-18-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='625301c146fd49d5f45dae30876079fe01ee959d84573a056426362fd6699f1f'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/27/GPL/openjdk-18-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='ad926dc5db48de8dce170eb97ed1539d03829b3f23cf4a2a654e0f8f296be8e7'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 10 Dec 2021 21:54:08 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7c7f43e0be8e395071a65cf4a7b754dc421cf18e5de6bde1fab5e7376f8d28`  
		Last Modified: Thu, 02 Dec 2021 11:24:55 GMT  
		Size: 3.1 MB (3118874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3828d7f15d72abec822039673c103cc1ae0d91b6a7c8341d6030b5ba324bdffe`  
		Last Modified: Fri, 10 Dec 2021 22:07:49 GMT  
		Size: 187.7 MB (187666826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
