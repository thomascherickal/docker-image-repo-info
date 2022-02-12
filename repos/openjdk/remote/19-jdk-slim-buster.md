## `openjdk:19-jdk-slim-buster`

```console
$ docker pull openjdk@sha256:d1cac3e9ae5e80455f62d4876406c676c6ddba7cb03fcb1eadcd5ad055e785ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-jdk-slim-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:a4325078d4aca45474facc57b6e8906e503de77c18224c87cebb6831bef1933b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.0 MB (220963473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8618002daabbecc6ab66eb037dbed66e9853e625d73fec75f7274c4141b1fbb`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 09:19:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:19:38 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Wed, 26 Jan 2022 09:19:39 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:19:39 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:50:56 GMT
ENV JAVA_VERSION=19-ea+9
# Fri, 11 Feb 2022 23:51:15 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/9/GPL/openjdk-19-ea+9_linux-x64_bin.tar.gz'; 			downloadSha256='df0cd18dd2885e213244d96e894df4b7f4570eec80a3110f3e50663ba3019c36'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/9/GPL/openjdk-19-ea+9_linux-aarch64_bin.tar.gz'; 			downloadSha256='a77a19b7ec6cd8b57ed1d35d893b166b3d2d5e60036d559fd71f37733bf08031'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:51:16 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa8d0f5eb646a53df0b867301afa43404e868c540fdf170240578844dfd0d6b`  
		Last Modified: Wed, 26 Jan 2022 09:43:10 GMT  
		Size: 3.3 MB (3269688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17b888a1c238ee96d8bf9e1b792dddc6724f72a812721c6b3055c77b8d14d63`  
		Last Modified: Sat, 12 Feb 2022 00:14:14 GMT  
		Size: 190.5 MB (190540054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-jdk-slim-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:036f268d0983cdce1f4f210b92561aad4f155edce3904aa789f4df414fa6e055
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.4 MB (218414425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb12af2978d35b1132bbaf7e30ff4b0b0bced27611a43ecdef1960575142ac8e`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:51:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:51:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Wed, 26 Jan 2022 05:51:03 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:51:04 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:08:30 GMT
ENV JAVA_VERSION=19-ea+9
# Sat, 12 Feb 2022 00:08:46 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/9/GPL/openjdk-19-ea+9_linux-x64_bin.tar.gz'; 			downloadSha256='df0cd18dd2885e213244d96e894df4b7f4570eec80a3110f3e50663ba3019c36'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/9/GPL/openjdk-19-ea+9_linux-aarch64_bin.tar.gz'; 			downloadSha256='a77a19b7ec6cd8b57ed1d35d893b166b3d2d5e60036d559fd71f37733bf08031'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:08:46 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a5c9716b24a17043a5d8ede1303daffeaaa07ff0393fa14caed54f01154833`  
		Last Modified: Wed, 26 Jan 2022 06:14:50 GMT  
		Size: 3.1 MB (3118858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0c4bb8f0870f8bf8abb40307f7c42202e0be5b704f2176fac721cf0404732f`  
		Last Modified: Sat, 12 Feb 2022 00:32:30 GMT  
		Size: 189.4 MB (189372351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
