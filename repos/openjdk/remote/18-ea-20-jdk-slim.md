## `openjdk:18-ea-20-jdk-slim`

```console
$ docker pull openjdk@sha256:9c44ec0dd5c8ebdc479a9c4a80c22a0e19b4727a1550f18a385b40d993730793
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `openjdk:18-ea-20-jdk-slim` - linux; amd64

```console
$ docker pull openjdk@sha256:49fd8d33db60e4f9e569392f6f2da10a236f275528587dbde382bab3c249b5f6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221396661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e2ccc3c438f6d70345783895c32417e384a18a4148128b71e270fe18c2fe19`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:42 GMT
ADD file:16dc2c6d1932194edec28d730b004fd6deca3d0f0e1a07bc5b8b6e8a1662f7af in / 
# Tue, 12 Oct 2021 01:20:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:27:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:27:47 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 12 Oct 2021 16:27:47 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 16:27:47 GMT
ENV LANG=C.UTF-8
# Thu, 21 Oct 2021 23:41:41 GMT
ENV JAVA_VERSION=18-ea+20
# Thu, 21 Oct 2021 23:41:56 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/20/GPL/openjdk-18-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='aa609b9f3a4a31b3cb3649a39dabf11476d9c5f1f3b8b9583b2be48e14e3c321'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/20/GPL/openjdk-18-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='a1bfee1fed3794347cfce38d0f4a163b7e90702ceb5fe9256d06664c0daa5726'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 21 Oct 2021 23:41:57 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7d63c13d9b9b6ec5f05a2b07daadacaa9c610d01102a662ae9b1d082105f1ffa`  
		Last Modified: Tue, 12 Oct 2021 01:26:05 GMT  
		Size: 31.4 MB (31357311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225be9814eda07dabebf0e4deb415366f34b2cfe12ef1ad167ba1104423f42d7`  
		Last Modified: Tue, 12 Oct 2021 16:42:59 GMT  
		Size: 1.6 MB (1582043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac27684e3fb0f3efea036305e9670f7e85b1c3ca6270bf542d001cb4d4b834f`  
		Last Modified: Thu, 21 Oct 2021 23:54:33 GMT  
		Size: 188.5 MB (188457307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
