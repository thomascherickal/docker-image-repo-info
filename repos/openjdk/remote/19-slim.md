## `openjdk:19-slim`

```console
$ docker pull openjdk@sha256:e36fccc9a2a3c1eee42a554f7e07d8f124c1169b1f8d0f3b02396207eea51309
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-slim` - linux; amd64

```console
$ docker pull openjdk@sha256:a18ca4a38a167548d1f51dfb6b96343601a375481adb8177987bdb4ee4373c68
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.1 MB (228087363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2958b5ae283c90e5269fc099adad93a4cfafdd766a32ef6b85867036cb790c01`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:46:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:46:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Wed, 11 May 2022 05:46:48 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 05:46:48 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 05:46:48 GMT
ENV JAVA_VERSION=19-ea+21
# Wed, 11 May 2022 05:47:01 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/21/GPL/openjdk-19-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='8723353dfc5a3dd34d01b96faddc950c48f450083519a62b287fcb1ef82fc446'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/21/GPL/openjdk-19-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='6e9719e928c6bfa2ed1e3ed7885bc2ff3751e0a8a6c5dde6808dddbd239cba32'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 11 May 2022 05:47:02 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf31789c5c1a5e3676cbd7a34472d61217c52c819552f5b116565c22cb6d2f1`  
		Last Modified: Wed, 11 May 2022 05:58:33 GMT  
		Size: 1.6 MB (1582150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9be2bd8343df132155a1714d8bca5dbfdea19fa8e9eba38eb594c7875915a6f`  
		Last Modified: Wed, 11 May 2022 05:58:48 GMT  
		Size: 195.1 MB (195125737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-slim` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:b48abb805ea82223049369a455adf0aadf930a17280ba316074fd37b24da7d33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.2 MB (225197278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:855427d644b79431d8cf1e95025af15905b8c86b9a520db6d3171793eb7b3d46`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 14:15:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:15:57 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Wed, 11 May 2022 14:15:58 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 14:15:59 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 14:16:00 GMT
ENV JAVA_VERSION=19-ea+21
# Wed, 11 May 2022 14:16:12 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/21/GPL/openjdk-19-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='8723353dfc5a3dd34d01b96faddc950c48f450083519a62b287fcb1ef82fc446'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/21/GPL/openjdk-19-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='6e9719e928c6bfa2ed1e3ed7885bc2ff3751e0a8a6c5dde6808dddbd239cba32'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 11 May 2022 14:16:12 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5ad7be01b68fe78dada799da391fe706a6e51b7a0ec158e40069f53de08619`  
		Last Modified: Wed, 11 May 2022 14:33:48 GMT  
		Size: 1.4 MB (1361175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa23babdf3dc31d83ccd42149658ac60a9488085eb16ac9d2b488ce6cee0922a`  
		Last Modified: Wed, 11 May 2022 14:34:05 GMT  
		Size: 193.8 MB (193770410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
