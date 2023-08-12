## `openjdk:21-rc-bookworm`

```console
$ docker pull openjdk@sha256:467cf30aa827badd94f148f14fb45ecb94f171ec7b780d76777fc21c0dfe6412
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `openjdk:21-rc-bookworm` - linux; amd64

```console
$ docker pull openjdk@sha256:1ef3ee7065e8e9b18ff85694ff036558cb9be30c9476db28ec6b1650af3a73a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.7 MB (358698786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70b2c78aa9d3837ac42ee0468592805cb75bebda504323c421b4761e46142235`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:29 GMT
ADD file:cc1376ecb3d9e93e4160573c110da753ffeb2efe2223351f1fbf483d89f1a756 in / 
# Thu, 27 Jul 2023 23:24:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:01:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:10:03 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Fri, 28 Jul 2023 04:10:03 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 04:10:03 GMT
ENV LANG=C.UTF-8
# Sat, 12 Aug 2023 00:04:31 GMT
ENV JAVA_VERSION=21
# Sat, 12 Aug 2023 00:04:41 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_linux-x64_bin.tar.gz'; 			downloadSha256='a30c454a9bef8f46d5f1bf3122830014a8fbe7ac03b5f8729bc3add4b92a1d0a'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_linux-aarch64_bin.tar.gz'; 			downloadSha256='e8f4ed1a69815ddf56d7da365116eefc1e5a1159396dffee3dd21616a86d5d28'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Aug 2023 00:04:41 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:785ef8b9b236a5f027f33cae77513051704c0538bff455ff5548105c954c3b1c`  
		Last Modified: Thu, 27 Jul 2023 23:29:02 GMT  
		Size: 49.6 MB (49557354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6dad8f55ae6c733e986316bd08205c8b2c41640bf8d08ff6e9bbcb6884304f`  
		Last Modified: Fri, 28 Jul 2023 03:07:18 GMT  
		Size: 24.0 MB (24030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd36c7bfe5f4bdffcc0bbb74b0fb38feb35c286ea58b5992617fb38b0c933603`  
		Last Modified: Fri, 28 Jul 2023 03:07:36 GMT  
		Size: 64.1 MB (64112293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23081abc6d37ce8cde709fa970343e4a97f93dc71c081510386ac63a6804ae7f`  
		Last Modified: Fri, 28 Jul 2023 04:12:13 GMT  
		Size: 16.9 MB (16947358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be17df41c4ec9fa124df4d53193f6ee07e2bb91cc0fbba3a489d650c000804b`  
		Last Modified: Sat, 12 Aug 2023 00:11:39 GMT  
		Size: 204.1 MB (204051242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
