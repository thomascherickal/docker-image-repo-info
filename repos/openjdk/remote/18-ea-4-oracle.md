## `openjdk:18-ea-4-oracle`

```console
$ docker pull openjdk@sha256:93e0f1cde536ad05a6f1f630d79bd6d58b2dc2cf30de1f75c26e3a2de6f1ee14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-ea-4-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:66a49803b9232c9796871860893591b5dc37f5634079b5fc84dfebcaa0900f43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.4 MB (243431265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6284118bb15ba6fec340b35e825ee80acd3feaaad5dac5f503b3242086aa8d9`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 30 Jun 2021 17:23:40 GMT
ADD file:d49890823c4e8287f936eec210400575f79c20f14f048017368faed0584841a6 in / 
# Wed, 30 Jun 2021 17:23:41 GMT
CMD ["/bin/bash"]
# Wed, 30 Jun 2021 17:40:57 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 30 Jun 2021 17:40:58 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Wed, 30 Jun 2021 17:40:58 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Jun 2021 17:40:58 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jul 2021 19:25:22 GMT
ENV JAVA_VERSION=18-ea+4
# Fri, 02 Jul 2021 19:25:33 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/4/GPL/openjdk-18-ea+4_linux-x64_bin.tar.gz'; 			downloadSha256='716cfd996b255bbad0b3d17027e5637bf2cf30bf320339116c661d63e797a324'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/4/GPL/openjdk-18-ea+4_linux-aarch64_bin.tar.gz'; 			downloadSha256='d2c4885f81f8be83225ef11849eaaa35af6af01337b90435d9abb8b4138d2795'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 02 Jul 2021 19:25:33 GMT
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
	-	`sha256:723de75bb2103323f9d145315cff6cfc7c60348e1f69e78b43d2ca48405d94ab`  
		Last Modified: Fri, 02 Jul 2021 19:32:32 GMT  
		Size: 187.9 MB (187860592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-4-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:f9fdab364752537c0f05e5516895ab3cfbe337789687c13801efff67ea5a8b69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.8 MB (242785255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:149988ff9b39e1a0d4d9f4233edd817ddd4544de42ffb5a3deaaf352ff067fc8`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 30 Jun 2021 16:40:33 GMT
ADD file:c33580f17660c9afa2637bda7e6cf34d631535b13ffc1535bb21cfb0ab7bdb5c in / 
# Wed, 30 Jun 2021 16:40:33 GMT
CMD ["/bin/bash"]
# Wed, 30 Jun 2021 17:08:45 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 30 Jun 2021 17:08:45 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Wed, 30 Jun 2021 17:08:46 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Jun 2021 17:08:46 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jul 2021 19:30:02 GMT
ENV JAVA_VERSION=18-ea+4
# Fri, 02 Jul 2021 19:30:28 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/4/GPL/openjdk-18-ea+4_linux-x64_bin.tar.gz'; 			downloadSha256='716cfd996b255bbad0b3d17027e5637bf2cf30bf320339116c661d63e797a324'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/4/GPL/openjdk-18-ea+4_linux-aarch64_bin.tar.gz'; 			downloadSha256='d2c4885f81f8be83225ef11849eaaa35af6af01337b90435d9abb8b4138d2795'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 02 Jul 2021 19:30:28 GMT
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
	-	`sha256:2573d0e1c910ac0b52babc67c9f9c9e87954ef125078319f5d916a75987c2617`  
		Last Modified: Fri, 02 Jul 2021 19:44:13 GMT  
		Size: 186.6 MB (186560707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
