## `openjdk:22-oraclelinux8`

```console
$ docker pull openjdk@sha256:c6211c6b7dc99ebc5bb572670534f9f65ee8a7f900b7a83b5986d5ffc63d21eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:22-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:c6f0b3a2a975af975495028a2243949ee877f57c3f55879bd4729441569e114c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.0 MB (264991966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc216b769f1faa6c9fef71de64826c86138c2db673424537f93a588483b3bbb0`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:54 GMT
ADD file:1632d5b9918ff63c9e38191b65ad8e6f1e0eb5c2ef274cce4f50534bba2f7493 in / 
# Sat, 16 Sep 2023 02:40:55 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 02:53:11 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Sat, 16 Sep 2023 02:53:11 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Sat, 16 Sep 2023 02:53:11 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 Sep 2023 02:53:11 GMT
ENV LANG=C.UTF-8
# Sat, 16 Sep 2023 02:53:11 GMT
ENV JAVA_VERSION=22-ea+15
# Sat, 16 Sep 2023 02:53:24 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/15/GPL/openjdk-22-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='86b3ab4e12d302e039dc65fc4700ffd572d072d6d822c983a6d74b569b9186ef'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/15/GPL/openjdk-22-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='6c680f4dc89b64fbe5cfcf7b12f232e31737112a8801ac594416c21e4b04c892'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 16 Sep 2023 02:53:24 GMT
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
	-	`sha256:9a4a746de42f6c684ace484cf55415b8c197bc4e7ea2c033a58f67a0600ce0c9`  
		Last Modified: Sat, 16 Sep 2023 02:55:07 GMT  
		Size: 205.1 MB (205078982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:36238665f9adf15a79a7c1101e2fc49395a5dddf399f31cce4c0bc6f4bea4009
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.7 MB (262697640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:888e8f842cf46d61278010f96579727931e7333771949470fdf7b098258b82ee`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 16 Sep 2023 02:21:42 GMT
ADD file:c1b7bfaf11bf64b9c1b24345749a98cbd3f593162ea942e12b15c6f2110c1e94 in / 
# Sat, 16 Sep 2023 02:21:43 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 02:49:47 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Sat, 16 Sep 2023 02:49:47 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Sat, 16 Sep 2023 02:49:47 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 Sep 2023 02:49:47 GMT
ENV LANG=C.UTF-8
# Sat, 16 Sep 2023 02:49:47 GMT
ENV JAVA_VERSION=22-ea+15
# Sat, 16 Sep 2023 02:49:59 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/15/GPL/openjdk-22-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='86b3ab4e12d302e039dc65fc4700ffd572d072d6d822c983a6d74b569b9186ef'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/15/GPL/openjdk-22-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='6c680f4dc89b64fbe5cfcf7b12f232e31737112a8801ac594416c21e4b04c892'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 16 Sep 2023 02:50:00 GMT
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
	-	`sha256:ea1fef6e96a1b52fba3ce172e634ed96d0a9a630966a5bf6d7ba3cc07ea78c46`  
		Last Modified: Sat, 16 Sep 2023 02:51:33 GMT  
		Size: 203.4 MB (203391491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
