## `openjdk:20-ea-23-jdk-oracle`

```console
$ docker pull openjdk@sha256:d5595d087163e6f0db51ed58573f8ac25bfff3e8ed761236362159bf0fdd5a95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-23-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:b4ee01ca5c7925026250fb6971709a16f311b49e3717029b230f2da591897a1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.0 MB (251042264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bab8184f21de35719e60326e04a9acee05af4b203e6c1f94d7d40be566b1f75`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 04 Nov 2022 23:33:07 GMT
ADD file:00e6899b8d3eccf7f795d17f9316af6ae0f3955ef2204b61bd064f5173c18357 in / 
# Fri, 04 Nov 2022 23:33:07 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:19:43 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Sat, 05 Nov 2022 02:19:44 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Sat, 05 Nov 2022 02:19:44 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 02:19:44 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 00:55:46 GMT
ENV JAVA_VERSION=20-ea+23
# Fri, 11 Nov 2022 00:55:59 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-x64_bin.tar.gz'; 			downloadSha256='0344aa24310a388514ddbc4a0279a9e28f222ae783ac918860ef8f13cfebabbe'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-aarch64_bin.tar.gz'; 			downloadSha256='57ae94d8d6968fc4b6603eab15361e998664b7bb1707611dfa4ab9542c17fd24'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Nov 2022 00:56:00 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:feec22b5b79860f47a87861bed3a29d5431a279cc239b44a2522a9ab5459d844`  
		Last Modified: Fri, 04 Nov 2022 23:34:48 GMT  
		Size: 40.6 MB (40580917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab968c9bcaf076780e21bb249a61cd5dfda4716508c17678f3082057a3c9b8f8`  
		Last Modified: Sat, 05 Nov 2022 02:23:30 GMT  
		Size: 12.2 MB (12229784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf6385da395568951fb61497c938edf2fd6a188ddde7d7db5494360a2511b5e`  
		Last Modified: Fri, 11 Nov 2022 01:00:08 GMT  
		Size: 198.2 MB (198231563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-23-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:9d7f15521d7f7db2ea9638d20e3777aabca3f3600d7dfc59fae3b64d59aff39d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.2 MB (249243808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7a66440227e5c03e2cd4b6f21004555d62c856096992422f43ec601bc655e66`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 04 Nov 2022 22:50:08 GMT
ADD file:efa6454225ba5be177493364c69d425968d42231b708b5d492a41f9ab14d64f4 in / 
# Fri, 04 Nov 2022 22:50:08 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 00:48:43 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Sat, 05 Nov 2022 00:48:43 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Sat, 05 Nov 2022 00:48:43 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 00:48:43 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 11:33:30 GMT
ENV JAVA_VERSION=20-ea+23
# Fri, 11 Nov 2022 11:33:38 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-x64_bin.tar.gz'; 			downloadSha256='0344aa24310a388514ddbc4a0279a9e28f222ae783ac918860ef8f13cfebabbe'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-aarch64_bin.tar.gz'; 			downloadSha256='57ae94d8d6968fc4b6603eab15361e998664b7bb1707611dfa4ab9542c17fd24'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Nov 2022 11:33:40 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a13cd8cb50ab4c8c5cb15a9929fa5faf1b7833f87c827551a9a54e84789b1e0b`  
		Last Modified: Fri, 04 Nov 2022 22:51:35 GMT  
		Size: 39.4 MB (39401738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2b575a486b4b7df2602a19466f69783be33126ccdea7a939dbef7ecc85a7c7`  
		Last Modified: Sat, 05 Nov 2022 00:53:50 GMT  
		Size: 13.0 MB (13049666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a80be26959592a5861c6f1306a65cf2b59f4b8127eaaa22c99a4e74ed04281`  
		Last Modified: Fri, 11 Nov 2022 11:37:55 GMT  
		Size: 196.8 MB (196792404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
