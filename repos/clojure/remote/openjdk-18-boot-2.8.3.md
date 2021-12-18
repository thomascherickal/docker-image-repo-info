## `clojure:openjdk-18-boot-2.8.3`

```console
$ docker pull clojure@sha256:a0d50b92d8187d900457c399be8268f0eb20a98cc41fb7c87b41371a9bb30e68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-boot-2.8.3` - linux; amd64

```console
$ docker pull clojure@sha256:37d5c13acfe98718904a6ddb22b20d9f56430c86641092b22bddef5193fbd9bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.1 MB (281064835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4a028b035118b4b1b6261779e020f8984bdfa152fe7b24a441430fc30a6d4ce`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:20 GMT
ADD file:ece5ff85ca549f0b1e9139d29dcb43a52af672d0591c423e28180f6d8d700ad7 in / 
# Thu, 02 Dec 2021 02:48:21 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 11:29:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:29:26 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Thu, 02 Dec 2021 11:29:27 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 11:29:27 GMT
ENV LANG=C.UTF-8
# Sat, 18 Dec 2021 04:11:11 GMT
ENV JAVA_VERSION=18-ea+28
# Sat, 18 Dec 2021 04:11:28 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='7e5f0e54c799f8c155a934e61d88f4fef3a70a641c1636c925158622c7bd9341'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='e29aa39763ebcfe5f037cc4fe47c6b9eb34cbe482f6ea57e93de89070255e22b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 18 Dec 2021 04:11:29 GMT
CMD ["jshell"]
# Sat, 18 Dec 2021 06:53:51 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 18 Dec 2021 06:53:51 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 18 Dec 2021 06:53:51 GMT
WORKDIR /tmp
# Sat, 18 Dec 2021 06:53:56 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 18 Dec 2021 06:53:56 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 18 Dec 2021 06:53:56 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 18 Dec 2021 06:54:20 GMT
RUN boot
# Sat, 18 Dec 2021 06:54:21 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Sat, 18 Dec 2021 06:54:21 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 18 Dec 2021 06:54:21 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:e5ae68f740265288a4888db98d2999a638fdcb6d725f427678814538d253aa4d`  
		Last Modified: Thu, 02 Dec 2021 02:53:46 GMT  
		Size: 31.4 MB (31370221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9f5b9b70c2f137dc70e816256e7a568a084d066e7c34c028d30a6a45438685`  
		Last Modified: Thu, 02 Dec 2021 11:47:20 GMT  
		Size: 1.6 MB (1582045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e71fd0564b64594d9d12cfa9a977c2d399df5350dfe24ddecd9dad968e3f197`  
		Last Modified: Sat, 18 Dec 2021 04:24:19 GMT  
		Size: 189.0 MB (189008722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815c53055e063f4a3f8a7d707009c288eef6b911aa3b92b0e50ed7213e4f5e9f`  
		Last Modified: Sat, 18 Dec 2021 07:01:07 GMT  
		Size: 283.0 KB (283043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022c39f6bf2a9602be2ea149c742c9a449e0bd69951176ebbec1846fd5dee801`  
		Last Modified: Sat, 18 Dec 2021 07:01:11 GMT  
		Size: 58.8 MB (58820398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68eb256459888ae6b17f7e517d8d58d6d8ca94b48d7cd8d522d86a816917730a`  
		Last Modified: Sat, 18 Dec 2021 07:01:07 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-boot-2.8.3` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:3440d3b224fd19027305673934cf0586e8ab7f65d6cd8df587745ee465074eb2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.0 MB (278031220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7091da7811dfff2de61df3c42a5c9ecab7f0c6d8d0fa06f17358b1280fcf3416`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:09 GMT
ADD file:002f2f7c6dc806b24b6c365882acd59d2b3d3fcec46d8fd99130b07a4575c88c in / 
# Thu, 02 Dec 2021 08:08:10 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 11:02:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:02:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Thu, 02 Dec 2021 11:02:15 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 11:02:16 GMT
ENV LANG=C.UTF-8
# Fri, 17 Dec 2021 23:44:20 GMT
ENV JAVA_VERSION=18-ea+28
# Fri, 17 Dec 2021 23:44:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='7e5f0e54c799f8c155a934e61d88f4fef3a70a641c1636c925158622c7bd9341'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='e29aa39763ebcfe5f037cc4fe47c6b9eb34cbe482f6ea57e93de89070255e22b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 17 Dec 2021 23:44:36 GMT
CMD ["jshell"]
# Sat, 18 Dec 2021 00:35:08 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 18 Dec 2021 00:35:09 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 18 Dec 2021 00:35:10 GMT
WORKDIR /tmp
# Sat, 18 Dec 2021 00:35:15 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 18 Dec 2021 00:35:15 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 18 Dec 2021 00:35:16 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 18 Dec 2021 00:35:32 GMT
RUN boot
# Sat, 18 Dec 2021 00:35:33 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Sat, 18 Dec 2021 00:35:33 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 18 Dec 2021 00:35:34 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:968621624b326084ed82349252b333e649eaab39f71866edb2b9a4f847283680`  
		Last Modified: Thu, 02 Dec 2021 08:40:45 GMT  
		Size: 30.1 MB (30056536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595058421fcb005f80f2faa2434369885cb20645caed265e7b4912808701d893`  
		Last Modified: Thu, 02 Dec 2021 11:23:15 GMT  
		Size: 1.4 MB (1361242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6bb80b9448f431cc3c0af268f0b30679515f3d723763aecec0a9573c94e718`  
		Last Modified: Sat, 18 Dec 2021 00:03:31 GMT  
		Size: 187.7 MB (187729942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602140c07b0a07dffab63d55d9fa20df73d0c4faccf09879f891bb0094f91b22`  
		Last Modified: Sat, 18 Dec 2021 00:45:23 GMT  
		Size: 67.3 KB (67252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93beed4a8a1319ae025d38892d043d96251f9bf79afb955c7cb93ce88e4f0b39`  
		Last Modified: Sat, 18 Dec 2021 00:45:28 GMT  
		Size: 58.8 MB (58815843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae9b21cf6cb7b0fcadf570546b53c8388a0e6a99f7a41f1ddbf4825cca9718d`  
		Last Modified: Sat, 18 Dec 2021 00:45:23 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
