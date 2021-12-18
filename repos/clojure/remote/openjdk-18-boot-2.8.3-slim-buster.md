## `clojure:openjdk-18-boot-2.8.3-slim-buster`

```console
$ docker pull clojure@sha256:ee6a357d0fc900348246bb2a5e3ad5416ca22ebfd888f506b21b10814f873d27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-boot-2.8.3-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:f8474a8c78ff56dfde161122d5981902f5f254c0a757295df934422d98be0bf9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.5 MB (278536379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1863ed6818c6ead6dd6842e09b64ba04cb9d74aac9a96cd38489cb36ea0af0d3`
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
# Sat, 18 Dec 2021 04:11:52 GMT
ENV JAVA_VERSION=18-ea+28
# Sat, 18 Dec 2021 04:12:07 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='7e5f0e54c799f8c155a934e61d88f4fef3a70a641c1636c925158622c7bd9341'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='e29aa39763ebcfe5f037cc4fe47c6b9eb34cbe482f6ea57e93de89070255e22b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 18 Dec 2021 04:12:07 GMT
CMD ["jshell"]
# Sat, 18 Dec 2021 06:50:02 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 18 Dec 2021 06:50:03 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 18 Dec 2021 06:50:03 GMT
WORKDIR /tmp
# Sat, 18 Dec 2021 06:50:08 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 18 Dec 2021 06:50:08 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 18 Dec 2021 06:50:08 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 18 Dec 2021 06:50:53 GMT
RUN boot
# Sat, 18 Dec 2021 06:50:53 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Sat, 18 Dec 2021 06:50:53 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 18 Dec 2021 06:50:54 GMT
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
	-	`sha256:b6fcca4b8a0d7e8f5eaa98fdcf97f0e34def478e6fd8229f64a3ea47c7b8caf7`  
		Last Modified: Sat, 18 Dec 2021 04:25:43 GMT  
		Size: 189.0 MB (189011855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b200df20633357e5e6f504ff46ed5acd7f78e15f6a4b7589d616a3ff99659870`  
		Last Modified: Sat, 18 Dec 2021 06:59:03 GMT  
		Size: 279.8 KB (279804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcad31b624c8a832075f9bdf5aad9c736a5be48a293fd1a98726735107edfdf3`  
		Last Modified: Sat, 18 Dec 2021 06:59:07 GMT  
		Size: 58.8 MB (58820959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a26ea5030f8a4f591eea205a6bfcc09fce977920cf4ca9b4eb543ab3f9ea33b`  
		Last Modified: Sat, 18 Dec 2021 06:59:03 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-boot-2.8.3-slim-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:ab5e723c7b6520d05b699e9caad2658c9d4fd0d6e569bef997ed1673d704ba29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.7 MB (275667256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91e43131f7363c70ceccd088c2b11e71e8c68b837870d0bfd57323ea9408ea33`
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
# Fri, 17 Dec 2021 23:45:06 GMT
ENV JAVA_VERSION=18-ea+28
# Fri, 17 Dec 2021 23:45:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='7e5f0e54c799f8c155a934e61d88f4fef3a70a641c1636c925158622c7bd9341'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='e29aa39763ebcfe5f037cc4fe47c6b9eb34cbe482f6ea57e93de89070255e22b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 17 Dec 2021 23:45:20 GMT
CMD ["jshell"]
# Sat, 18 Dec 2021 00:30:21 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 18 Dec 2021 00:30:22 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 18 Dec 2021 00:30:23 GMT
WORKDIR /tmp
# Sat, 18 Dec 2021 00:30:28 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 18 Dec 2021 00:30:29 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 18 Dec 2021 00:30:30 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 18 Dec 2021 00:31:09 GMT
RUN boot
# Sat, 18 Dec 2021 00:31:11 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Sat, 18 Dec 2021 00:31:11 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 18 Dec 2021 00:31:12 GMT
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
	-	`sha256:0edef99cacc4b0a23fd5f6b9fddbd12345d270199685bb97304918f0f7f3b6ff`  
		Last Modified: Sat, 18 Dec 2021 00:05:13 GMT  
		Size: 187.7 MB (187740634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6eeb47b8f27d0b720aa466b95d3d03c185f8960dfd3aa15253c8c48c41e8e03`  
		Last Modified: Sat, 18 Dec 2021 00:42:43 GMT  
		Size: 67.5 KB (67549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019062f14bf36ad7f398411ffd84852a34039a4ae8755775a9b04fa03622c016`  
		Last Modified: Sat, 18 Dec 2021 00:42:49 GMT  
		Size: 58.8 MB (58816651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9cbb5bbdfbb7238531f4b9f33a5eab819cd9a9d57686e3310ff725f79de809`  
		Last Modified: Sat, 18 Dec 2021 00:42:43 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
