## `openjdk:20-jdk-buster`

```console
$ docker pull openjdk@sha256:d312297b423510d7e5c301f595fc53a01f2a6de1245eb2fbf0042de84f459256
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-jdk-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:9811d67dad34f7d0c9a31afe9ecfb5014c8360b77d628c275a325a192d4ebdf9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.4 MB (331366801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d062b08080838200872e5c3253820792e404422702ab13ebddb0e884b395584b`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:00 GMT
ADD file:d420ffdf63082e03517284553796e5a100e425201458860f07b1aa8598c5929a in / 
# Tue, 23 Aug 2022 00:21:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:49:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:49:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:49:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:30:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:30:03 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 23 Aug 2022 04:30:03 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 04:30:03 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 04:30:03 GMT
ENV JAVA_VERSION=20-ea+11
# Tue, 23 Aug 2022 04:30:14 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/11/GPL/openjdk-20-ea+11_linux-x64_bin.tar.gz'; 			downloadSha256='9a0afe9f1c3ef50968060fe8d70d7b27d93b5515479846193de809127f0d427f'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/11/GPL/openjdk-20-ea+11_linux-aarch64_bin.tar.gz'; 			downloadSha256='d7e80f5000f66440c34073bdb0e443b941ef11209ca30f0e698f07a3fce08118'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 23 Aug 2022 04:30:15 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:76dff75df4d9dbdf29a4459adaec745740bfb476cd915906e33eddd9cd94db93`  
		Last Modified: Tue, 23 Aug 2022 00:25:20 GMT  
		Size: 50.4 MB (50440273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8c90a1c4bb422a88cc9ff532712db3c6a7a8cdc5030af2e60ec51947f2c8aa`  
		Last Modified: Tue, 23 Aug 2022 00:56:49 GMT  
		Size: 7.9 MB (7856913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3662c1050803c4e17c1848dffe636eae5e6e5aafb8f1fffcf82248ccfef21c2`  
		Last Modified: Tue, 23 Aug 2022 00:56:49 GMT  
		Size: 10.0 MB (9998130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5dcb7dd59206e662084addf318ef296595c82800a9107e362439db4c158df9`  
		Last Modified: Tue, 23 Aug 2022 00:57:06 GMT  
		Size: 51.8 MB (51843805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b41608ebffcfb87bcec612e78548c51c5fd92ed1605a2f36089ab6dc0e1ebc0`  
		Last Modified: Tue, 23 Aug 2022 04:37:20 GMT  
		Size: 13.9 MB (13921555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8ea89f169093d0ff59d7bece776978e4bcb0ba72107900506d9b9fe0d81228`  
		Last Modified: Tue, 23 Aug 2022 04:37:33 GMT  
		Size: 197.3 MB (197306125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-jdk-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:8fb78650cdda743d780fda60b49b85190c53483ac9c3f1b045a236659e864d92
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.4 MB (329402170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18ff3aa6aaeeaa2dcad81be00b5c63b4f6cde45fe4d74e0929c8665fd0136e24`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:43 GMT
ADD file:a3ba1802e6680a14c605fbe754f9fb56a642f0799f51ce0010d253cb66c9691f in / 
# Tue, 23 Aug 2022 01:52:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:29:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:29:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 05:17:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 05:17:04 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 23 Aug 2022 05:17:04 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 05:17:05 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 05:17:06 GMT
ENV JAVA_VERSION=20-ea+11
# Tue, 23 Aug 2022 05:17:19 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/11/GPL/openjdk-20-ea+11_linux-x64_bin.tar.gz'; 			downloadSha256='9a0afe9f1c3ef50968060fe8d70d7b27d93b5515479846193de809127f0d427f'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/11/GPL/openjdk-20-ea+11_linux-aarch64_bin.tar.gz'; 			downloadSha256='d7e80f5000f66440c34073bdb0e443b941ef11209ca30f0e698f07a3fce08118'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 23 Aug 2022 05:17:19 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3332e5c67ba650c61dbca801cf2739a1f5b6faac33f7b0543f97f4ab1165fe69`  
		Last Modified: Tue, 23 Aug 2022 01:58:23 GMT  
		Size: 49.2 MB (49228066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61dd9df5607d27eb8d7af8db0ec4f1e1634f54db08cd06c03131ac8a25ff710b`  
		Last Modified: Tue, 23 Aug 2022 02:38:02 GMT  
		Size: 7.7 MB (7720187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28122dfd7d7cf006c384197d918567d3d812f94f0030b87104b26c2d2ded69a`  
		Last Modified: Tue, 23 Aug 2022 02:38:02 GMT  
		Size: 9.8 MB (9768739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e3536e0d6df43cb88858e2f77eaa514bd51e583a6d593d494fcb67e03bfda1`  
		Last Modified: Tue, 23 Aug 2022 02:38:21 GMT  
		Size: 52.2 MB (52174764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246a2f5e9cf744fdddb945099efc2014170988f6754c19802f33155206860374`  
		Last Modified: Tue, 23 Aug 2022 05:28:44 GMT  
		Size: 14.7 MB (14670863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7492ff06b8cb88633eb8df72b2384f96a05cc279b9b0884ee7519072a636cfc2`  
		Last Modified: Tue, 23 Aug 2022 05:29:00 GMT  
		Size: 195.8 MB (195839551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
