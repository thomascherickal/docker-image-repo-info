## `openjdk:21-ea-34-jdk-oracle`

```console
$ docker pull openjdk@sha256:44f169e03d70cb2f6d4b812652f6d88e2a8f7f5990fbb248eaf1e857581f39ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-34-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:899f55e83ba1bbdbf5eeb9c959d24c17370e7135ea7f7a05bb772da9722f5aeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.8 MB (263846440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13e035ec8fcfca2cb07bd31269327747c4de8177e00b735506b77146cde0cb0d`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 11 Aug 2023 01:20:36 GMT
ADD file:196115c6281a0a56854066be2766eb0dc9da452f60a060b90bbe681e6b8ffc11 in / 
# Fri, 11 Aug 2023 01:20:36 GMT
CMD ["/bin/bash"]
# Fri, 11 Aug 2023 01:53:51 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 11 Aug 2023 01:54:38 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Fri, 11 Aug 2023 01:54:38 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Aug 2023 01:54:38 GMT
ENV LANG=C.UTF-8
# Fri, 11 Aug 2023 01:54:38 GMT
ENV JAVA_VERSION=21-ea+34
# Fri, 11 Aug 2023 01:55:02 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/34/GPL/openjdk-21-ea+34_linux-x64_bin.tar.gz'; 			downloadSha256='d16356385a726320077563c6180f2eabf72ded64b5695f24f3e7a2d3980b1f11'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/34/GPL/openjdk-21-ea+34_linux-aarch64_bin.tar.gz'; 			downloadSha256='cb862b1f34e15c99aacab2c9e6ed259ad056eaa3dfc547ebc6026630db64af94'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Aug 2023 01:55:03 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b193354265ba898bb7548038f52378b3dbb6aac5afbaca49bb83ccfe51dfadeb`  
		Last Modified: Fri, 11 Aug 2023 01:21:58 GMT  
		Size: 44.9 MB (44910081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e75d2bbaed8a6321c319c610e5cd0923e1fc6a9ad6122e3b9573f10a5166f9e`  
		Last Modified: Fri, 11 Aug 2023 01:56:08 GMT  
		Size: 15.0 MB (15004378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14feb7742244847f6caaea8c7c590fbe02a1d984871ee0bc04043bc8a00c5a08`  
		Last Modified: Fri, 11 Aug 2023 01:57:18 GMT  
		Size: 203.9 MB (203931981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-34-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:659b0f85de2f031b3393213c164e40143a84024d6946ac9bf360538f99b83a7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.6 MB (261560882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba8e53658b9a973129890e482df183a703997e469b77457c8165eb8bdf2f99c1`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 11 Aug 2023 00:40:33 GMT
ADD file:24663feb951dcfae36948e6cbc8697e8bef563d86c15af3daa54a1b830965593 in / 
# Fri, 11 Aug 2023 00:40:34 GMT
CMD ["/bin/bash"]
# Fri, 11 Aug 2023 01:11:14 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 11 Aug 2023 01:11:44 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Fri, 11 Aug 2023 01:11:44 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Aug 2023 01:11:44 GMT
ENV LANG=C.UTF-8
# Fri, 11 Aug 2023 01:11:44 GMT
ENV JAVA_VERSION=21-ea+34
# Fri, 11 Aug 2023 01:11:59 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/34/GPL/openjdk-21-ea+34_linux-x64_bin.tar.gz'; 			downloadSha256='d16356385a726320077563c6180f2eabf72ded64b5695f24f3e7a2d3980b1f11'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/34/GPL/openjdk-21-ea+34_linux-aarch64_bin.tar.gz'; 			downloadSha256='cb862b1f34e15c99aacab2c9e6ed259ad056eaa3dfc547ebc6026630db64af94'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Aug 2023 01:12:01 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bd2ec1b01835c3bcf117123886f982435cd8e445790b761779f35779d61faad3`  
		Last Modified: Fri, 11 Aug 2023 00:41:41 GMT  
		Size: 43.6 MB (43625591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7023146e285ffba3adcf0df2d0ef98b1f28c00ef46b2ffc20a5c3d01540eba`  
		Last Modified: Fri, 11 Aug 2023 01:13:09 GMT  
		Size: 15.7 MB (15666637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0f94eb1652cb21489d1a1719225ceb4b47f1694be38e244e6b95d9f32990a6`  
		Last Modified: Fri, 11 Aug 2023 01:14:14 GMT  
		Size: 202.3 MB (202268654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
