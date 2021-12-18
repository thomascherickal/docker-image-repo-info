## `openjdk:19-slim-bullseye`

```console
$ docker pull openjdk@sha256:a67098ced826179cb1068a4fa30f3b2c56c720a9f19d9f7c3ba07d3db81aae71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-slim-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:c2164adc2bb89567c52158eed44acaf953e8a43d3b4563c17aea209c3b8ed289
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.8 MB (222831129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:686184be92f6160d6775aa7fefe482609fe8a0f5279c2a84dd4098d862ca0a60`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:20 GMT
ADD file:ece5ff85ca549f0b1e9139d29dcb43a52af672d0591c423e28180f6d8d700ad7 in / 
# Thu, 02 Dec 2021 02:48:21 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 11:29:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 14 Dec 2021 01:41:59 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Tue, 14 Dec 2021 01:41:59 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Dec 2021 01:42:00 GMT
ENV LANG=C.UTF-8
# Sat, 18 Dec 2021 04:08:26 GMT
ENV JAVA_VERSION=19-ea+2
# Sat, 18 Dec 2021 04:08:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/2/GPL/openjdk-19-ea+2_linux-x64_bin.tar.gz'; 			downloadSha256='66b20dfbd8d0c7ce80d61fef923fb91721244f6194b191b90f130a3380be459d'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/2/GPL/openjdk-19-ea+2_linux-aarch64_bin.tar.gz'; 			downloadSha256='4e19a1ffdaf1f9890ff45d8ff7264b4c4cc968714466abdfe2b47229aa2e4e2f'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 18 Dec 2021 04:08:51 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e5ae68f740265288a4888db98d2999a638fdcb6d725f427678814538d253aa4d`  
		Last Modified: Thu, 02 Dec 2021 02:53:46 GMT  
		Size: 31.4 MB (31370221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9f5b9b70c2f137dc70e816256e7a568a084d066e7c34c028d30a6a45438685`  
		Last Modified: Thu, 02 Dec 2021 11:47:20 GMT  
		Size: 1.6 MB (1582045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a270b924f84ad65c3c3bda35a95e9e3b407822dadf4b2ee60b306b12b73bb1d1`  
		Last Modified: Sat, 18 Dec 2021 04:20:24 GMT  
		Size: 189.9 MB (189878863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:2c0748a73ec46f50cc7711b63ada8ca983acc8982e2bf49e980326565fd768bc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.0 MB (220008872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5e5e817355adcd02195036222a4af6a6e2b5f96f9a6c92785f06454196a3ea7`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:09 GMT
ADD file:002f2f7c6dc806b24b6c365882acd59d2b3d3fcec46d8fd99130b07a4575c88c in / 
# Thu, 02 Dec 2021 08:08:10 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 11:02:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 14 Dec 2021 01:59:57 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Tue, 14 Dec 2021 01:59:58 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Dec 2021 01:59:59 GMT
ENV LANG=C.UTF-8
# Fri, 17 Dec 2021 23:41:47 GMT
ENV JAVA_VERSION=19-ea+2
# Fri, 17 Dec 2021 23:42:04 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/2/GPL/openjdk-19-ea+2_linux-x64_bin.tar.gz'; 			downloadSha256='66b20dfbd8d0c7ce80d61fef923fb91721244f6194b191b90f130a3380be459d'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/2/GPL/openjdk-19-ea+2_linux-aarch64_bin.tar.gz'; 			downloadSha256='4e19a1ffdaf1f9890ff45d8ff7264b4c4cc968714466abdfe2b47229aa2e4e2f'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 17 Dec 2021 23:42:04 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:968621624b326084ed82349252b333e649eaab39f71866edb2b9a4f847283680`  
		Last Modified: Thu, 02 Dec 2021 08:40:45 GMT  
		Size: 30.1 MB (30056536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595058421fcb005f80f2faa2434369885cb20645caed265e7b4912808701d893`  
		Last Modified: Thu, 02 Dec 2021 11:23:15 GMT  
		Size: 1.4 MB (1361242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3613dffb1d41bd5237eeb338c5d76471c5abbf2acfdb2a37c28d8fdcf236ad`  
		Last Modified: Fri, 17 Dec 2021 23:58:43 GMT  
		Size: 188.6 MB (188591094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
