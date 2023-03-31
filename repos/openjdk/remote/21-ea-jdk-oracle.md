## `openjdk:21-ea-jdk-oracle`

```console
$ docker pull openjdk@sha256:a21282c8bc58314e1aa9cd83a86a0cbe3bc264bc9a13ab657b1c1bd2a86952e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:1e765dd1a8f6fa157fa6d33f42f7e2afd816a907f517fb90211775966d05328c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261139952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c451870e361cf7f6dc5c0c57a64b1acb82c67c89864da9030edd65bca9c266a`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 29 Mar 2023 00:21:35 GMT
ADD file:728bdb9bb48c571a53579f02c3df258a071a1612cb28160c8348fd0b83893f1a in / 
# Wed, 29 Mar 2023 00:21:35 GMT
CMD ["/bin/bash"]
# Wed, 29 Mar 2023 00:39:18 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 29 Mar 2023 00:39:18 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Wed, 29 Mar 2023 00:39:18 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 00:39:18 GMT
ENV LANG=C.UTF-8
# Wed, 29 Mar 2023 00:39:18 GMT
ENV JAVA_VERSION=21-ea+15
# Wed, 29 Mar 2023 00:39:28 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/15/GPL/openjdk-21-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='0fec1002b8c8975b181bd6966a817028d6b373cbc759254231f9b96db1fe6edd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/15/GPL/openjdk-21-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='93cc1eb6202093a127f1f9ed2e866a51dff29321f878085c18f317cefb113ffc'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 29 Mar 2023 00:39:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d98f7984035168bbebf20a188b8cf4aa680c740ceff10816dcbbd32a58483843`  
		Last Modified: Wed, 29 Mar 2023 00:23:00 GMT  
		Size: 44.6 MB (44562176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b76522ebbbebe1d33d391848d9f7910bda3808bb7ca0ec5f2a7f84db25521768`  
		Last Modified: Wed, 29 Mar 2023 00:40:36 GMT  
		Size: 15.0 MB (15006652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e21df7acaee6af113a84facd0a98a4333a3b99a721e8a086a1d8ec388cf026c`  
		Last Modified: Wed, 29 Mar 2023 00:40:48 GMT  
		Size: 201.6 MB (201571124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:62053110fd596d64a7b41d2ff5b8f09e834b9a9f511274e97f4fb744372e8790
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.4 MB (259356453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1de3d35ce520980655a1626680f68d056e9f0284d5f463ada627249c514c0d61`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 31 Mar 2023 21:40:18 GMT
ADD file:c201d04749a3d092a7936542e4e280194ac00d3a3f3e3cd1722455429b0c4d18 in / 
# Fri, 31 Mar 2023 21:40:19 GMT
CMD ["/bin/bash"]
# Fri, 31 Mar 2023 22:07:22 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 31 Mar 2023 22:07:22 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Fri, 31 Mar 2023 22:07:22 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 31 Mar 2023 22:07:22 GMT
ENV LANG=C.UTF-8
# Fri, 31 Mar 2023 22:07:22 GMT
ENV JAVA_VERSION=21-ea+15
# Fri, 31 Mar 2023 22:07:36 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/15/GPL/openjdk-21-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='0fec1002b8c8975b181bd6966a817028d6b373cbc759254231f9b96db1fe6edd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/15/GPL/openjdk-21-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='93cc1eb6202093a127f1f9ed2e866a51dff29321f878085c18f317cefb113ffc'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 31 Mar 2023 22:07:37 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e83b78392ad9185bc4dcd144ceb39aea57035dc1457949ceaa1ac05c786aeaab`  
		Last Modified: Fri, 31 Mar 2023 21:41:31 GMT  
		Size: 43.5 MB (43477120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e92b3e3d0e23cc44a53dbd0cd2db3c27142b9fab15cb207c1444dad9ab16eb`  
		Last Modified: Fri, 31 Mar 2023 22:08:55 GMT  
		Size: 15.8 MB (15844880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59d16d0b0f5ed1826fa9bc027a183c3f90ec477a7bc65b7b3ac47b523bf2bec`  
		Last Modified: Fri, 31 Mar 2023 22:09:05 GMT  
		Size: 200.0 MB (200034453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
