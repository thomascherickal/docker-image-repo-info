## `openjdk:20-ea-8-slim-buster`

```console
$ docker pull openjdk@sha256:7a46cd2f2478b9feabd206533404a1eb0d60a73713b1a2a26dcd1b109578e839
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-8-slim-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:c6750338184a7d3575b0cc3430d79c29a884e64658fc17750f5f76165b5b529b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.9 MB (227891893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e70a73153b8c5908fff855ab9b27110c2721ea30cc8e1a89bf5ccc9fb740e8c6`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:32 GMT
ADD file:7f2320197e75c5169402827ce0c47d93629331875d76b9f0ddd389244747eccd in / 
# Tue, 12 Jul 2022 01:20:33 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:56:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 01:56:05 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 12 Jul 2022 01:56:06 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 01:56:06 GMT
ENV LANG=C.UTF-8
# Fri, 29 Jul 2022 02:03:59 GMT
ENV JAVA_VERSION=20-ea+8
# Fri, 29 Jul 2022 02:04:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/8/GPL/openjdk-20-ea+8_linux-x64_bin.tar.gz'; 			downloadSha256='2e4e4cf5e00dbef999c047b82bcde7abf801f9ef8f0b144fa72d2c3fe8f0a4b6'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/8/GPL/openjdk-20-ea+8_linux-aarch64_bin.tar.gz'; 			downloadSha256='ce07f1a5afc64397de7a13d559c8b3f92f1a843b7efe3e11d969ee64a04fba55'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 29 Jul 2022 02:04:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ac2fb615420c18b61e0693f2569a3d38e3b9b58456b691bac44405e08389a591`  
		Last Modified: Tue, 12 Jul 2022 01:25:22 GMT  
		Size: 27.1 MB (27139850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62264f680cd73ea710b719ee1e279e0a800def0defab33dd092436647625fa1a`  
		Last Modified: Tue, 12 Jul 2022 02:10:29 GMT  
		Size: 3.3 MB (3273429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c0290c3ff0c0eb4d55c560298027d1e136adf869968b514df758fe7bdc5314`  
		Last Modified: Fri, 29 Jul 2022 02:15:12 GMT  
		Size: 197.5 MB (197478614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-8-slim-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:19672ff3c33a5c620823439dc43cc3459c2f0f0d8ee5a391f6e54b692fa007cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.1 MB (225123768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c8236aff678e0c85b445a586d71312123d0cdeaea9b5f541071182a9e8ab42`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 12 Jul 2022 00:41:02 GMT
ADD file:d6b43ca12a2cc7f73a66ace962f04878f02eab9345172028d77c21d3dc94fe0c in / 
# Tue, 12 Jul 2022 00:41:03 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:29:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 01:29:29 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 12 Jul 2022 01:29:30 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 01:29:31 GMT
ENV LANG=C.UTF-8
# Fri, 29 Jul 2022 02:39:07 GMT
ENV JAVA_VERSION=20-ea+8
# Fri, 29 Jul 2022 02:39:21 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/8/GPL/openjdk-20-ea+8_linux-x64_bin.tar.gz'; 			downloadSha256='2e4e4cf5e00dbef999c047b82bcde7abf801f9ef8f0b144fa72d2c3fe8f0a4b6'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/8/GPL/openjdk-20-ea+8_linux-aarch64_bin.tar.gz'; 			downloadSha256='ce07f1a5afc64397de7a13d559c8b3f92f1a843b7efe3e11d969ee64a04fba55'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 29 Jul 2022 02:39:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8bd5501da4f4b37ad7488bd0eafa32d8927de3bf1e32747545810f2ca65429ed`  
		Last Modified: Tue, 12 Jul 2022 00:47:14 GMT  
		Size: 25.9 MB (25914236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebd82c0fcc991163b8dd04e396a3c7388adb7b021c0463cecaa0345cbd7ac1b`  
		Last Modified: Tue, 12 Jul 2022 01:51:21 GMT  
		Size: 3.1 MB (3126061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754a1b8347e53f8dd4f302e42db51e41755c51ea671ed2756863122f89a62983`  
		Last Modified: Fri, 29 Jul 2022 02:56:45 GMT  
		Size: 196.1 MB (196083471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
