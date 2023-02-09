## `openjdk:21-jdk-bullseye`

```console
$ docker pull openjdk@sha256:483a900624a0c57a92335e006c4562e9ea50ef9f8af8760dc338f517d7252ce4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-jdk-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:bd2b4ce95247df06b97b754f331358049a4dcbda352a48b3e3db4a2f26755913
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.1 MB (339099806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd57b9237cbad36a8d7cfacd85ccaf7fd64a9c8b98cb53b32d31520c41397943`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:10:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:10:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 09:11:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:46:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:46:56 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Thu, 09 Feb 2023 10:46:56 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 10:46:56 GMT
ENV LANG=C.UTF-8
# Thu, 09 Feb 2023 10:46:56 GMT
ENV JAVA_VERSION=21-ea+8
# Thu, 09 Feb 2023 10:47:10 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/8/GPL/openjdk-21-ea+8_linux-x64_bin.tar.gz'; 			downloadSha256='ce77e229b2dc811e1231ab1197f851d3234e56cb9e9a26e9f1d7c0294eb09af8'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/8/GPL/openjdk-21-ea+8_linux-aarch64_bin.tar.gz'; 			downloadSha256='c52c76023ce2b7202744161d92772f5bc21c6ada643b926c92d5a56b0d1c4664'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 09 Feb 2023 10:47:11 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1024729feeb2893dad43684fe7679c4d866c3640dfc3912bbd93c5a51f32d2`  
		Last Modified: Thu, 09 Feb 2023 09:17:56 GMT  
		Size: 5.2 MB (5165984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3aa11fbc85a2a9660c98cfb4d0a2db8cde983ce3c87565c356cfdf1ddf2654c`  
		Last Modified: Thu, 09 Feb 2023 09:17:56 GMT  
		Size: 10.9 MB (10876805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa54add66b3a47555c8b761f60b15f818236cc928109a30032111efc98c6fcd4`  
		Last Modified: Thu, 09 Feb 2023 09:18:15 GMT  
		Size: 54.6 MB (54587652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424a482a242625bf23d28ac754f5a65ffc1365d58a9c2f254bb8403169077fe0`  
		Last Modified: Thu, 09 Feb 2023 10:53:37 GMT  
		Size: 14.1 MB (14072070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28814134fff80be45423a9b4487e78c95f07ed0d9ab85b9b7e75774b0f3e15a7`  
		Last Modified: Thu, 09 Feb 2023 10:53:49 GMT  
		Size: 199.4 MB (199350524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-jdk-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:3e6a09bb6aef0be9dc12e0c2ad675577d18c3f27618f48902e980e40770df3a6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.8 MB (337753919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cae96c1745aa98e454e87299adcb8ab6ae2a659ef5326f18ccd4f0812b592553`
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
# Thu, 09 Feb 2023 10:07:30 GMT
ENV JAVA_VERSION=21-ea+8
# Thu, 09 Feb 2023 10:07:43 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/8/GPL/openjdk-21-ea+8_linux-x64_bin.tar.gz'; 			downloadSha256='ce77e229b2dc811e1231ab1197f851d3234e56cb9e9a26e9f1d7c0294eb09af8'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/8/GPL/openjdk-21-ea+8_linux-aarch64_bin.tar.gz'; 			downloadSha256='c52c76023ce2b7202744161d92772f5bc21c6ada643b926c92d5a56b0d1c4664'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 09 Feb 2023 10:07:45 GMT
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
	-	`sha256:cf0fe246f205865eef3e701e4586a41752e412ae62f448f0e21650324e79e7de`  
		Last Modified: Thu, 09 Feb 2023 10:14:23 GMT  
		Size: 197.8 MB (197816006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
