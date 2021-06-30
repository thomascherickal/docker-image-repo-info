## `openjdk:17-ea-28-oracle`

```console
$ docker pull openjdk@sha256:c05a57e6656af263346e335966d4bafc6eb7433fb8963d5c9a62dfbdd984d247
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:17-ea-28-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:b823292cb4065a96238ffa7ca5358bda019df30ed0c6dfe676d8af08222264d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.7 MB (242682194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:751cfcc067d2769aac9859d5203c176905f04989f573123e78375037d814d9b5`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 30 Jun 2021 17:23:40 GMT
ADD file:d49890823c4e8287f936eec210400575f79c20f14f048017368faed0584841a6 in / 
# Wed, 30 Jun 2021 17:23:41 GMT
CMD ["/bin/bash"]
# Wed, 30 Jun 2021 17:40:57 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 30 Jun 2021 17:43:12 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Wed, 30 Jun 2021 17:43:12 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Jun 2021 17:43:12 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 17:43:13 GMT
ENV JAVA_VERSION=17-ea+28
# Wed, 30 Jun 2021 17:43:24 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/28/GPL/openjdk-17-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='29f489da387fdabce2ebfbb74f474c424ed9c92380783da511d8ab1ed5dee912'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/28/GPL/openjdk-17-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='60752f6f44e478db934f4dc4b9a7cb715387ae964fb353e469dd986a5aeaf92b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 30 Jun 2021 17:43:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9660ffb7976c51eb47b4425f6bb95173c170f4fcc442a2bb2b6ba7bf154f6fc8`  
		Last Modified: Wed, 30 Jun 2021 17:25:00 GMT  
		Size: 42.2 MB (42179226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f8b4ca74ea5f238671d4c7981ca7c99e6c70d3fcd8d4d0596ccdf6b8329dbe`  
		Last Modified: Wed, 30 Jun 2021 17:50:04 GMT  
		Size: 13.4 MB (13391447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da92b3bc8acc347b4c113e7f363ec20753cc078e7d01c51b81e9d89543008cc`  
		Last Modified: Wed, 30 Jun 2021 17:51:21 GMT  
		Size: 187.1 MB (187111521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-ea-28-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:e8d87ffa883a55864a8b8c205b2ff28ee5b3e57fa10f4df1391cad8cc7d1abd7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.1 MB (242138643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:274d588d701f9305efe12256f22ac2a05c37273f8f509c43838c555e41f4f85d`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 30 Jun 2021 16:40:33 GMT
ADD file:c33580f17660c9afa2637bda7e6cf34d631535b13ffc1535bb21cfb0ab7bdb5c in / 
# Wed, 30 Jun 2021 16:40:33 GMT
CMD ["/bin/bash"]
# Wed, 30 Jun 2021 17:08:45 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 30 Jun 2021 17:09:42 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Wed, 30 Jun 2021 17:09:42 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Jun 2021 17:09:43 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 17:09:43 GMT
ENV JAVA_VERSION=17-ea+28
# Wed, 30 Jun 2021 17:09:52 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/28/GPL/openjdk-17-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='29f489da387fdabce2ebfbb74f474c424ed9c92380783da511d8ab1ed5dee912'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/28/GPL/openjdk-17-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='60752f6f44e478db934f4dc4b9a7cb715387ae964fb353e469dd986a5aeaf92b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 30 Jun 2021 17:09:53 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e02c40d2e97c148eec83200018cd774bcf09562d984b2237577a0bebd5900481`  
		Last Modified: Wed, 30 Jun 2021 16:41:47 GMT  
		Size: 42.0 MB (42045297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c341a81c74999386f57f0e8e08448131a5297ce89816bbfe58e5d804b6e1384`  
		Last Modified: Wed, 30 Jun 2021 17:21:19 GMT  
		Size: 14.2 MB (14179251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eeb872558aabedcdaa6adbd459087dad5be3d43f9e1f8644a88a49bf7d146c1`  
		Last Modified: Wed, 30 Jun 2021 17:22:58 GMT  
		Size: 185.9 MB (185914095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
