## `openjdk:21-ea-2-slim-buster`

```console
$ docker pull openjdk@sha256:75637af5ede24a15034fb593e386d8e01f54707b18b76861f5a904616d78024f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-2-slim-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:03535a7d917aa3362a16850bf52e3256412d59297b839d1653727fd02609a047
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.8 MB (229772392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1dd8bb489a181bf2acd00b35a80ef40b131cac65f626ab0fa103ac37ea3fe1a`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:18 GMT
ADD file:30180333dcb9028c0d2776f05042f6f309238b100863a050f3981fb80604e871 in / 
# Tue, 06 Dec 2022 01:21:18 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 05:06:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Dec 2022 00:34:17 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Wed, 14 Dec 2022 00:34:17 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Dec 2022 00:34:17 GMT
ENV LANG=C.UTF-8
# Fri, 16 Dec 2022 23:31:05 GMT
ENV JAVA_VERSION=21-ea+2
# Fri, 16 Dec 2022 23:31:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/2/GPL/openjdk-21-ea+2_linux-x64_bin.tar.gz'; 			downloadSha256='8070902e5bfbb71a4e7c723bb0439faeb9f3127e1fb048f7ed4e6a5abc5a3505'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/2/GPL/openjdk-21-ea+2_linux-aarch64_bin.tar.gz'; 			downloadSha256='011358a514a8d4030c36bbd5b7d7fb5c404f326498f4c832ee5f890fff8709db'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 16 Dec 2022 23:31:21 GMT
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
	-	`sha256:d614a9885f4dcc2e0599fade3e407f4ffd5a8f1b9dcaf158ce1752ec1efa5dd2`  
		Last Modified: Fri, 16 Dec 2022 23:39:45 GMT  
		Size: 199.4 MB (199356097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-2-slim-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:906b544b08d234be09762aeaab4e34e680989b09e8ed30cfe75d7b3b76ab9ff5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.9 MB (226906104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f123fdd16b76046f437c52c216c98f0ed0d6da4de1db1a08b07a4da08f608d12`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:34 GMT
ADD file:764288ad3920160093c500e1a7277f174a656030bbe3a0511e7925e84495b6ee in / 
# Tue, 06 Dec 2022 01:40:34 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Dec 2022 00:54:47 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Wed, 14 Dec 2022 00:54:47 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Dec 2022 00:54:47 GMT
ENV LANG=C.UTF-8
# Sat, 17 Dec 2022 00:26:57 GMT
ENV JAVA_VERSION=21-ea+2
# Sat, 17 Dec 2022 00:27:10 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/2/GPL/openjdk-21-ea+2_linux-x64_bin.tar.gz'; 			downloadSha256='8070902e5bfbb71a4e7c723bb0439faeb9f3127e1fb048f7ed4e6a5abc5a3505'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/2/GPL/openjdk-21-ea+2_linux-aarch64_bin.tar.gz'; 			downloadSha256='011358a514a8d4030c36bbd5b7d7fb5c404f326498f4c832ee5f890fff8709db'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 17 Dec 2022 00:27:12 GMT
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
	-	`sha256:7e843d0fd37de3948def348d087b8410c3191630c3e0086325874f128b38864f`  
		Last Modified: Sat, 17 Dec 2022 00:35:21 GMT  
		Size: 197.9 MB (197861810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
