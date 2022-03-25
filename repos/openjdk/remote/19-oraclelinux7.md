## `openjdk:19-oraclelinux7`

```console
$ docker pull openjdk@sha256:de3c419115524b69b148118b5890e89b78732b869fa35f95b49892e858700367
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:6603efc489e55fa6f448a7c402113850b12a861152ffe9e267cc635b6a337a24
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.1 MB (256067886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:076e8a7acfb6da44eb04ac5bf9be12ee49efba6af9c6170d696dc486e8acc7fb`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 24 Mar 2022 22:26:41 GMT
ADD file:c54c465abf0c60dc924ca0809a1a862121214379efe90dacb9c9947c81054213 in / 
# Thu, 24 Mar 2022 22:26:42 GMT
CMD ["/bin/bash"]
# Fri, 25 Mar 2022 01:17:16 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 25 Mar 2022 01:17:17 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Fri, 25 Mar 2022 01:17:17 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 25 Mar 2022 01:17:17 GMT
ENV LANG=en_US.UTF-8
# Fri, 25 Mar 2022 01:17:17 GMT
ENV JAVA_VERSION=19-ea+14
# Fri, 25 Mar 2022 01:17:26 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/14/GPL/openjdk-19-ea+14_linux-x64_bin.tar.gz'; 			downloadSha256='7c64317f728ce251b1fa6fcc612bbc5e4fac4d2862cf0f9b9edd98800072b6bc'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/14/GPL/openjdk-19-ea+14_linux-aarch64_bin.tar.gz'; 			downloadSha256='166aaa023baf2fff6484465efd16040557b4bbd57362409d730acec5d01fe749'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 25 Mar 2022 01:17:27 GMT
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
	-	`sha256:36151540928ef42a2d9e10eeb6e004ab906ccc1e1dc9edcc49f9b8376ac362d4`  
		Last Modified: Fri, 25 Mar 2022 01:25:52 GMT  
		Size: 193.1 MB (193089053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:f4cbcea239a1daccc71c709c60892d0ed4b9cf486c237269db7775d89b570c34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.7 MB (256730018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6349c3529e551190755bf503504100cd7b6e899baeae71288112ba369c03326e`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 24 Mar 2022 22:21:33 GMT
ADD file:458f691e62c6797d5a132b3af3e3d34358f4563c2f767879ff5a5edaac9c76ee in / 
# Thu, 24 Mar 2022 22:21:34 GMT
CMD ["/bin/bash"]
# Thu, 24 Mar 2022 22:46:20 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 24 Mar 2022 22:46:20 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Thu, 24 Mar 2022 22:46:21 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 22:46:22 GMT
ENV LANG=en_US.UTF-8
# Thu, 24 Mar 2022 22:46:23 GMT
ENV JAVA_VERSION=19-ea+14
# Thu, 24 Mar 2022 22:46:40 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/14/GPL/openjdk-19-ea+14_linux-x64_bin.tar.gz'; 			downloadSha256='7c64317f728ce251b1fa6fcc612bbc5e4fac4d2862cf0f9b9edd98800072b6bc'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/14/GPL/openjdk-19-ea+14_linux-aarch64_bin.tar.gz'; 			downloadSha256='166aaa023baf2fff6484465efd16040557b4bbd57362409d730acec5d01fe749'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 24 Mar 2022 22:46:40 GMT
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
	-	`sha256:8d7fec4a9c0560ac5383d8165de8320c09985b26303c3bc962391b5e17c10028`  
		Last Modified: Thu, 24 Mar 2022 23:02:28 GMT  
		Size: 192.1 MB (192119637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
