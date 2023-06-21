## `openjdk:22-ea-2-slim-bullseye`

```console
$ docker pull openjdk@sha256:2f25a310d54102728a894107da4bc36d36ed9c87de58d86a129d87c6202ff89a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:22-ea-2-slim-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:acb758108e806b74a690b740e01cad94d58295b643d27d68ae9ede39002de2f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.0 MB (237981934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1afec2f7fd36fd1f47272ca46be770e45af28d04598fe8954d55b0a69e8b0e69`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:19:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:19:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Tue, 13 Jun 2023 07:19:25 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 07:19:25 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jun 2023 01:13:45 GMT
ENV JAVA_VERSION=22-ea+2
# Wed, 21 Jun 2023 01:14:01 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/2/GPL/openjdk-22-ea+2_linux-x64_bin.tar.gz'; 			downloadSha256='d759c4f3b3cf116701356fb6276cbe5cebac2ff8fbc88e7ca0c10db5c659bf0b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/2/GPL/openjdk-22-ea+2_linux-aarch64_bin.tar.gz'; 			downloadSha256='b60aa1790dc7fa69e983498162b3e0cd883ddc0d89319529cf9dd381b3b04ded'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 21 Jun 2023 01:14:01 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454a143e8504247dc2e9e60b33533bee1b7a6ce927b0222b0354c9ab465ce3bf`  
		Last Modified: Tue, 13 Jun 2023 07:22:50 GMT  
		Size: 1.6 MB (1582441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25190a7d8967dd7e02c9860d0c6952e7ba20b17ec55e1858d5e21e1ab4d558a`  
		Last Modified: Wed, 21 Jun 2023 01:20:07 GMT  
		Size: 205.0 MB (204982083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-ea-2-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:9dcdf356288b7a5efd0380797fedde411543401a6ddf2c0491b7919e5d21e886
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.9 MB (234934884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bc956af8ca7de4b4374f299164daefd88e8d896075adc68c26afb731d45b6dd`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:38:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:38:58 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Tue, 13 Jun 2023 04:38:58 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:38:58 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jun 2023 01:14:47 GMT
ENV JAVA_VERSION=22-ea+2
# Wed, 21 Jun 2023 01:15:00 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/2/GPL/openjdk-22-ea+2_linux-x64_bin.tar.gz'; 			downloadSha256='d759c4f3b3cf116701356fb6276cbe5cebac2ff8fbc88e7ca0c10db5c659bf0b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/2/GPL/openjdk-22-ea+2_linux-aarch64_bin.tar.gz'; 			downloadSha256='b60aa1790dc7fa69e983498162b3e0cd883ddc0d89319529cf9dd381b3b04ded'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 21 Jun 2023 01:15:02 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5dc0b678bee14b591fc8dcf5858d219d0fce4abb02971967b35484ea1bfdd40`  
		Last Modified: Tue, 13 Jun 2023 04:42:13 GMT  
		Size: 1.6 MB (1566460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136ca618beb8de99e2645a226cb890bddabfecb0056f3cd02a710f86f65c44da`  
		Last Modified: Wed, 21 Jun 2023 01:20:47 GMT  
		Size: 203.3 MB (203305590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
