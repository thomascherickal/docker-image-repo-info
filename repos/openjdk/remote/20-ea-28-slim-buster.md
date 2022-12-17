## `openjdk:20-ea-28-slim-buster`

```console
$ docker pull openjdk@sha256:81f37da84db4cb618da68d37c5f6885c25909246fdfdfc42208905e3e9e5ee5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-28-slim-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:6a02370e9f12a0a1691354582374ff48a2a2bcf4a5fa1308b34e8b150e6a6513
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.9 MB (228885448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8343ba00c3e711f550149616062027503e8afc8791443c6828809594ff5b92df`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:18 GMT
ADD file:30180333dcb9028c0d2776f05042f6f309238b100863a050f3981fb80604e871 in / 
# Tue, 06 Dec 2022 01:21:18 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 05:06:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 05:06:57 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 06 Dec 2022 05:06:57 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 05:06:58 GMT
ENV LANG=C.UTF-8
# Fri, 16 Dec 2022 23:33:04 GMT
ENV JAVA_VERSION=20-ea+28
# Fri, 16 Dec 2022 23:33:18 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/28/GPL/openjdk-20-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='d7b481073f0135b7862e9867a61f2133012fc7e555c7f04a383004cedcaad316'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/28/GPL/openjdk-20-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='2201e01fa03d9921f68a072ff6175eddef9370d6ecb1b47f2e6dc200f12f0aca'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 16 Dec 2022 23:33:19 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6eab20599fab240a56b06125a77b4921dd39662d3b9f9008da7306531772a1d0`  
		Last Modified: Tue, 06 Dec 2022 01:25:52 GMT  
		Size: 27.1 MB (27140356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9669963fa8087b26171d843ba42c25760333a213b886c3b12289e827c22c574d`  
		Last Modified: Tue, 06 Dec 2022 05:12:29 GMT  
		Size: 3.3 MB (3275939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9885bf712149934235d05f905181e755c4fd42857097f6f2aad48ca45cf05325`  
		Last Modified: Fri, 16 Dec 2022 23:43:27 GMT  
		Size: 198.5 MB (198469153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-28-slim-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:3bf4ebcdd1d6def193de82d1de9e3d1ef01ec363b361e4d31b908d24e4c85689
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.0 MB (226009366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47b1ff2292a8041e8f38458e259e8c66b8e58dc901ef446572b7b7f1a184da7e`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:34 GMT
ADD file:764288ad3920160093c500e1a7277f174a656030bbe3a0511e7925e84495b6ee in / 
# Tue, 06 Dec 2022 01:40:34 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:28:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 06 Dec 2022 04:28:02 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 04:28:02 GMT
ENV LANG=C.UTF-8
# Sat, 17 Dec 2022 00:28:38 GMT
ENV JAVA_VERSION=20-ea+28
# Sat, 17 Dec 2022 00:28:49 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/28/GPL/openjdk-20-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='d7b481073f0135b7862e9867a61f2133012fc7e555c7f04a383004cedcaad316'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/28/GPL/openjdk-20-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='2201e01fa03d9921f68a072ff6175eddef9370d6ecb1b47f2e6dc200f12f0aca'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 17 Dec 2022 00:28:50 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b473b36a3d93c888196b326b1aad1f802bb6a9fa6fcbc5d2614d99a67899d587`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 25.9 MB (25914951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198ebe9071c02f951926aefb5793b954b3398b0073a3c4a5b8ce0984c4f12050`  
		Last Modified: Tue, 06 Dec 2022 04:33:26 GMT  
		Size: 3.1 MB (3129343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a0175ece43e1cbd19e0d90d872f5334ce7c51a8ebf2364d20631672605d4a8`  
		Last Modified: Sat, 17 Dec 2022 00:38:48 GMT  
		Size: 197.0 MB (196965072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
