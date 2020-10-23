## `openjdk:16-jdk-buster`

```console
$ docker pull openjdk@sha256:8e7f0ef45265d41282a800bfdffe41e0f03c931393adbd4b871e497983fef350
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:16-jdk-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:20ed76e084a7b6abd1782eebb8d7e5924d27e2f8d2a32bd4e2e65c500142cb61
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.1 MB (333067936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:255ea4ea79d1a047690c30d69581ed8b6d44e06985f4d51e04540f6e870c0678`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:30 GMT
ADD file:6627ad39ea0cb9fcb212342326d14efaff51aece1fd0dc16d5bbcaa25d858622 in / 
# Tue, 13 Oct 2020 01:38:30 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:14:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:14:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 02:15:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:57:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				binutils 		fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:57:38 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 08:57:38 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Tue, 13 Oct 2020 08:57:38 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 08:57:40 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 22 Oct 2020 23:35:11 GMT
ENV JAVA_VERSION=16-ea+21
# Thu, 22 Oct 2020 23:35:25 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/21/GPL/openjdk-16-ea+21_linux-aarch64_bin.tar.gz; 			downloadSha256=bee09458526a8c10a40f3d4e5bf6c384b1bbc6f9002997d2f4c0d8c090cca1f8; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/21/GPL/openjdk-16-ea+21_linux-x64_bin.tar.gz; 			downloadSha256=3294d805c6125a6dd55a387f82f74df0c9fc0bce06934061fb3ff2dd42075b33; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 22 Oct 2020 23:35:26 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e4c3d3e4f7b024979a1c12daa4073f6353b2ba92d96418bc90451994927c9bff`  
		Last Modified: Tue, 13 Oct 2020 01:48:02 GMT  
		Size: 50.4 MB (50395978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101c41d0463bc77661fb3343235b16d536a92d2efb687046164d413e51bd4fc4`  
		Last Modified: Tue, 13 Oct 2020 02:28:35 GMT  
		Size: 7.8 MB (7811737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8275efcd805f9905d7def23603618236284b0be6b9e47455c638fbfb03fa9208`  
		Last Modified: Tue, 13 Oct 2020 02:28:35 GMT  
		Size: 10.0 MB (9996326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751620502a7a2905067c2f32d4982fb9b310b9808670ce82c0e2b40f5307a3ee`  
		Last Modified: Tue, 13 Oct 2020 02:28:53 GMT  
		Size: 51.8 MB (51829492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f28f646e98144707f2cc19e3ad498b86228306ce9f907e555f8f055d690dd1`  
		Last Modified: Tue, 13 Oct 2020 09:07:43 GMT  
		Size: 13.9 MB (13920357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c897a95d35d1447da4697256d475f3b6e2e93937ff0cadb54fb8553540c76c`  
		Last Modified: Tue, 13 Oct 2020 09:07:40 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b9e313e5d47fdf7b59fd49a32b0a1e762fb9cd2c43afdc4dce0e11604ed534`  
		Last Modified: Thu, 22 Oct 2020 23:41:00 GMT  
		Size: 199.1 MB (199113833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-jdk-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:5b1c2317102450f880e462085e089e00535226813540e1ed272967af61628ad6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.3 MB (311321653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab8bb2551cec39f40c5b66b9aabc86991e2f9b93ad26bdab4a6744b99c0663af`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 13 Oct 2020 01:40:40 GMT
ADD file:7a9016f6c75910c392bbea2cb9e146d1eba3942cdfd666a44004c79951c5d46f in / 
# Tue, 13 Oct 2020 01:40:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:32:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:33:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 02:33:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 12:23:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				binutils 		fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 12:23:16 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 12:23:17 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Tue, 13 Oct 2020 12:23:17 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 12:23:19 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 22 Oct 2020 22:49:25 GMT
ENV JAVA_VERSION=16-ea+21
# Thu, 22 Oct 2020 22:49:43 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/21/GPL/openjdk-16-ea+21_linux-aarch64_bin.tar.gz; 			downloadSha256=bee09458526a8c10a40f3d4e5bf6c384b1bbc6f9002997d2f4c0d8c090cca1f8; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/21/GPL/openjdk-16-ea+21_linux-x64_bin.tar.gz; 			downloadSha256=3294d805c6125a6dd55a387f82f74df0c9fc0bce06934061fb3ff2dd42075b33; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 22 Oct 2020 22:49:45 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:04aacb10cb67f5fa248646a0ac9f40af5a6d3b0dbef65505bb7766bed6bf4885`  
		Last Modified: Tue, 13 Oct 2020 01:47:53 GMT  
		Size: 49.2 MB (49175405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136d6e4f4b17bdbefbe60820da5f5711a26d31c075dc69bcaf9b077d7d29262d`  
		Last Modified: Tue, 13 Oct 2020 02:47:32 GMT  
		Size: 7.7 MB (7681432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28db65b8364fc73072a0d5b51199cc9c6b108b4229d92e784b92ae67898dd0bd`  
		Last Modified: Tue, 13 Oct 2020 02:47:32 GMT  
		Size: 10.0 MB (9983936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff74fb95e95674d2f0c26f446a2cb7c0ee055d78182a9d61e1578c64c171f2b4`  
		Last Modified: Tue, 13 Oct 2020 02:48:00 GMT  
		Size: 52.2 MB (52163324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbd3ea57013c00ec3468c25b1885278bbd9f62b7240044251733b502bf621e5`  
		Last Modified: Tue, 13 Oct 2020 12:33:14 GMT  
		Size: 14.7 MB (14674162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669285db2797a08b2f857538eeb8d14e2fe14d0d5f38acbec74091b9fda4189f`  
		Last Modified: Tue, 13 Oct 2020 12:33:10 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0e91238814b4e4c24b0b7fe3d0d551229464ba7230b55773c513e478e0677b`  
		Last Modified: Thu, 22 Oct 2020 22:56:13 GMT  
		Size: 177.6 MB (177643184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
