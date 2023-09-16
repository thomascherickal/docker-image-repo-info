## `openjdk:21-oracle`

```console
$ docker pull openjdk@sha256:fb91003c9bfa4ac50394e1d29b82c8398ff8282e37373fc66023e8b56b282e70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:e13fa44915f842eeee56a554bd9b828102aac5e5e92e40fd34721a18d3c89775
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.8 MB (263846988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3776133e019a351e65c03dbd640e0f1b7f833f34d253ed482ce9bddd5377baa0`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:54 GMT
ADD file:1632d5b9918ff63c9e38191b65ad8e6f1e0eb5c2ef274cce4f50534bba2f7493 in / 
# Sat, 16 Sep 2023 02:40:55 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 02:53:11 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Sat, 16 Sep 2023 02:53:42 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Sat, 16 Sep 2023 02:53:42 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 Sep 2023 02:53:42 GMT
ENV LANG=C.UTF-8
# Sat, 16 Sep 2023 02:53:42 GMT
ENV JAVA_VERSION=21
# Sat, 16 Sep 2023 02:53:53 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_linux-x64_bin.tar.gz'; 			downloadSha256='a30c454a9bef8f46d5f1bf3122830014a8fbe7ac03b5f8729bc3add4b92a1d0a'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_linux-aarch64_bin.tar.gz'; 			downloadSha256='e8f4ed1a69815ddf56d7da365116eefc1e5a1159396dffee3dd21616a86d5d28'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 16 Sep 2023 02:53:54 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bc377bce3181aab0e51009b13b6a6890e49c64e7bf6ab7fa12dce86a95c88bd4`  
		Last Modified: Sat, 16 Sep 2023 02:42:29 GMT  
		Size: 44.9 MB (44911063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fe7d94225755f280f5249e52cf0633729ae0585805f1912428007f164e1d7e`  
		Last Modified: Sat, 16 Sep 2023 02:54:54 GMT  
		Size: 15.0 MB (15001921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd2d43889c653bfac5c3a0efa6cb92ead52feccd72d893443fe520818622d90`  
		Last Modified: Sat, 16 Sep 2023 02:56:17 GMT  
		Size: 203.9 MB (203934004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:b2a7756a6ffc8d8a9fc15c7bc5a7435389a99b3a78dbe9c7734cec63d32c5a2d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.6 MB (261579684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dd372107973c64680041c0313e66e4e35eb376006c111b16a314fc844b95a06`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 16 Sep 2023 02:21:42 GMT
ADD file:c1b7bfaf11bf64b9c1b24345749a98cbd3f593162ea942e12b15c6f2110c1e94 in / 
# Sat, 16 Sep 2023 02:21:43 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 02:49:47 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Sat, 16 Sep 2023 02:50:19 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Sat, 16 Sep 2023 02:50:19 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 Sep 2023 02:50:19 GMT
ENV LANG=C.UTF-8
# Sat, 16 Sep 2023 02:50:19 GMT
ENV JAVA_VERSION=21
# Sat, 16 Sep 2023 02:50:30 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_linux-x64_bin.tar.gz'; 			downloadSha256='a30c454a9bef8f46d5f1bf3122830014a8fbe7ac03b5f8729bc3add4b92a1d0a'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_linux-aarch64_bin.tar.gz'; 			downloadSha256='e8f4ed1a69815ddf56d7da365116eefc1e5a1159396dffee3dd21616a86d5d28'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 16 Sep 2023 02:50:31 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d095360c6402749d9f7a3d7b7cdd417f27e41419f8027f4704ab00d0dd8ae7ee`  
		Last Modified: Sat, 16 Sep 2023 02:22:42 GMT  
		Size: 43.6 MB (43630964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7548ed69b34282ed3935dd421a868025a61827eb4d197bcee64f8ae913c858ad`  
		Last Modified: Sat, 16 Sep 2023 02:51:22 GMT  
		Size: 15.7 MB (15675185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59373ccb9849113c5d10995d08d736e9287d0602f359a8269754c29565b2ee48`  
		Last Modified: Sat, 16 Sep 2023 02:52:28 GMT  
		Size: 202.3 MB (202273535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
