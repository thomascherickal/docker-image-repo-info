## `openjdk:22-ea-jdk-bullseye`

```console
$ docker pull openjdk@sha256:4de2c93c38a0c869b043a63d4714e8353df555075885c45dcea71896ee65dd3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:22-ea-jdk-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:2612ccc79c2cfb392611e86eac4941140595ac5e9818c8c447b1467efa0f7ef0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.4 MB (344378777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97fe42cf00c680bd14faa52e96d66441c8d3b34f3f759c0881cd04673e8ed630`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:02:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:09:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:09:22 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Fri, 28 Jul 2023 04:09:22 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 04:09:22 GMT
ENV LANG=C.UTF-8
# Sat, 12 Aug 2023 00:03:27 GMT
ENV JAVA_VERSION=22-ea+10
# Sat, 12 Aug 2023 00:03:40 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/10/GPL/openjdk-22-ea+10_linux-x64_bin.tar.gz'; 			downloadSha256='aa3e45c81e7269d389411b52c17721916d2acb7d3e7ab6367c62138063f5052b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/10/GPL/openjdk-22-ea+10_linux-aarch64_bin.tar.gz'; 			downloadSha256='e143f6323650bd4747e4304ef07ba80ade1510a71325bc36a7c4f51939cfe423'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Aug 2023 00:03:41 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd6a2c0cfa3eb4e8012b3f2df526acc8711a4a9515e0e968419a8ab1e9899e4`  
		Last Modified: Fri, 28 Jul 2023 03:08:40 GMT  
		Size: 54.6 MB (54585034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28bfe4d14b6484ed32c77d146385c72ef90db4a661c6c0e87429110ac5eba9a`  
		Last Modified: Fri, 28 Jul 2023 04:13:30 GMT  
		Size: 14.1 MB (14072137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5360e8c34753505b77db6784c5525800a388974a5f0a8d42f9952fc109edf569`  
		Last Modified: Sat, 12 Aug 2023 00:09:22 GMT  
		Size: 204.9 MB (204905450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-ea-jdk-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:2bfe8fb57f09c2c4d8cc1d1a2e804782e0009b3846d1bd937875355dcba6d3d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.9 MB (342942668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bdc431b3290ccb3bcb1db2f5bbcd69e7b2193f739b91838e2efc9ea1542da53`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:07 GMT
ADD file:a0144d077c2c6b73bbb5f7e7b8e6b58e4127de2a5faf907cd4e83e4d83437fad in / 
# Thu, 27 Jul 2023 23:43:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:37:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:37:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 10:41:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 10:41:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Fri, 28 Jul 2023 10:41:11 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 10:41:11 GMT
ENV LANG=C.UTF-8
# Fri, 04 Aug 2023 00:58:39 GMT
ENV JAVA_VERSION=22-ea+9
# Fri, 04 Aug 2023 00:58:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/9/GPL/openjdk-22-ea+9_linux-x64_bin.tar.gz'; 			downloadSha256='dd11f0f96ed6992b56452eee0683b50f1b550f74c31fb39e1eb1ff8a232caf68'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/9/GPL/openjdk-22-ea+9_linux-aarch64_bin.tar.gz'; 			downloadSha256='47ab1fb3cbe8174c21e10880e5de0c60d754cf5ba6d5cdfbe1a1d91b53b193bc'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 04 Aug 2023 00:58:52 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:49185a1a3bc353699370ac57d50a7b7234b59616b6aebde79ba6a0a0314bb107`  
		Last Modified: Thu, 27 Jul 2023 23:46:34 GMT  
		Size: 53.7 MB (53704790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f6f6b31000e991bdd81caebc21e281fc1350f09586d393f3b8bf36dceeb99e`  
		Last Modified: Fri, 28 Jul 2023 01:42:56 GMT  
		Size: 15.7 MB (15746528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385ee361272e1c36fe7d96fe8ab6b0f30cf33bfb9bbe29bfc2d33f51bd771993`  
		Last Modified: Fri, 28 Jul 2023 01:43:10 GMT  
		Size: 54.7 MB (54676175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3685694dfe4a43e9db9358680ffcb69ef3c8ee13df6588581a7bc2d034d0e00`  
		Last Modified: Fri, 28 Jul 2023 10:45:29 GMT  
		Size: 15.5 MB (15529258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c29bb4d9a6cda9e7ab78d3399a6b093b53e283b38310082fb626c9a7756d15`  
		Last Modified: Fri, 04 Aug 2023 01:04:37 GMT  
		Size: 203.3 MB (203285917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
