## `openjdk:21-ea-oraclelinux8`

```console
$ docker pull openjdk@sha256:f7710daa243de359dd1fbd7999c93f8a90fc27f075e7f5537fc9237aca869477
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:a28e83c325f912b59edb3820fc53f3778346f3fdee6c6f2012c783ac39c552c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.7 MB (263706891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:814f02636c0d5d877cb3c40910ef0e14ac44f5cf70214902cf1937368ecf107a`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 16 Jun 2023 00:20:42 GMT
ADD file:9f649031a04a4d0b24cc167d52bbd5ae3415fd808304c971291e35e75109822a in / 
# Fri, 16 Jun 2023 00:20:43 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:40:59 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 16 Jun 2023 00:41:30 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Fri, 16 Jun 2023 00:41:31 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 00:41:31 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 00:41:31 GMT
ENV JAVA_VERSION=21-ea+26
# Fri, 16 Jun 2023 00:41:41 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/26/GPL/openjdk-21-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='16c6b09c742e73c9e092134517ecc36db2a5e44453c8b8b5374cfac1ee367a28'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/26/GPL/openjdk-21-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='aa59bb222c548c18c21cb05a71854a46263a618a72ec6f2f408328689280380d'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 16 Jun 2023 00:41:42 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:46ef68baacb785b3cf2f2826bfce791acb5264bed0fdf301623ac0c3c57f4daf`  
		Last Modified: Fri, 16 Jun 2023 00:22:14 GMT  
		Size: 44.9 MB (44871780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df40f423a19e7cc991828aa15e47b0b84747ce895ae0ee55b8298f3bc44f03a3`  
		Last Modified: Fri, 16 Jun 2023 00:42:40 GMT  
		Size: 15.0 MB (15006208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3cd0e7dde4836e262b6ac396f4b0aa054b696b63d8871a509cc6f6ffe39aee`  
		Last Modified: Fri, 16 Jun 2023 00:43:42 GMT  
		Size: 203.8 MB (203828903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:d39168aa1aa08306cc7330e03aeae238e6b90a1e181cd82819229c352634b7f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.4 MB (261445740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d54493c4d9e620b05d91d4ad257c4f8ee23068ce7c17ecb0a4d5e6ee14f1ab5`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 15 Jun 2023 23:40:30 GMT
ADD file:37cef5fcd08f57d005adb8f14f69ecc78a9c669280f45f7d81b1c899489e93ba in / 
# Thu, 15 Jun 2023 23:40:31 GMT
CMD ["/bin/bash"]
# Thu, 15 Jun 2023 23:59:49 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 16 Jun 2023 00:00:10 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Fri, 16 Jun 2023 00:00:10 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 00:00:11 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 00:00:11 GMT
ENV JAVA_VERSION=21-ea+26
# Fri, 16 Jun 2023 00:00:19 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/26/GPL/openjdk-21-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='16c6b09c742e73c9e092134517ecc36db2a5e44453c8b8b5374cfac1ee367a28'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/26/GPL/openjdk-21-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='aa59bb222c548c18c21cb05a71854a46263a618a72ec6f2f408328689280380d'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 16 Jun 2023 00:00:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:029ab4a5f8e75aadbbba1505624cf10a4c35a0fd897cc85b9e7536785b8ba37c`  
		Last Modified: Thu, 15 Jun 2023 23:41:45 GMT  
		Size: 43.6 MB (43601336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cca9ab147b9b93cf01a583c33e8ade844f6d31bfb69334e1614ef5dd4d6a973`  
		Last Modified: Fri, 16 Jun 2023 00:01:25 GMT  
		Size: 15.7 MB (15673775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e8ecd9a6a9f7f006a2749ab8d2e70b8093b984a849d945f467a03d574acd69`  
		Last Modified: Fri, 16 Jun 2023 00:02:28 GMT  
		Size: 202.2 MB (202170629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
