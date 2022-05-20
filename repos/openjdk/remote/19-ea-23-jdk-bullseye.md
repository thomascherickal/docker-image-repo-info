## `openjdk:19-ea-23-jdk-bullseye`

```console
$ docker pull openjdk@sha256:0d485519dc24fb845dfb4cf40839cd3ba1c355d088f251f5822926eee479fe1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `openjdk:19-ea-23-jdk-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:f10dc05e9a891786ef9cc67be0417fa9853708f0d2e224d417e7047357c63e60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.1 MB (334078156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88a64420634073c780cd12fee1acd7372569bd598ff444c788f7a3b33684f401`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 11 May 2022 00:46:44 GMT
ADD file:239aa42118877a929b2fbfc0d5793fee7815289280affa5286de2459385c0679 in / 
# Wed, 11 May 2022 00:46:44 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:25:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:25:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:25:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:15:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:15:31 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Wed, 11 May 2022 14:15:32 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 14:15:33 GMT
ENV LANG=C.UTF-8
# Fri, 20 May 2022 21:04:19 GMT
ENV JAVA_VERSION=19-ea+23
# Fri, 20 May 2022 21:04:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/23/GPL/openjdk-19-ea+23_linux-x64_bin.tar.gz'; 			downloadSha256='37187e2eecb64237757cf5d5b2c7a94b25d2b03f3ea5b12bf77a5fe8b1508ac4'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/23/GPL/openjdk-19-ea+23_linux-aarch64_bin.tar.gz'; 			downloadSha256='ad7e6c255a6a0fcb02b05a879036c1d3029693c577b7cc97323f7e43901e48e7'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 20 May 2022 21:04:31 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3a36574378e6cece2dd3a839e1c0220eaccc4063b61d7481d1a19d3990c1f2c2`  
		Last Modified: Wed, 11 May 2022 00:53:15 GMT  
		Size: 53.6 MB (53634337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61d3345afba43846f3e638752cce2f0d1d47b21cc667ba08b00db10767a4702`  
		Last Modified: Wed, 11 May 2022 01:35:45 GMT  
		Size: 4.9 MB (4938615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e267d6aa58f93a513352a3b46c7addbf9335d7d43bfa4f1df4026d21785181c`  
		Last Modified: Wed, 11 May 2022 01:35:46 GMT  
		Size: 10.7 MB (10656992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f647907d26b879e0d43f6f4f0807f01e4dbdc034edcecbc988f6033cf401becf`  
		Last Modified: Wed, 11 May 2022 01:36:07 GMT  
		Size: 54.7 MB (54672822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b8129a4eda877bb83fd5fc2f5f0629e387ba37e1fd0eaa0b8ebbaec9d30779`  
		Last Modified: Wed, 11 May 2022 14:33:06 GMT  
		Size: 15.5 MB (15526030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5636bad0b71345a705794523a2db90be23dfe53681780504ebb382a99e1bb61a`  
		Last Modified: Fri, 20 May 2022 21:18:09 GMT  
		Size: 194.6 MB (194649360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
