## `clojure:openjdk-19-boot-slim-bullseye`

```console
$ docker pull clojure@sha256:2d0c91b5a0c7ec46daba592e214370b54d7a2ec97eb1084a8b4f265473a0f832
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-19-boot-slim-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:7c2cf8d7f7654c301ab2d0a87c138a5d12a463fc313a686e4e9cdd2b5625c3d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.1 MB (286145045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19cf6f31cd5cd70448a4dae80e7d3182f630ba2b39e4542971a2f497a689a568`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:52:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 00:52:15 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Tue, 29 Mar 2022 00:52:15 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 00:52:15 GMT
ENV LANG=C.UTF-8
# Fri, 08 Apr 2022 20:28:13 GMT
ENV JAVA_VERSION=19-ea+17
# Fri, 08 Apr 2022 20:28:27 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/17/GPL/openjdk-19-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='263cc28c3abc084b653e28887ee67701189283a5d29f840062eb778b47c65dbe'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/17/GPL/openjdk-19-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='50323cdf380ab1d6a8930371ed9e86c29f9e4d99afde67c641be3191087aba87'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 08 Apr 2022 20:28:27 GMT
CMD ["jshell"]
# Sat, 09 Apr 2022 00:58:23 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 09 Apr 2022 00:58:23 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 09 Apr 2022 00:58:23 GMT
WORKDIR /tmp
# Sat, 09 Apr 2022 00:58:28 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 09 Apr 2022 00:58:28 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 09 Apr 2022 00:58:28 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 09 Apr 2022 00:59:06 GMT
RUN boot
# Sat, 09 Apr 2022 00:59:06 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Sat, 09 Apr 2022 00:59:06 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 09 Apr 2022 00:59:06 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1dc05f270bad654ee17f1143c48586c188a72929a128d61fd8ae15905d7b00`  
		Last Modified: Tue, 29 Mar 2022 01:04:32 GMT  
		Size: 1.6 MB (1582122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd55c8c4ce3e9e2bfd4bcc4d40a70ef3eb3c99eaec3ca6cc27fac18a730b67b`  
		Last Modified: Fri, 08 Apr 2022 20:36:45 GMT  
		Size: 194.1 MB (194079969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fe5b46ba9b23220ba59b0181baa53fbaa973a6dd406cf2495314e5ef302c5f`  
		Last Modified: Sat, 09 Apr 2022 01:04:35 GMT  
		Size: 283.1 KB (283080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0070ed9dbea293c9a771e8969f690cc95f697aca60b60a518e9bb832a09995`  
		Last Modified: Sat, 09 Apr 2022 01:04:39 GMT  
		Size: 58.8 MB (58821014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14bd54e3580a0f6944974855fc55a0d86cefc43c4d91c1af3e0b96f64cdb8b8`  
		Last Modified: Sat, 09 Apr 2022 01:04:35 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-19-boot-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:84bb65a5b02d0ff3c03525f509c11f5fc0c18652e93e24debbfa64b5063b5d52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.1 MB (283077323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60d9ee99148d4233985f153c7a57e89684ff636429c20ee4253691d62cabac5b`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:17 GMT
ADD file:e95289cd39de0f389d09cda9edf8476d5da371bc68d76e820c5e1c310dc54baf in / 
# Tue, 29 Mar 2022 00:43:17 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 01:18:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 01:18:12 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Tue, 29 Mar 2022 01:18:13 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 01:18:14 GMT
ENV LANG=C.UTF-8
# Fri, 08 Apr 2022 20:42:45 GMT
ENV JAVA_VERSION=19-ea+17
# Fri, 08 Apr 2022 20:42:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/17/GPL/openjdk-19-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='263cc28c3abc084b653e28887ee67701189283a5d29f840062eb778b47c65dbe'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/17/GPL/openjdk-19-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='50323cdf380ab1d6a8930371ed9e86c29f9e4d99afde67c641be3191087aba87'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 08 Apr 2022 20:42:58 GMT
CMD ["jshell"]
# Fri, 08 Apr 2022 22:45:41 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 08 Apr 2022 22:45:41 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 08 Apr 2022 22:45:42 GMT
WORKDIR /tmp
# Fri, 08 Apr 2022 22:45:47 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 08 Apr 2022 22:45:48 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 08 Apr 2022 22:45:49 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 08 Apr 2022 22:46:20 GMT
RUN boot
# Fri, 08 Apr 2022 22:46:21 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 08 Apr 2022 22:46:21 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 08 Apr 2022 22:46:22 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:2203022c5aa978ec114a15a7cdc2c323c65922d3b0a8eab11d50811bb9ae1cfb`  
		Last Modified: Tue, 29 Mar 2022 00:50:04 GMT  
		Size: 30.1 MB (30064311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dee14fdb7a0a09a9e31998d2906081734dba985b95da3f35b7bd79d79b73330`  
		Last Modified: Tue, 29 Mar 2022 01:37:54 GMT  
		Size: 1.4 MB (1361189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c59a541dc2bf17254b255b713f3a7e6fe497ca4eb617646769b6df7cc53c464`  
		Last Modified: Fri, 08 Apr 2022 20:57:41 GMT  
		Size: 192.8 MB (192767740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3799318de26600ae98c915fe10edb1afb64dacca9f488dc9db5ba9c0b0434940`  
		Last Modified: Fri, 08 Apr 2022 22:56:51 GMT  
		Size: 67.3 KB (67265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0dfb41e5e9627a770c0a3d3d0bf294a1d3c62019b09cc7c193c0405de9e50fc`  
		Last Modified: Fri, 08 Apr 2022 22:56:56 GMT  
		Size: 58.8 MB (58816414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe72ae92b643b3baac06a6ce8bcbd94c0fd6944f01b3611e7d87a3cff802715`  
		Last Modified: Fri, 08 Apr 2022 22:56:51 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
