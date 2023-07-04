## `openjdk:21-ea-29-slim-bullseye`

```console
$ docker pull openjdk@sha256:1f9ab9acf16731141b97fe31d8af9aa29169753deac2dcdc033f7a42f7c26c81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-29-slim-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:246f19ecec351eaa846847da32ad08172af0ae2387783ff4f821a2df4440c7db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.2 MB (237245282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aadfb1b460ac2d2fbc5f8bed24e775fef29d2045c22f5625829e95a810831cff`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:53:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 01:54:54 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Tue, 04 Jul 2023 01:54:54 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 01:54:54 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 01:54:54 GMT
ENV JAVA_VERSION=21-ea+29
# Tue, 04 Jul 2023 01:55:07 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/29/GPL/openjdk-21-ea+29_linux-x64_bin.tar.gz'; 			downloadSha256='414ca270602b11d0b674c105d1d5577793c9db79e2947187e663dba4750cbf9b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/29/GPL/openjdk-21-ea+29_linux-aarch64_bin.tar.gz'; 			downloadSha256='ddfa7ea3dd22c846676b4def3aef78a5411c208987ace8f47bbcfafd33f26f46'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 04 Jul 2023 01:55:07 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae78b1797b5f8b06d429ce740e570a94adf8b155152e2e3faa83a259c83894cc`  
		Last Modified: Tue, 04 Jul 2023 01:59:02 GMT  
		Size: 1.6 MB (1582468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5644baf89b4a613a359190715b9faf0f103a5743374ca28e1479b098c0ec316`  
		Last Modified: Tue, 04 Jul 2023 02:03:04 GMT  
		Size: 204.2 MB (204245426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-29-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:ff6da91c1d01a853095622a888eab823b153f378057c9941c7113849332d9f2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.2 MB (234211700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec61f1a1aa3df2318ca9211eb28da6c1b52e0b6dc548072cb417ee97dc6d720d`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:38:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:40:16 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Tue, 13 Jun 2023 04:40:16 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:40:16 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 01:20:11 GMT
ENV JAVA_VERSION=21-ea+29
# Tue, 04 Jul 2023 01:20:22 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/29/GPL/openjdk-21-ea+29_linux-x64_bin.tar.gz'; 			downloadSha256='414ca270602b11d0b674c105d1d5577793c9db79e2947187e663dba4750cbf9b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/29/GPL/openjdk-21-ea+29_linux-aarch64_bin.tar.gz'; 			downloadSha256='ddfa7ea3dd22c846676b4def3aef78a5411c208987ace8f47bbcfafd33f26f46'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 04 Jul 2023 01:20:24 GMT
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
	-	`sha256:a55f5f5926ba67212ab9aace57de26a51b7d1ff0ae4f79a6823a3c895f8d4cb4`  
		Last Modified: Tue, 04 Jul 2023 01:27:32 GMT  
		Size: 202.6 MB (202582406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
