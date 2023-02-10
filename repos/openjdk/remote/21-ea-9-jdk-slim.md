## `openjdk:21-ea-9-jdk-slim`

```console
$ docker pull openjdk@sha256:8de7749e70004688ea9bc8e8cbef47084986285686cc59db325bb1781deaba40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `openjdk:21-ea-9-jdk-slim` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:919ece76d4c486e699e844ba267fa0e3e076178afd831603a298c76447e0e6cf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.7 MB (229725668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14e86539ff8f3c63d3320ab54ed2d38ac687cb80a961bd25a9e4b41380507532`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:07:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:07:54 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Thu, 09 Feb 2023 10:07:54 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 10:07:54 GMT
ENV LANG=C.UTF-8
# Fri, 10 Feb 2023 01:57:18 GMT
ENV JAVA_VERSION=21-ea+9
# Fri, 10 Feb 2023 01:57:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/9/GPL/openjdk-21-ea+9_linux-x64_bin.tar.gz'; 			downloadSha256='50ce8bd2e9b710726e7117ba3a302287a0be51cb187721a422ee63cadbf717a2'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/9/GPL/openjdk-21-ea+9_linux-aarch64_bin.tar.gz'; 			downloadSha256='86f137227e32994689e70b0a2f426adb45a16807bc84398926e841452cfe83d0'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 10 Feb 2023 01:57:32 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12ec23d1569af13aa4b739730163609a2c012fc5a8c00a55e2c980462802868`  
		Last Modified: Thu, 09 Feb 2023 10:14:41 GMT  
		Size: 1.6 MB (1566302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43eec875672d1f64dd0da5872777dc4255836c7f68303c3f294a11404ed13d31`  
		Last Modified: Fri, 10 Feb 2023 02:04:42 GMT  
		Size: 198.1 MB (198096857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
