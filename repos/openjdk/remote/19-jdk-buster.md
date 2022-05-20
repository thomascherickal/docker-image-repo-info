## `openjdk:19-jdk-buster`

```console
$ docker pull openjdk@sha256:195b9f709eb6a8fa63f28ea53019f6f570fdd6b9b0802f87108cdad9756e5ff7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-jdk-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:a517ad17db61250444187094c120a54b1a433c953a34b603847cf0f75e9cc341
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.8 MB (329813611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4467641b6e2eb033021e4ea6b58e37086c972732f6088c9c688d0e883108856`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 11 May 2022 01:20:26 GMT
ADD file:54d60144d251caa916ff50606bc2364131d47d6b10ed83d08c81c647ab56cc40 in / 
# Wed, 11 May 2022 01:20:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:50:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:50:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:50:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:47:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:47:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Wed, 11 May 2022 05:47:15 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 05:47:15 GMT
ENV LANG=C.UTF-8
# Fri, 20 May 2022 21:43:35 GMT
ENV JAVA_VERSION=19-ea+23
# Fri, 20 May 2022 21:43:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/23/GPL/openjdk-19-ea+23_linux-x64_bin.tar.gz'; 			downloadSha256='37187e2eecb64237757cf5d5b2c7a94b25d2b03f3ea5b12bf77a5fe8b1508ac4'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/23/GPL/openjdk-19-ea+23_linux-aarch64_bin.tar.gz'; 			downloadSha256='ad7e6c255a6a0fcb02b05a879036c1d3029693c577b7cc97323f7e43901e48e7'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 20 May 2022 21:43:45 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b03a94565ecb6e02edf716307f25a0ea5090e3e2f7acec6a3687b95415378a30`  
		Last Modified: Wed, 11 May 2022 01:25:33 GMT  
		Size: 50.4 MB (50437966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7bcede80b1916d73be58ae0a2af8321770c4ce0c8ada05c39271e292355325`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 7.9 MB (7856436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37471fc83c2dc382a8aec5dc1c1f0f2f8156f4df529cd1aea7647cbaee4b25fa`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 10.0 MB (9997259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0162432a49c07aa492d3e1031af58a9a9f9b22acde859829434e5a54d019aa1c`  
		Last Modified: Wed, 11 May 2022 01:58:46 GMT  
		Size: 51.8 MB (51843657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c991e290c00eaf78c3b16a504803042009e8ab196f4d572d415dc6916274f0c2`  
		Last Modified: Wed, 11 May 2022 05:59:23 GMT  
		Size: 13.9 MB (13921435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f327c5160edaa1fe1585c92c8f4fe33a650bdc4b8059910703196afc943b25a0`  
		Last Modified: Fri, 20 May 2022 21:51:57 GMT  
		Size: 195.8 MB (195756858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-jdk-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:db6b2672f771ba52bd4daadcdb4cce91689b8949242f92a90dda0a843cfc16ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.2 MB (328218150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:860deeee571b88d941ef2cdfe2858b77f8ef3ea1dcd33fd7b2e77c4e873e4cde`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 11 May 2022 00:47:11 GMT
ADD file:5389b77733b44ebc41850baff3ebfc491726af264a745f108d5f16076a0f04ab in / 
# Wed, 11 May 2022 00:47:11 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:26:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:26:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:27:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:16:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:16:31 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Wed, 11 May 2022 14:16:31 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 14:16:32 GMT
ENV LANG=C.UTF-8
# Fri, 20 May 2022 21:05:05 GMT
ENV JAVA_VERSION=19-ea+23
# Fri, 20 May 2022 21:05:16 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/23/GPL/openjdk-19-ea+23_linux-x64_bin.tar.gz'; 			downloadSha256='37187e2eecb64237757cf5d5b2c7a94b25d2b03f3ea5b12bf77a5fe8b1508ac4'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/23/GPL/openjdk-19-ea+23_linux-aarch64_bin.tar.gz'; 			downloadSha256='ad7e6c255a6a0fcb02b05a879036c1d3029693c577b7cc97323f7e43901e48e7'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 20 May 2022 21:05:17 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5528d23e3f315103c99c14258e007a025d09bb4fd587c2d8a32d6dbb6047b891`  
		Last Modified: Wed, 11 May 2022 00:54:09 GMT  
		Size: 49.2 MB (49228300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b2d66a1dbe5960c6de4181ca3512467d3303dfb9cde3d92ecf7a85111cf68b`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 7.7 MB (7719789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9244ac9f9851b43ddc1032930666d339c3a5d9b934e2ca42ecd2e8ef3dd680`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 9.8 MB (9767329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06885dc77f03f05a5f98ceb35e871f027525d932d32027ed9d4ffb0cbd29786c`  
		Last Modified: Wed, 11 May 2022 01:37:21 GMT  
		Size: 52.2 MB (52174787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2119f34492bb8627749583ea25e03ced955c255123d455e6530cea4eba269ee4`  
		Last Modified: Wed, 11 May 2022 14:34:47 GMT  
		Size: 14.7 MB (14670863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdac87ec38de137f3e11f775bd6ab11d88d367b83c97b697696d74d64a80700`  
		Last Modified: Fri, 20 May 2022 21:19:50 GMT  
		Size: 194.7 MB (194657082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
