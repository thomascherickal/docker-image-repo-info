## `openjdk:18-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:b86d6e692f748b7da9d4dc72435d04efacbb6de4910aa17a2cc5905ba91591c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:c2ae403970ef62ce199a248ebe252e32198e1af538a7a6d8673905657b7bc5e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.6 MB (251648856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c08ea353fae76d7597abf1932dc479dcbcc4f717996fe2b5ab23b5ccf90a3d4`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 24 Mar 2022 22:26:41 GMT
ADD file:c54c465abf0c60dc924ca0809a1a862121214379efe90dacb9c9947c81054213 in / 
# Thu, 24 Mar 2022 22:26:42 GMT
CMD ["/bin/bash"]
# Fri, 25 Mar 2022 01:17:16 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 25 Mar 2022 01:18:00 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Fri, 25 Mar 2022 01:18:00 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 25 Mar 2022 01:18:01 GMT
ENV LANG=en_US.UTF-8
# Fri, 25 Mar 2022 01:18:01 GMT
ENV JAVA_VERSION=18
# Fri, 25 Mar 2022 01:18:10 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18/43f95e8614114aeaa8e8a5fcf20a682d/36/GPL/openjdk-18_linux-x64_bin.tar.gz'; 			downloadSha256='0f60aef7b8504983d6e374fe94d09a7bedcf05ec559e812d801a33bd4ebd23d0'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18/43f95e8614114aeaa8e8a5fcf20a682d/36/GPL/openjdk-18_linux-aarch64_bin.tar.gz'; 			downloadSha256='dff2860ba24c3f70f32ad3ac9b03f768dd28044bbda87c9607654fd03795c2ab'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 25 Mar 2022 01:18:11 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:fda5369ef22868b2225eb458f776aabaf140371e2f8d709c4de99b69a02ae748`  
		Last Modified: Thu, 24 Mar 2022 22:28:00 GMT  
		Size: 48.7 MB (48749451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:175ebd0783e9e11a5749d6a07553e79af5cce82b84020eca354389f2e772070e`  
		Last Modified: Fri, 25 Mar 2022 01:25:40 GMT  
		Size: 14.2 MB (14229382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c5400659f550b6d49e73b80bd0c3abbb0b131821a686469bf328853e42770b`  
		Last Modified: Fri, 25 Mar 2022 01:27:14 GMT  
		Size: 188.7 MB (188670023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:c313368037156e8022b07279227efb34b5f0d2baaba6042410f78e7911a00697
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.2 MB (252203076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96a4bcabf8021fbeeced1fc908fcd1ff91c9677ed59ee6c11f419f3a75b40318`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 24 Mar 2022 22:21:33 GMT
ADD file:458f691e62c6797d5a132b3af3e3d34358f4563c2f767879ff5a5edaac9c76ee in / 
# Thu, 24 Mar 2022 22:21:34 GMT
CMD ["/bin/bash"]
# Thu, 24 Mar 2022 22:46:20 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 24 Mar 2022 22:47:34 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 24 Mar 2022 22:47:35 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 22:47:36 GMT
ENV LANG=en_US.UTF-8
# Thu, 24 Mar 2022 22:47:37 GMT
ENV JAVA_VERSION=18
# Thu, 24 Mar 2022 22:47:53 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18/43f95e8614114aeaa8e8a5fcf20a682d/36/GPL/openjdk-18_linux-x64_bin.tar.gz'; 			downloadSha256='0f60aef7b8504983d6e374fe94d09a7bedcf05ec559e812d801a33bd4ebd23d0'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18/43f95e8614114aeaa8e8a5fcf20a682d/36/GPL/openjdk-18_linux-aarch64_bin.tar.gz'; 			downloadSha256='dff2860ba24c3f70f32ad3ac9b03f768dd28044bbda87c9607654fd03795c2ab'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 24 Mar 2022 22:47:53 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3a4f104bbb26007de614fa29a9ed91e9210287087323d3de394a39f0d9f1139c`  
		Last Modified: Thu, 24 Mar 2022 22:23:06 GMT  
		Size: 49.3 MB (49340038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a5491893ff1eefd4a92b9f85621f8ee58a84cb7d0fa6edf8ca55ed7dad5724`  
		Last Modified: Thu, 24 Mar 2022 23:02:13 GMT  
		Size: 15.3 MB (15270343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3d09b2479a1cf103580cb6a69012d2124fdb58e4a8bc5d8f0355c73fc14ea4`  
		Last Modified: Thu, 24 Mar 2022 23:04:05 GMT  
		Size: 187.6 MB (187592695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
