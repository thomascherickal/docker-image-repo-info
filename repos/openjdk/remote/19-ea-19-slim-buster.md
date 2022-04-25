## `openjdk:19-ea-19-slim-buster`

```console
$ docker pull openjdk@sha256:bb4f99bc25086cad49147448a9dbd3711f318f8a60f82450fec532d4a59f6236
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-ea-19-slim-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:4ad006074b07a5dc35e4c974d3170996c61d2a84e204abba154d4138c60e16dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.4 MB (225412357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b8b28c82519c9171d3004c31e9b60eb669d479f4956f23c1b62c5075a716266`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:48:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:48:29 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Wed, 20 Apr 2022 10:48:29 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 10:48:29 GMT
ENV LANG=C.UTF-8
# Mon, 25 Apr 2022 18:24:11 GMT
ENV JAVA_VERSION=19-ea+19
# Mon, 25 Apr 2022 18:24:25 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/19/GPL/openjdk-19-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='5920845cb577a0883cfbd0bc3a781b5b0a4f71b19a870525c653f9815fa0596b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/19/GPL/openjdk-19-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='ad9457964256d9d43d6246a0da743a73450231506d0a8a711e28b996b7e6e6e3'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 25 Apr 2022 18:24:26 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b97724dec0639ffbe1d30e60defc8ff8fc2e27a3844e7c6173e64cb73e25b88`  
		Last Modified: Wed, 20 Apr 2022 11:02:57 GMT  
		Size: 3.3 MB (3273257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b9487caabf0788098f78250655b1e7a2b78188bb0f8e2aedd8dbc583556fdc`  
		Last Modified: Mon, 25 Apr 2022 18:36:14 GMT  
		Size: 195.0 MB (194998436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-ea-19-slim-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:30341ea5d5e4940f7ef1e1c0bded7c995f38c012aa5252739dfefe6c7024e84b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.7 MB (222662643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b4e9e16e2ce679085fba3105038556df274243a9afbf97c497479c12cc7cc17`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:25:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:25:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Wed, 20 Apr 2022 10:25:50 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 10:25:51 GMT
ENV LANG=C.UTF-8
# Mon, 25 Apr 2022 18:42:32 GMT
ENV JAVA_VERSION=19-ea+19
# Mon, 25 Apr 2022 18:42:46 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/19/GPL/openjdk-19-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='5920845cb577a0883cfbd0bc3a781b5b0a4f71b19a870525c653f9815fa0596b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/19/GPL/openjdk-19-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='ad9457964256d9d43d6246a0da743a73450231506d0a8a711e28b996b7e6e6e3'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 25 Apr 2022 18:42:46 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef4c0391a581a54e4ae08706ac3173bf39e99722f6efe3a9094dbe8916d7bfd`  
		Last Modified: Wed, 20 Apr 2022 10:47:49 GMT  
		Size: 3.1 MB (3125683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c32237c6e015215f47af63cc19955716a914a4aaba01d580c53fe1eeeebb478`  
		Last Modified: Mon, 25 Apr 2022 19:01:04 GMT  
		Size: 193.6 MB (193628611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
