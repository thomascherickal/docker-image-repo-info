## `clojure:openjdk-17-boot-slim-buster`

```console
$ docker pull clojure@sha256:d9c548aebeffe54fee5c410cd67b62c89dc5917e9fbe94e098cc7cb10a4f73de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-17-boot-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:c430ffed92297197f7d365f174f2101187f95ba44df9d811ac4ce6795614ab36
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.5 MB (275539245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd3238360ae597f2965d24eddd2a6e2ec9e140546a478f73f9130136d35787da`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 17:10:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:10:17 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Tue, 09 Feb 2021 17:10:18 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 17:10:18 GMT
ENV LANG=C.UTF-8
# Fri, 26 Feb 2021 21:22:51 GMT
ENV JAVA_VERSION=17-ea+11
# Fri, 26 Feb 2021 21:23:09 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/11/GPL/openjdk-17-ea+11_linux-x64_bin.tar.gz'; 			downloadSha256='03f129a2a92537e3eea68a0f816baae2e97a228deb50176631d040f6895b3d78'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/11/GPL/openjdk-17-ea+11_linux-aarch64_bin.tar.gz'; 			downloadSha256='8680345eaa4cd3e14584f480f75491fd20966a6fd6c9d4a418e0ec55d9d2ed12'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 26 Feb 2021 21:23:09 GMT
CMD ["jshell"]
# Fri, 26 Feb 2021 22:27:00 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 26 Feb 2021 22:27:00 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 26 Feb 2021 22:27:00 GMT
WORKDIR /tmp
# Fri, 26 Feb 2021 22:27:05 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 26 Feb 2021 22:27:06 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 26 Feb 2021 22:27:06 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 26 Feb 2021 22:27:25 GMT
RUN boot
# Fri, 26 Feb 2021 22:27:26 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91c0c19c84860aaa974864243509770a5b009f3a88b4a228010a9ade71ac968`  
		Last Modified: Tue, 09 Feb 2021 17:20:14 GMT  
		Size: 3.3 MB (3267910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a37071eae8ef2be10d6c9333d71dfdc5d736302f8b04d8607071182a6b7ed07`  
		Last Modified: Fri, 26 Feb 2021 21:28:55 GMT  
		Size: 186.1 MB (186076347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d57441f926ea74c49385e8c49bff66210f60b542a7fcca21b6dc3afdeae4e0e`  
		Last Modified: Fri, 26 Feb 2021 22:31:35 GMT  
		Size: 279.7 KB (279738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f1f3d0826f0b4eb615c601fe075cbfec07faf163400e16dde7f654a4da5db9`  
		Last Modified: Fri, 26 Feb 2021 22:31:38 GMT  
		Size: 58.8 MB (58820108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-17-boot-slim-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:b2d0f0eda1194ba7f747588af0bc8154cc2980d6834a73519718850cd6c4b832
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.2 MB (270166581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be4dbe706eb834de9fde7b175d3e5ba13ff549c83cbc1678a1b6497448ab8131`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 07:12:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 07:12:09 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Tue, 09 Feb 2021 07:12:10 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 07:12:11 GMT
ENV LANG=C.UTF-8
# Fri, 26 Feb 2021 21:56:00 GMT
ENV JAVA_VERSION=17-ea+11
# Fri, 26 Feb 2021 21:56:24 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/11/GPL/openjdk-17-ea+11_linux-x64_bin.tar.gz'; 			downloadSha256='03f129a2a92537e3eea68a0f816baae2e97a228deb50176631d040f6895b3d78'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/11/GPL/openjdk-17-ea+11_linux-aarch64_bin.tar.gz'; 			downloadSha256='8680345eaa4cd3e14584f480f75491fd20966a6fd6c9d4a418e0ec55d9d2ed12'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 26 Feb 2021 21:56:26 GMT
CMD ["jshell"]
# Fri, 26 Feb 2021 22:35:52 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 26 Feb 2021 22:35:53 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 26 Feb 2021 22:35:54 GMT
WORKDIR /tmp
# Fri, 26 Feb 2021 22:36:03 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 26 Feb 2021 22:36:04 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 26 Feb 2021 22:36:04 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 26 Feb 2021 22:36:40 GMT
RUN boot
# Fri, 26 Feb 2021 22:36:42 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96062c0c15f683e4abb09efb938dfd7ff23002f72a375c75492d44bde3a6c26f`  
		Last Modified: Tue, 09 Feb 2021 07:22:32 GMT  
		Size: 3.1 MB (3118711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8686785edc66f81a75368e82afa9f07feea9de89d4811e9b6e4afe6a5669a6`  
		Last Modified: Fri, 26 Feb 2021 22:02:19 GMT  
		Size: 182.1 MB (182096095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36af045392ecbc8a6ba9ae8a75bb34243933621464048a3f536ee56ce6e2ee01`  
		Last Modified: Fri, 26 Feb 2021 22:41:36 GMT  
		Size: 279.6 KB (279607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4216edca0d9d4ad911f3f1395e9b1ab67773519777c831cc1359a99e9ba5cf0`  
		Last Modified: Fri, 26 Feb 2021 22:41:38 GMT  
		Size: 58.8 MB (58820719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
