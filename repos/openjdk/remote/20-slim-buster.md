## `openjdk:20-slim-buster`

```console
$ docker pull openjdk@sha256:0a64d13c0c3af5c91f2fc85d37b29624481e5b29535c901ab9b207078a6015b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-slim-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:ff5359fb115205be70c6a9a84c427a2149dbfb62cf56ced31ee12cc65c10ec52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.0 MB (227969617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a58029fd15f22e9733fec1143c6f94c3e0b7b0cd8b5084f52083c1361a605c99`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:10 GMT
ADD file:baca493d7744d12304f6d9c7b6ec0800453a0ba02cbf4005ec35c7b921adf0c4 in / 
# Tue, 23 Aug 2022 00:21:10 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:30:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:30:24 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 23 Aug 2022 04:30:24 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 04:30:24 GMT
ENV LANG=C.UTF-8
# Thu, 01 Sep 2022 23:30:17 GMT
ENV JAVA_VERSION=20-ea+13
# Thu, 01 Sep 2022 23:30:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/13/GPL/openjdk-20-ea+13_linux-x64_bin.tar.gz'; 			downloadSha256='93758735b85b0f9e8a98728ad636942bcf266476824286754fe6dbd2a2f6aeff'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/13/GPL/openjdk-20-ea+13_linux-aarch64_bin.tar.gz'; 			downloadSha256='305cd60ab947992620abe377f9d1fe876c6a80db3fab369a8cb5517edbfc30be'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 01 Sep 2022 23:30:58 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2238450926aa858e592e60bb5d68dd26eeab8a984eee45505ca89d2022e3b450`  
		Last Modified: Tue, 23 Aug 2022 00:25:43 GMT  
		Size: 27.1 MB (27138330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4bb2aa3cefa352eef3f71a4b1e2d70041ef3c1e9cf1b9802e5d43db17fcf35`  
		Last Modified: Tue, 23 Aug 2022 04:37:53 GMT  
		Size: 3.3 MB (3273368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243e3ce118a3c86449468877c5d3c5c884613791501358bd3ac07da07db7da69`  
		Last Modified: Thu, 01 Sep 2022 23:37:37 GMT  
		Size: 197.6 MB (197557919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-slim-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:1c6fbf33b935afaa0e02086cd1fc1a717a1018c20716bc5592290b76eef923ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.9 MB (224936604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae235d8759ae1d354cb59c6e07e92f237e9ea98c35c127ce3b316d638c55a42c`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:58 GMT
ADD file:4c5bca2d158b11314fb47a6d4b34239575621c2f00f92e77870f23aa02913fac in / 
# Tue, 23 Aug 2022 01:52:59 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 05:17:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 05:17:33 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 23 Aug 2022 05:17:34 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 05:17:35 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 00:44:35 GMT
ENV JAVA_VERSION=20-ea+13
# Fri, 02 Sep 2022 00:44:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/13/GPL/openjdk-20-ea+13_linux-x64_bin.tar.gz'; 			downloadSha256='93758735b85b0f9e8a98728ad636942bcf266476824286754fe6dbd2a2f6aeff'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/13/GPL/openjdk-20-ea+13_linux-aarch64_bin.tar.gz'; 			downloadSha256='305cd60ab947992620abe377f9d1fe876c6a80db3fab369a8cb5517edbfc30be'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 02 Sep 2022 00:44:53 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a84b81edbdb892b3702892bbb01c240695b0b9d619fda43a9b951c9d2df1443c`  
		Last Modified: Tue, 23 Aug 2022 01:58:50 GMT  
		Size: 25.9 MB (25912515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356227960c8e171a8438469fe7c95bc6d10c5694b55ced0cb37aaaabaef7f2dc`  
		Last Modified: Tue, 23 Aug 2022 05:29:25 GMT  
		Size: 3.1 MB (3126086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7505dd18090dcf3a5799f718ee91e80c63e39985e50cefd614e827b002a573`  
		Last Modified: Fri, 02 Sep 2022 00:55:39 GMT  
		Size: 195.9 MB (195898003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
