## `openjdk:17-ea-29-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:0f7951c05cdb40f4f767157ad6480b0b9545705e9ca38375338abf8562a5a3e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:17-ea-29-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:406ae992bc4c2f9a747252c016e5de99f9e3990ab6e6551bfc19926ffbe7ba81
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.7 MB (242707248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51c73ed7eb3ac6909d1b9bce46a49eeba1e0cd2ae1d1e52efcf131cf4fc6b160`
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
# Fri, 02 Jul 2021 19:26:29 GMT
ENV JAVA_VERSION=17-ea+29
# Fri, 02 Jul 2021 19:26:41 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/29/GPL/openjdk-17-ea+29_linux-x64_bin.tar.gz'; 			downloadSha256='c277cda62e368aa595450d3ffa018fbe98adc97c08e0ab777f5f74e86e3bf3f3'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/29/GPL/openjdk-17-ea+29_linux-aarch64_bin.tar.gz'; 			downloadSha256='8d5901a58b02e77d255166678c54cdc14c293d17730d794d70bb13434a934bb4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 02 Jul 2021 19:26:42 GMT
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
	-	`sha256:d232cb69bc19e391b23d86daf9fb513e382855a72df89b5869dc79fefeee3a95`  
		Last Modified: Fri, 02 Jul 2021 19:35:24 GMT  
		Size: 187.1 MB (187136575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-ea-29-jdk-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:012d71f1bb0e00027f908107105e35fdc3a6a919a1971005dbcbbf2c78f44396
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.2 MB (242167780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:891362e1b30a56bf9c868f6bafcdf00a259f267b7656c1378beade2d75a6b21b`
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
# Fri, 02 Jul 2021 19:31:53 GMT
ENV JAVA_VERSION=17-ea+29
# Fri, 02 Jul 2021 19:32:16 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/29/GPL/openjdk-17-ea+29_linux-x64_bin.tar.gz'; 			downloadSha256='c277cda62e368aa595450d3ffa018fbe98adc97c08e0ab777f5f74e86e3bf3f3'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/29/GPL/openjdk-17-ea+29_linux-aarch64_bin.tar.gz'; 			downloadSha256='8d5901a58b02e77d255166678c54cdc14c293d17730d794d70bb13434a934bb4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 02 Jul 2021 19:32:16 GMT
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
	-	`sha256:5e2d48f6731221028563c167dc2d7cda63c6b46f7c1351521fbeb6e06b079902`  
		Last Modified: Fri, 02 Jul 2021 19:47:52 GMT  
		Size: 185.9 MB (185943232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
