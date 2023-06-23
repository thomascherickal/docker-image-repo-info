## `openjdk:21-ea-28-bookworm`

```console
$ docker pull openjdk@sha256:b623f04e870c20ee1a341482eb4a1499c4e79197efbf2d3844ce91e566ee2bd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `openjdk:21-ea-28-bookworm` - linux; amd64

```console
$ docker pull openjdk@sha256:2e85c8cedcff8447e28cf81546bff5c898fc219b95b1331cffa951663ba80ab1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.6 MB (358611097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c3529d4e3add187e69b31f899de1c4aa6217e654198c4faa7d92a0cbe57a238`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:28 GMT
ADD file:98cacc5890a8c0b29d7a2b296774428cb2268b01b4ff97a84deadcd3b513f319 in / 
# Mon, 12 Jun 2023 23:20:29 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:26:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:27:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:42:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:43:06 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Tue, 13 Jun 2023 18:43:06 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 18:43:06 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jun 2023 00:27:54 GMT
ENV JAVA_VERSION=21-ea+28
# Fri, 23 Jun 2023 00:28:04 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/28/GPL/openjdk-21-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='c5ff4dc462286ead4a7f1480719f695a976a130005df30d33ba210aadc094ff9'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/28/GPL/openjdk-21-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='4f98a729913be1d28fda8491420394e394fbbf84c4d1f41f05b83ba4c8b989aa'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 23 Jun 2023 00:28:04 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bba7bb10d5baebcaad1d68ab3cbfd37390c646b2a688529b1d118a47991116f4`  
		Last Modified: Mon, 12 Jun 2023 23:25:26 GMT  
		Size: 49.6 MB (49552112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2b820b8e87758dde67c29b25d4cbf88377601a4355cc5d556a9beebc80da00`  
		Last Modified: Tue, 13 Jun 2023 03:36:28 GMT  
		Size: 24.0 MB (24030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284f2345db055020282f6e80a646f1111fb2d5dfc6f7ee871f89bc50919a51bf`  
		Last Modified: Tue, 13 Jun 2023 03:36:47 GMT  
		Size: 64.1 MB (64111555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9350d4cb97cd74af4173b0a47cb308cd97cec7c6d33e7f66f37adf410f7b5d31`  
		Last Modified: Tue, 13 Jun 2023 18:44:35 GMT  
		Size: 16.9 MB (16947115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29366366296150b2fe30a720200d5c95cb854cebd93dc7e3fc8b410bfd2a7072`  
		Last Modified: Fri, 23 Jun 2023 00:34:43 GMT  
		Size: 204.0 MB (203969776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
