## `clojure:openjdk-16-boot`

```console
$ docker pull clojure@sha256:3ae69f6b0ab573f0fdb3b3a9f82cc8b7466b80b59a7a61bbe89f1fe373c035f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-16-boot` - linux; amd64

```console
$ docker pull clojure@sha256:2b69ee406b45e9633d011df4ff900ee11721efb5a822b0005d72974d009bc5a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.7 MB (274690879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75ab4f12e27c4562b4606e3cc61cd3b69f55000e7ae8f3715ba37ce917e79dee`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 08:00:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 08:02:29 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Wed, 23 Jun 2021 08:02:29 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 08:02:29 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 08:02:29 GMT
ENV JAVA_VERSION=16.0.1
# Wed, 23 Jun 2021 08:02:46 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-x64_bin.tar.gz'; 			downloadSha256='b1198ffffb7d26a3fdedc0fa599f60a0d12aa60da1714b56c1defbce95d8b235'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='602b005074777df2a0b4306e20152a6446803edd87ccbab95b2f313c4d9be6ba'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 23 Jun 2021 08:02:47 GMT
CMD ["jshell"]
# Thu, 24 Jun 2021 02:43:25 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 24 Jun 2021 02:43:25 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 24 Jun 2021 02:43:26 GMT
WORKDIR /tmp
# Thu, 24 Jun 2021 02:43:31 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 24 Jun 2021 02:43:31 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 24 Jun 2021 02:43:31 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 24 Jun 2021 02:43:52 GMT
RUN boot
# Thu, 24 Jun 2021 02:43:53 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee45ae9730633057cf9bd12924f9a1bf2b590631d3d085b14c96f4466557794`  
		Last Modified: Wed, 23 Jun 2021 08:12:04 GMT  
		Size: 3.3 MB (3268886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd24cb1363715cab6b066cccbcdfb412215d244ff8cf0038145d0246f6ca10c`  
		Last Modified: Wed, 23 Jun 2021 08:16:21 GMT  
		Size: 185.2 MB (185175871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07da30d189b2c0ae43c045d9919362fbf0364a7e7342868be5078236463626f`  
		Last Modified: Thu, 24 Jun 2021 02:54:14 GMT  
		Size: 279.8 KB (279757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5f42b0c9bb6225f460dde265ae6946035be0ffa2bf313772a16710d5821621`  
		Last Modified: Thu, 24 Jun 2021 02:54:18 GMT  
		Size: 58.8 MB (58820514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-16-boot` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:b472a0306020b0dd3f8a0dd2b1e64ebdb44c434bb590c4bf286d107a70dfd269
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.7 MB (267692411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2b829a58836ba7b2829ee4b55a885242833ef2bd03a456fede3323411d9d232`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 04:56:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 04:58:21 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Wed, 23 Jun 2021 04:58:21 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 04:58:21 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 04:58:21 GMT
ENV JAVA_VERSION=16.0.1
# Wed, 23 Jun 2021 04:58:33 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-x64_bin.tar.gz'; 			downloadSha256='b1198ffffb7d26a3fdedc0fa599f60a0d12aa60da1714b56c1defbce95d8b235'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='602b005074777df2a0b4306e20152a6446803edd87ccbab95b2f313c4d9be6ba'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 23 Jun 2021 04:58:34 GMT
CMD ["jshell"]
# Wed, 23 Jun 2021 19:58:45 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 23 Jun 2021 19:58:46 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 23 Jun 2021 19:58:46 GMT
WORKDIR /tmp
# Wed, 23 Jun 2021 19:58:55 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 23 Jun 2021 19:58:56 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 23 Jun 2021 19:58:56 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 23 Jun 2021 19:59:16 GMT
RUN boot
# Wed, 23 Jun 2021 19:59:16 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb5c013aa648ff2c30dafc35db9efb2faa7f9fa6f1c98a2f31c1b5fee0334dc`  
		Last Modified: Wed, 23 Jun 2021 05:11:10 GMT  
		Size: 3.1 MB (3118894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f933fcbcc981b073247ef4de4fa9f95dbfe58a932631b03dae69d8025f465e52`  
		Last Modified: Wed, 23 Jun 2021 05:15:44 GMT  
		Size: 179.6 MB (179558374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c9475241280a1a9741bbe8e4e08abd17109ae0463a750c0d5144ec89f197d1`  
		Last Modified: Wed, 23 Jun 2021 20:10:05 GMT  
		Size: 279.6 KB (279588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f10f0308417b2bd665c4e95e9739f434bb7f7832be25b33441931d949b73fff`  
		Last Modified: Wed, 23 Jun 2021 20:10:09 GMT  
		Size: 58.8 MB (58820562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
