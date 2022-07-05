## `openjdk:19-oraclelinux8`

```console
$ docker pull openjdk@sha256:82b6a536489540c385f90018de76409cf7228f097de243c00e9553f49bd96bcd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:8732b6dd17d1fca7f60ea81605de0e8644df07a5b4ae67c24b364920048d08c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.9 MB (248881368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7181f7a3b61e135ccd2dd14c634c6eceda62a262c3b5968f6fccb52a88be33de`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 05 Jul 2022 22:20:34 GMT
ADD file:69555d6633d88e50ab2ddecc8bc5002a8f79005d828a9093975d68ca05b023e9 in / 
# Tue, 05 Jul 2022 22:20:34 GMT
CMD ["/bin/bash"]
# Tue, 05 Jul 2022 22:49:44 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 05 Jul 2022 22:50:40 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Tue, 05 Jul 2022 22:50:40 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Jul 2022 22:50:40 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jul 2022 22:50:40 GMT
ENV JAVA_VERSION=19-ea+29
# Tue, 05 Jul 2022 22:50:50 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/29/GPL/openjdk-19-ea+29_linux-x64_bin.tar.gz'; 			downloadSha256='04ada1133ef2771a80998706ff9168ca511e4f4e7c42b1ba4c9cdbd570d6cc31'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/29/GPL/openjdk-19-ea+29_linux-aarch64_bin.tar.gz'; 			downloadSha256='d2d5d6b1b6f1116f93a6f934f2fb03d8a4d257f0c72ad95c61a1aa2011ceb833'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 05 Jul 2022 22:50:51 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e54b73e95ef388354463a761e4e93ce3dac29cb244b2dc0424f2f4afc6ddf5cd`  
		Last Modified: Tue, 05 Jul 2022 22:21:41 GMT  
		Size: 39.2 MB (39222121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e62647f09f0ab1a3ac2d84823777bead33aa8e201c13b86c063296e8268023`  
		Last Modified: Tue, 05 Jul 2022 22:58:01 GMT  
		Size: 13.5 MB (13505357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd96c3a21fd31e18c2823815f90147b4d00aa7ac915e54c4bba4a9054d9117e`  
		Last Modified: Tue, 05 Jul 2022 22:59:49 GMT  
		Size: 196.2 MB (196153890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:097b5dd984dda7e5a3d9e5a66095865a7f4c2a5b97e630bb38b51fb5ff9d218c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.3 MB (247300292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da263f4aa87468a42fe639f2863a5a8cc5c9c967926e1db59f18cad685af5fb5`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 05 Jul 2022 22:43:14 GMT
ADD file:e864e9187ff57bc1df9611a0990052f89611bfe7b6bc8e3d24b500b0886ec725 in / 
# Tue, 05 Jul 2022 22:43:14 GMT
CMD ["/bin/bash"]
# Tue, 05 Jul 2022 23:04:00 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 05 Jul 2022 23:06:00 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Tue, 05 Jul 2022 23:06:01 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Jul 2022 23:06:02 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jul 2022 23:06:03 GMT
ENV JAVA_VERSION=19-ea+29
# Tue, 05 Jul 2022 23:06:20 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/29/GPL/openjdk-19-ea+29_linux-x64_bin.tar.gz'; 			downloadSha256='04ada1133ef2771a80998706ff9168ca511e4f4e7c42b1ba4c9cdbd570d6cc31'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/29/GPL/openjdk-19-ea+29_linux-aarch64_bin.tar.gz'; 			downloadSha256='d2d5d6b1b6f1116f93a6f934f2fb03d8a4d257f0c72ad95c61a1aa2011ceb833'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 05 Jul 2022 23:06:20 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e5d41499b4049578ed8bbb14817cd79d4136a84899b65e4364b0125d4d1c792c`  
		Last Modified: Tue, 05 Jul 2022 22:44:31 GMT  
		Size: 38.0 MB (38027757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c622a5406eea6948259fe9d62dd3f3f40ef71254cb260355242ef51e23880970`  
		Last Modified: Tue, 05 Jul 2022 23:20:55 GMT  
		Size: 14.3 MB (14282866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f383d125677643d9f502bb8cdc482bb1387443ff76fa51ac0ca2b478d879f`  
		Last Modified: Tue, 05 Jul 2022 23:23:09 GMT  
		Size: 195.0 MB (194989669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
