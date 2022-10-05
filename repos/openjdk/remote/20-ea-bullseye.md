## `openjdk:20-ea-bullseye`

```console
$ docker pull openjdk@sha256:eeda11e387f84053eb826231db391339cedb3e6a4964d77e6e2a01e26c98822a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:85357827a49b99f2f881edced41c851eafcb6fa3e2a4b65c13048f2fa3de9b2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.8 MB (336750880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7584b8acce82ad1547901ae9d7b8bfda3413945e22db282012f12fb445ad8fab`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:27 GMT
ADD file:d1268789456d2cdace6e50149e60404ad5a849b7c61e8fc8bc7b6e0eb6eeb7ca in / 
# Tue, 04 Oct 2022 23:26:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:54:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:55:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:55:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:00:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Wed, 05 Oct 2022 13:00:41 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 13:00:41 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:00:41 GMT
ENV JAVA_VERSION=20-ea+17
# Wed, 05 Oct 2022 13:00:53 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/17/GPL/openjdk-20-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='9d46acb0892a134f62ab21fca33fdef1da5d579f61ddbd0ae3ff0b4d33c5eca2'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/17/GPL/openjdk-20-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='31245b15195bf9f12a6db08474bfcbd1ddbccc76436372bf4db538c6ede8f976'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 05 Oct 2022 13:00:54 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f606d8928ed378229f2460b94b504cca239fb906efc57acbdf9340bd298d5ddf`  
		Last Modified: Tue, 04 Oct 2022 23:30:27 GMT  
		Size: 55.0 MB (55046248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47db815c6a4547dc224b75222193cb1851cf529d2cbdf26f854b9bbf97099b98`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 5.2 MB (5163279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf48494000001a037b72870d2a6a2536f9da8bc5d1ceddd72d79f4a51fe7a60e`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 10.9 MB (10876505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a572f7a256d36a93ab0777949771b120c5d7dce75ea2a2d3d9444793b26b2ef1`  
		Last Modified: Wed, 05 Oct 2022 01:19:34 GMT  
		Size: 54.6 MB (54584293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec9184f949d7424381e024c08a4940ffa66da77a6cd8aaa1d9374b7f366f561`  
		Last Modified: Wed, 05 Oct 2022 13:05:37 GMT  
		Size: 14.1 MB (14071819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfd6bccfa9e7252d34e8c333006148e37a02d69a708754d357be77f7a17026a`  
		Last Modified: Wed, 05 Oct 2022 13:05:49 GMT  
		Size: 197.0 MB (197008736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:373b05edf497c0f54b63d6bcccb0831a6c672eefa7db1a862b40e0fe4d395288
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.1 MB (335085243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc1ae86c9febc3aeb48f0467164138c119edcb82b795a7f0d34ad36c02088bf7`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:26 GMT
ADD file:59bc45fad9cada77bf8e44ebdd982c7f6e575816b5ed6b7d1d8494faddd9b8b9 in / 
# Tue, 04 Oct 2022 23:44:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:23:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:23:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:23:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:25:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:26:00 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Wed, 05 Oct 2022 04:26:01 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 04:26:02 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 04:26:03 GMT
ENV JAVA_VERSION=20-ea+17
# Wed, 05 Oct 2022 04:26:22 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/17/GPL/openjdk-20-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='9d46acb0892a134f62ab21fca33fdef1da5d579f61ddbd0ae3ff0b4d33c5eca2'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/17/GPL/openjdk-20-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='31245b15195bf9f12a6db08474bfcbd1ddbccc76436372bf4db538c6ede8f976'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 05 Oct 2022 04:26:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:172730635f67c8f081f43275b390514bd8a05a4a7c3c467ae74ee42a029dce2b`  
		Last Modified: Tue, 04 Oct 2022 23:49:51 GMT  
		Size: 53.7 MB (53700625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37c953a37e989b49a533e8d08c80d87ce66fadee48160f9a4d8cd2dd5b0ec87`  
		Last Modified: Wed, 05 Oct 2022 00:37:21 GMT  
		Size: 4.9 MB (4944361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98802a15fc60bda24c79203236f930586f1dba6218aa2b4c121cf0dbf5627b38`  
		Last Modified: Wed, 05 Oct 2022 00:37:22 GMT  
		Size: 10.7 MB (10657400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aff223bb11e201213e82ed9838541b6a63fd9276370f73ed0dbdd6efd73e32a`  
		Last Modified: Wed, 05 Oct 2022 00:37:44 GMT  
		Size: 54.7 MB (54681658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cd1b7c124d493606efa74bb734facd3be5b8f2603628d9c24fda9b146dd616`  
		Last Modified: Wed, 05 Oct 2022 04:34:43 GMT  
		Size: 15.5 MB (15527320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2cc9b34457dd5b83f5b1868327c61506b7a7afcbef4f30b859c811eef9f818`  
		Last Modified: Wed, 05 Oct 2022 04:35:01 GMT  
		Size: 195.6 MB (195573879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
