## `openjdk:22-ea-bookworm`

```console
$ docker pull openjdk@sha256:990627b3c1154dc40b264895dfe2da2e5b37673c38114f543f19e1f469d89f36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:22-ea-bookworm` - linux; amd64

```console
$ docker pull openjdk@sha256:38bd62e2e0d9ff99bae03ac2ef8c29dc65fd3ffa1302e99924d83af526c4766f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.3 MB (360346214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:347dd838f03481926a45b8023071e4de4311f79175cec1bdda3c55cb879111eb`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:37 GMT
ADD file:1e4dd5dab602337b5d5ef8d84b8dbe8b1ac62225f077b29b27d045842486d8e2 in / 
# Wed, 11 Oct 2023 18:34:37 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:19:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:19:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 13:58:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 13:58:42 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Thu, 12 Oct 2023 13:58:42 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 13:58:42 GMT
ENV LANG=C.UTF-8
# Sat, 28 Oct 2023 00:37:29 GMT
ENV JAVA_VERSION=22-ea+21
# Sat, 28 Oct 2023 00:37:39 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/21/GPL/openjdk-22-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='cefe6f9697801dd2a7abebdbd5b7bd36ad489794589e838562da46bde434ae5e'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/21/GPL/openjdk-22-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='b77e7f170973c91690aa64a028f2e991828fde5092eabc29b602e26824216797'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 28 Oct 2023 00:37:40 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:0a9573503463fd3166b5b1f34a7720dac28609e98d731e50e7068f92e79b8545`  
		Last Modified: Wed, 11 Oct 2023 18:39:10 GMT  
		Size: 49.6 MB (49582224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccc26d841b4acc2562483bf393ce1cf8bc358ced09ccd825425226827c79c92`  
		Last Modified: Thu, 12 Oct 2023 03:28:45 GMT  
		Size: 24.1 MB (24051259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800d84653581fc119cd75cd572fa190d3b813d49221b9e5ee463e3560e2cb342`  
		Last Modified: Thu, 12 Oct 2023 03:29:04 GMT  
		Size: 64.1 MB (64130287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc5a642a701433b4f9473abb5932a8cb41a3b21a8ecb44308c2bd1937f64696`  
		Last Modified: Thu, 12 Oct 2023 14:00:13 GMT  
		Size: 17.0 MB (16951780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3d8779495b540b76205a1e83895ce97981c351347c888e9fc375462d638852`  
		Last Modified: Sat, 28 Oct 2023 00:40:34 GMT  
		Size: 205.6 MB (205630664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-ea-bookworm` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:bf8191971d76eaef5cbe5714869ff4c6250849dd3ebbac9458e9ec8dd9fbc885
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.8 MB (358766779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4af9d4efecc1f1d89428c12dccc834f0b97f8c62dae9c364cf06a8c65ade66b`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:43 GMT
ADD file:bf4264671bd91eb30c67d512144ebcf7f5c55a3e490ebe7876fa9b20d433bf7b in / 
# Wed, 11 Oct 2023 18:24:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:44:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:45:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:49:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:49:44 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Wed, 11 Oct 2023 22:49:44 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 22:49:44 GMT
ENV LANG=C.UTF-8
# Sat, 28 Oct 2023 00:37:29 GMT
ENV JAVA_VERSION=22-ea+21
# Sat, 28 Oct 2023 00:37:37 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/21/GPL/openjdk-22-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='cefe6f9697801dd2a7abebdbd5b7bd36ad489794589e838562da46bde434ae5e'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/21/GPL/openjdk-22-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='b77e7f170973c91690aa64a028f2e991828fde5092eabc29b602e26824216797'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 28 Oct 2023 00:37:39 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e720f94321d63ecb6efa873b294dce7eaa1c3a5ddcd5bf7daddf375b955669a4`  
		Last Modified: Wed, 11 Oct 2023 18:28:04 GMT  
		Size: 49.6 MB (49612578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7541d83e7b8c0f5f6cacacddfcf5fdd942793f13418bc4645203b4ab4f3de3`  
		Last Modified: Wed, 11 Oct 2023 19:53:48 GMT  
		Size: 23.6 MB (23588086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a653d69b7b96df6835b157d043d7b926f776531e96c9263f4c7dae0033514d`  
		Last Modified: Wed, 11 Oct 2023 19:54:07 GMT  
		Size: 64.0 MB (63994319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de154cc53d72c8ff61e89ed76922abeb9188c1820dc7d0257c0459d92f3bd1a`  
		Last Modified: Wed, 11 Oct 2023 22:51:51 GMT  
		Size: 17.7 MB (17733456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e8e67b3fc822fa1bd3c7651eac0bb61727f64fb4ec3fdf735254d1483d18a0`  
		Last Modified: Sat, 28 Oct 2023 00:40:28 GMT  
		Size: 203.8 MB (203838340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
