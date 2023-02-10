## `openjdk:21-ea-9-jdk-bullseye`

```console
$ docker pull openjdk@sha256:81f2172fbdb5565b81a9859725c03069ab4ccd283bdb605727d841f2684ff31d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `openjdk:21-ea-9-jdk-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:36cae01f92da9b0aac0b4a66a6554eee8f0139f56a04b01fb48f0eca198d53ac
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.8 MB (337766114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c90bdf9c3f7e9d8c9f5b562c001d9ea33e96c700b0739c087e4b0785002f820`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:08:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 09:08:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:07:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:07:30 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Thu, 09 Feb 2023 10:07:30 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 10:07:30 GMT
ENV LANG=C.UTF-8
# Fri, 10 Feb 2023 01:57:04 GMT
ENV JAVA_VERSION=21-ea+9
# Fri, 10 Feb 2023 01:57:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/9/GPL/openjdk-21-ea+9_linux-x64_bin.tar.gz'; 			downloadSha256='50ce8bd2e9b710726e7117ba3a302287a0be51cb187721a422ee63cadbf717a2'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/9/GPL/openjdk-21-ea+9_linux-aarch64_bin.tar.gz'; 			downloadSha256='86f137227e32994689e70b0a2f426adb45a16807bc84398926e841452cfe83d0'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 10 Feb 2023 01:57:15 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae98695cf4875b92116a031bcf51736705c39b105be5f240a143935d8370f6`  
		Last Modified: Thu, 09 Feb 2023 09:14:20 GMT  
		Size: 5.2 MB (5152064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a74e69230a5d5ee55fb6baca6fb52404417efd177a2cb03c418d2d0cf599b5`  
		Last Modified: Thu, 09 Feb 2023 09:14:21 GMT  
		Size: 10.9 MB (10873498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e04cd4cd2ee5f2d53ea296fb22e3875a699f2ee5426c8908bfc38728acfb10a`  
		Last Modified: Thu, 09 Feb 2023 09:14:38 GMT  
		Size: 54.7 MB (54679990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8d0649ccd12c8208946367b5bd589be9432ea49700dd78f9f2b69e21c55fec`  
		Last Modified: Thu, 09 Feb 2023 10:14:13 GMT  
		Size: 15.5 MB (15528993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954a73457c3a6cb79bfafa4085883cac6602a3fea6f9fda5e1ef4437004a19dc`  
		Last Modified: Fri, 10 Feb 2023 02:04:09 GMT  
		Size: 197.8 MB (197828201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
