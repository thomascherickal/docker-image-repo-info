## `clojure:openjdk-18-boot-slim-buster`

```console
$ docker pull clojure@sha256:7e5c5bd2fb056707fa6bd2907e06c844a78122d322cb562638271480198fe733
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-boot-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:e7aa2f330cab8fec5f506f6c843f0cd12679a2ac67a14e2a887a462071ec57b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.5 MB (278484886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d8ee5bd9e9b4c86019ac85a0c542fc5d51733d84e57261d8e0891bb3a3cec8`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

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
# Fri, 10 Dec 2021 22:03:55 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 10 Dec 2021 22:03:56 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 10 Dec 2021 22:03:56 GMT
WORKDIR /tmp
# Fri, 10 Dec 2021 22:04:01 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 10 Dec 2021 22:04:01 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 10 Dec 2021 22:04:02 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 10 Dec 2021 22:04:35 GMT
RUN boot
# Fri, 10 Dec 2021 22:04:35 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 10 Dec 2021 22:04:36 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 10 Dec 2021 22:04:36 GMT
CMD ["repl"]
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
	-	`sha256:50b2644724fe377ab6bfb9fb92db160b6e73d2082efba268a1d9239f3627e8e3`  
		Last Modified: Fri, 10 Dec 2021 22:12:31 GMT  
		Size: 279.8 KB (279823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ccfd8fa32ebed44691c0e113e89d126fbc96798230a297e9ca87eb5388afe87`  
		Last Modified: Fri, 10 Dec 2021 22:12:34 GMT  
		Size: 58.8 MB (58820658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ddf8b5b4c9ed66a11d7cec39b7268268605a59a441c9f2b52916185ad6c300`  
		Last Modified: Fri, 10 Dec 2021 22:12:30 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-boot-slim-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:71d82c76a172153117d0233b045e2f910f94152b7a3c3c4acbed7f4d679ada44
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.6 MB (275593129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0accb7f50dfc967e48ea7796ce314db0b813f590932133d8b647331e6c8f86f`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

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
# Fri, 10 Dec 2021 23:14:57 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 10 Dec 2021 23:14:58 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 10 Dec 2021 23:14:59 GMT
WORKDIR /tmp
# Fri, 10 Dec 2021 23:15:04 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 10 Dec 2021 23:15:05 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 10 Dec 2021 23:15:06 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 10 Dec 2021 23:15:29 GMT
RUN boot
# Fri, 10 Dec 2021 23:15:31 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 10 Dec 2021 23:15:31 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 10 Dec 2021 23:15:32 GMT
CMD ["repl"]
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
	-	`sha256:31e55d4419408002d5447d3d5c223ca955054736bac60d94b528a740fd6caa2f`  
		Last Modified: Fri, 10 Dec 2021 23:27:08 GMT  
		Size: 67.5 KB (67541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab8f9b54b79cf3e4763e3d622d581518e5d6ae64bc81c56bea1b0365013fea8`  
		Last Modified: Fri, 10 Dec 2021 23:27:13 GMT  
		Size: 58.8 MB (58816338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163926d5e8d05470a740a1e8392d9eb75b70382fb57a3ce262d5f4b648704a29`  
		Last Modified: Fri, 10 Dec 2021 23:27:08 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
