## `openjdk:17-ea-17-slim`

```console
$ docker pull openjdk@sha256:3cfd2807872bce58e0da95921c5d5dd52752aec7e42bb16898072a90bcad472b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:17-ea-17-slim` - linux; amd64

```console
$ docker pull openjdk@sha256:2e1e0f54ccf6118b88f9d218c1d46cab6f14498ece52a27e73a59f9726f0e35a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.8 MB (216753417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:091962337324d8feb20b16fc9cb9c83dac0ff8821ff65ee945b584941f36e5e0`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 05:41:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 05:41:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 31 Mar 2021 05:41:07 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 05:41:07 GMT
ENV LANG=C.UTF-8
# Fri, 09 Apr 2021 18:55:52 GMT
ENV JAVA_VERSION=17-ea+17
# Fri, 09 Apr 2021 18:56:06 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/17/GPL/openjdk-17-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='a53ace955971ef1ad745c2e9fef7f76b57b51d57e7076dd3a55243ab65febf87'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/17/GPL/openjdk-17-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='ccd8ee7bb908835e697ebae8dbe38d2cf68d9f266e2d9787bdf34d26da30e45b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 09 Apr 2021 18:56:07 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875a154571f097680e56e5acc7383853036fac0e52855a4dd4fa740bfabf3f95`  
		Last Modified: Wed, 31 Mar 2021 05:52:39 GMT  
		Size: 3.3 MB (3268916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66cb6c029e779c6f74df0e401df856a138f1dc6ab2ec879fa41e0e2dbc800c1`  
		Last Modified: Fri, 09 Apr 2021 19:03:08 GMT  
		Size: 186.3 MB (186345208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-ea-17-slim` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:a7143a33cb60be6e538723921b946e9cf3b069abfb8e498ed5f2389b53d02f80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.4 MB (211416800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cca56e20a88de08ba464522397976624b84c88ddaa31389b84802bce67f016e8`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 30 Mar 2021 21:47:15 GMT
ADD file:a9b57ded2400fc7f60ea40e5ccdd3e9bf0f72acfcc47223ceb66b4fa16955059 in / 
# Tue, 30 Mar 2021 21:47:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:39:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:39:29 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 31 Mar 2021 01:39:30 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 01:39:32 GMT
ENV LANG=C.UTF-8
# Fri, 09 Apr 2021 18:42:43 GMT
ENV JAVA_VERSION=17-ea+17
# Fri, 09 Apr 2021 18:43:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/17/GPL/openjdk-17-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='a53ace955971ef1ad745c2e9fef7f76b57b51d57e7076dd3a55243ab65febf87'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/17/GPL/openjdk-17-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='ccd8ee7bb908835e697ebae8dbe38d2cf68d9f266e2d9787bdf34d26da30e45b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 09 Apr 2021 18:43:32 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6fcf2156bc23db75595b822b865fbc962ed6f4521dec8cae509e66742a6a5ad3`  
		Last Modified: Tue, 30 Mar 2021 21:54:27 GMT  
		Size: 25.9 MB (25904513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fde6667c188c81fcddee021ccbb3e054ebe83350fd4609e17a3d37f0ec7f9d`  
		Last Modified: Wed, 31 Mar 2021 01:49:41 GMT  
		Size: 3.1 MB (3118896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8b16884924ead4ccd567c020ee1730887bce95b7e3280b7c55dd93d97ac2b0`  
		Last Modified: Fri, 09 Apr 2021 18:49:26 GMT  
		Size: 182.4 MB (182393391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
